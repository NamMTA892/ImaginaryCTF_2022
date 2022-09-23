Đề bài:
![Imgur](https://i.imgur.com/jiCxhH9.png)
![Imgur](https://i.imgur.com/ppoQTBc.png)

Ở đây bài đã chỉ ra dòng flag đỏ là fake. Chúng ta có 1 cái hint ở dưới là: Please enable JS to view the flag.

Khi mình nhìn vào trong <body> của bài, tag <script> không triển khai để hiện flag và mình đã chú ý đến đoạn fetch('/totallynottheflag')
![Imgur](https://i.imgur.com/wvIPiH0.png)

Fetch() cho phép tạo một network request tương tự như XMLHttpRequest(XHR). 
Vì vậy mình đã truy cập vào /totallynottheflag.
![Imgur](https://i.imgur.com/RT9VbPC.png)

flag: ictf{gr333333333333333n_flags_are_g00d_tho}
