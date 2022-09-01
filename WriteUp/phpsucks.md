Đề bài:
![Imgur](https://i.imgur.com/5JUcvfJ.png)
![Imgur](https://i.imgur.com/ToEwB3h.png)

Để bypass qua Preg_match() mình truyền vào array nhưng không hoạt động(do eval(); ):
![Imgur](https://i.imgur.com/WjQBl7e.png)

Nhưng do không hoạt động nên mình đã nghĩ đến sử dụng PHPFuck:
![Imgur](https://i.imgur.com/LD5Kz1O.png)

Đề bài chỉ cho độ dài đầu vào 100 nên mình đã thất bại :))).
Rồi mình đã tìm được kĩ thuật bypass qua preg_match và có đầu vào truyền vào eval();.
Mình sẽ giải thích qua kĩ thuật này:
    Trong PHP, lời gọi hàm có thể thực thi:
![Imgur](https://i.imgur.com/wkVvxTM.png)

    Kỹ thuật sử dụng lệnh XOR:
![Imgur](https://i.imgur.com/TlG9Ifw.png)

"?" sẽ được đổi ra mã ASCII là 63 và quy đổi ra nhị phân 00111111
"}" sẽ được đổi ra mã ASCII là 125 và quy đổi ra nhị phân 01111101
Sau khi XOR sẽ ra 01000010 và quy đổi sẽ ra kí tự "B"
Thông qua 2 phương pháp trên mình sẽ truyền vào: 
![Imgur](https://i.imgur.com/tieSo5U.png)
![Imgur](https://i.imgur.com/KD79Cp7.png)
![Imgur](https://i.imgur.com/eP3ph4F.png)

$_GET[__] để nhận các tham số
![Imgur](https://i.imgur.com/bvYVMpq.png)

Và kết quả:
![Imgur](https://i.imgur.com/LM4w29K.png)

flag:ictf{th3r3_4r3_n0_l4ngu4g3_l1k3_Php}

