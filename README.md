# Cài Windows cho Linux
File sh hỗ trợ cài windows từ file gz cho mọi loại Linux chạy trực tiếp ( không cần qua Recovery )

Cách sử dụng:

- Trước tiên cần có sẵn 1 VPS Linux và 1 file GZ của windows ( nếu chưa có thể tự làm thông qua lab này : https://katacoda.com/embed/as247/winimagebuilder)
- Lệnh chạy:


sudo wget --no-check-certificate -qO InstallNET.sh 'https://raw.githubusercontent.com/kmille36/CaiWindowsChoLinux/main/InstallNET.sh' && bash InstallNET.sh -dd 'https://yourdirectdownloadlinkhere.gz'

Nhớ thay https://yourdirectdownloadlinkhere.gz bằng link tải file gz của bạn ( thường là up ở dropbox )

*Script này hỗ trợ cả MBR và UEFI.



