# Đề bài:
![Imgur](https://i.imgur.com/iPX8iVz.png)

Ở bài này khi chúng ta kiểm tra bằng Dev Tools sẽ chỉ ra đường dẫn tới source code:
![Imgur](https://i.imgur.com/z5PGPIX.png)

Chúng ta sẽ chú ý vào 2 phần:
#### Phần thực thi:
![Imgur](https://i.imgur.com/0kR2iB7.png)

#### Phần kiểm tra và ra kết quả:
![Imgur](https://i.imgur.com/ZYik47G.png)

Ở phần thực thi chúng ta không thể bypass qua IPLocal bằng các phương pháp như X-Forwarded-For hay X-Client-Ip  
Vì vậy chúng ta cần bypass qua Object.assign()  
Bằng phương pháp Prototype Pollution và chuyển Content-Type sang dạng JSON:
![Imgur](https://i.imgur.com/M8Kl4T3.png)
