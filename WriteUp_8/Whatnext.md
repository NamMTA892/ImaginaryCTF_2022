# Đề bài
![Imgur](https://i.imgur.com/DoudRhA.png)

Link source:https://imaginaryctf.org/f/5zCIW
Link bài: https://what-next.ictf.iciaran.com/
![Imgur](https://i.imgur.com/Hf75cCW.png)

2 phần Hello World và Imaginary Ctf đều là 2 phần lời chào, không có gì để khai thác.  

![Imgur](https://i.imgur.com/LdO6Us4.png)
![Imgur](https://i.imgur.com/PFw5VXN.png)

Khi mình truy cập vào Flag, nó sẽ dẫn mình vào đường dẫn /signin  
![Imgur](https://i.imgur.com/o7YUQxD.png)

Một điều mình nhận ra khá buồn cười là khi mình Go back lại paste, nó vẫn ở trong trang signin và trên thanh URL có sự thay đổi link dẫn rất nhanh. Khi mình reload lại trang thì nó xuất hiện dòng chờ  
![Imgur](https://i.imgur.com/cDzmQdg.png)

Sau đó reload lại page thì URL sẽ hiện ra dòng /protected/flag
![Imgur](https://i.imgur.com/Sd3SE8S.png)

Vì vậy mình quyết định đặt breakpoint và kiểm tra source của trang link /protected/flag
![Imgur](https://i.imgur.com/LxqGwGZ.png)

Base64 Decode và sẽ ra flag
Flag:ictf{sn34ky_st4t1c_g3n3r4t10n}
