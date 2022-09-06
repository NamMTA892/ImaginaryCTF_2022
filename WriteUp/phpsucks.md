Đề bài:
![Imgur](https://i.imgur.com/5JUcvfJ.png)
![Imgur](https://i.imgur.com/ToEwB3h.png)

Link:http://puzzler7.imaginaryctf.org:4011/  
Bài này chúng ta có rất nhiều cách khai thác:  
Cách 1: Byspass Preg_match() bằng array nhưng không hoạt động do không kích hoạt eval() để chạy.  
![Imgur](https://i.imgur.com/WjQBl7e.png)

Cách 2: Sử dụng PHPFuc*: nhưng do độ dài chuỗi nhập nhỏ hơn 100 nên không hoạt động.
![Imgur](https://i.imgur.com/LD5Kz1O.png)

Rồi mình đã tìm được kĩ thuật bypass qua preg_match và có đầu vào truyền vào eval();  
Mình sẽ giải thích qua kĩ thuật này:  
+Trong PHP, lời gọi hàm có thể thực thi bằng cách đặt tên biến là tên hàm và thêm () để gọi hàm:  
![Imgur](https://i.imgur.com/wkVvxTM.png)

+Áp dụng kỹ thuật trên, ta có kỹ thuật sử dụng lệnh XOR:
![Imgur](https://i.imgur.com/TlG9Ifw.png)

"?" sẽ được đổi ra mã ASCII là 63 và quy đổi ra nhị phân 00111111.
"}" sẽ được đổi ra mã ASCII là 125 và quy đổi ra nhị phân 01111101.
Sau khi XOR sẽ ra 01000010 và quy đổi sẽ ra kí tự "B".
Thông qua 2 phương pháp trên mình sẽ truyền vào: 
![Imgur](https://i.imgur.com/tieSo5U.png)
![Imgur](https://i.imgur.com/KD79Cp7.png)
![Imgur](https://i.imgur.com/eP3ph4F.png)

$_GET[__] để nhận các tham số
![Imgur](https://i.imgur.com/bvYVMpq.png)

Và kết quả:
![Imgur](https://i.imgur.com/LM4w29K.png)

flag:ictf{th3r3_4r3_n0_l4ngu4g3_l1k3_Php}

