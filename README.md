# Lab An toàn mạng máy tính
_An toàn mạng máy tính là việc bảo vệ hạ tầng mạng, dữ liệu và các thiết bị kết nối khỏi sự truy cập trái phép, phá hoại hoặc đánh cắp thông tin, vì vậy triển khai các biện pháp bảo vệ là rất quan trọng để đảm bảo tính toàn vẹn và sự vận hành liên tục của hệ thống_

## Triển khai Iptables
Iptables là một loại tường lửa mã nguồn mở được xây dựng trên hệ điều hành nhân linux, giúp quản lý các truy cập kết nối vào ra Internet và dịch vụ nội bộ. Giao diện dòng lệnh khá khó để thao tác. Chp phép quản trị viên tự thêm và xóa rule.
<img width="826" height="372" alt="image" src="https://github.com/user-attachments/assets/d9279366-3db3-4edb-ac13-7c612377217e" />

## Triển khai Pfsense
Pfsense là một loại tường lửa mã nguồn mở được xây dựng trên nhân Linux, có chức năng tương tự Iptables, ngoài ra còn cho phép triển khai dịch vụ VPN. Hỗ trợ quản lý, chạy shell, cấu hình thông qua ứng dụng web thân thiện.
<img width="1041" height="303" alt="image" src="https://github.com/user-attachments/assets/885b4089-0fb7-49c4-9ffe-d5b0fbebf757" />

<img width="976" height="498" alt="image" src="https://github.com/user-attachments/assets/ee770355-e465-493d-ba33-a05f64ef845e" />

## Triển khai IDPS-Snort
Snort là hệ thống giúp phát hiện và ngăn chặn sự xâm nhập trái phép mã nguồn mở, hỗ trở quản lý tốt trên hệ điều hành Linux. Là phần mềm có thể tải về hệ thống máy tính từ Internet, cấu hình và triển khai thông qua dòng lệnh. Có sẵn các tập luật, cũng cho phép thêm luật theo form của Snort. 
<img width="1323" height="223" alt="image" src="https://github.com/user-attachments/assets/f0bf7dae-cf16-4aa4-bfd6-98b49ad66bda" />

<img width="615" height="669" alt="image" src="https://github.com/user-attachments/assets/500e2a6e-263b-4baa-a52d-118daab64492" />

## Triển khai VPN client to side (VPN remote access)
Dùng sẵn dịch vụ remote access có sẵn trên windows server để triển khai, còn bên máy client thì thêm mạng ảo vào connect manage với giao thức tạo đường hầm mặc định là PPTP. Kiểm tra, đánh giá an toàn các kết nối VPN bằng wireshark. 
<img width="908" height="157" alt="image" src="https://github.com/user-attachments/assets/b764e84e-41f8-4a81-8702-c118d9cc5fc7" />

<img width="922" height="597" alt="image" src="https://github.com/user-attachments/assets/b13e1d0d-4637-4907-abd3-915a7dc7e4fa" />

Ngoài ra, có thể triển khai VPN với giao thức L2TP kết hợp IPSec
<img width="1125" height="616" alt="image" src="https://github.com/user-attachments/assets/67c84ca4-9ea5-48bf-a768-07f6279d6e44" />

<img width="1095" height="757" alt="image" src="https://github.com/user-attachments/assets/e582a20e-6c15-44ff-b7d1-84826befbc2d" />

## Triển khai Honeypot sử dụng Honeydrive
* Honeypot là một hệ thống tài nguyên thông tin được thiết kế giả lập như một mục tiêu thật (như máy chủ, cơ sở dữ liệu, thiết bị mạng) nhưng thực chất là một "cạm bẫy", cố tình để lộ các lỗ hổng bảo mật nhằm dụ dỗ kẻ tấn công mạng xâm nhập vào. Mục đích để đánh lạc hướng kẻ tấn công, giám sát và thu thập hành vi của chúng phục vụ việc phân tích và chống tấn công, nhanh chóng phát hiện các tấn công để ngăn chặn sớm. 
* Trong đó Honeydrive là một hệ điều hành Linux (dạng Appliance dựa trên Xubuntu) được cấu hình sẵn hàng loạt công cụ Honeypot phổ biến, chuyên dùng làm "bẫy" để thu thập, giám sát và phân tích các hành vi tấn công mạng. Hỗ trợ quản lý thông qua giao diện web, tạo các thống kê và cảnh báo khi bị tấn công.
<img width="1001" height="351" alt="image" src="https://github.com/user-attachments/assets/41907249-38f0-4049-b39a-9fb5142ffce9" />

<img width="1125" height="633" alt="image" src="https://github.com/user-attachments/assets/b301e0e7-d249-4266-9e4c-60993e294cc1" />

* Mô hình triển khai
<img width="1125" height="472" alt="image" src="https://github.com/user-attachments/assets/0e9de863-490b-4909-906b-d6bb2125ea48" />

* Thử nghiệm tấn công trên máy kali, kết quả thống kê của Honeydrive như dưới, ngoài ra câu lệnh kẻ tấn công đã chạy trên hệ thống cũng được ghi nhận lại. 
<img width="1125" height="603" alt="image" src="https://github.com/user-attachments/assets/797f48c0-7986-467c-9fd7-f62868e987d4" />

## Kết luận










