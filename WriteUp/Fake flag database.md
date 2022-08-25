Đề bài:
![Imgur](https://i.imgur.com/seJVk3X.png)

Khi chúng ta truy cập sẽ hiện ra 1 bảng Google sheet và ở đó chứa vài fakeflags của các bài khác.
Ở đây mình thấy có một Hidden Sheet và nó là phần Backend
![Imgur](https://i.imgur.com/2yvKB2n.png)

Mình thì chỉnh Show/Formulas để tìm thử một hướng đi
![Imgur](https://i.imgur.com/QLZXmrN.png)
![Imgur](https://i.imgur.com/oeM3Mt3.png)

Importrange()là hàm trong GGS có chứa năng cho đưa dữ liệu từ bảng khác vào bảng đang dùng với 2 tham số đầu vào
1. Link dẫn bảng cần thêm
2. [Tên bảng]![ Cột ]:[ Dòng ]
Khi thấy từ "Backend" thì mình sẽ thử truy cập thông qua nhập cột dòng trên GGS
![Imgur](https://i.imgur.com/jMfBWmN.png)
![Imgur](https://i.imgur.com/tFn4ikQ.png)

Tada!! Chúng ta đã truy cập vào Backend và tìm thấy flag.
flag: ictf{nothing_is_hidden_nothing_is_safe}
