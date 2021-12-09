# Cài Windows cho Linux
File sh hỗ trợ cài windows từ file gz cho mọi loại Linux chạy trực tiếp ( không cần qua Recovery )
- Hỗ trợ: Debian, Ubuntu, CentOS

Cách sử dụng:

- Trước tiên cần có sẵn 1 VPS Linux và 1 file GZ của windows ( nếu chưa có thể tự làm thông qua lab này : https://katacoda.com/embed/as247/winimagebuilder)
- Lệnh chạy:


sudo wget --no-check-certificate -qO InstallNET.sh 'https://raw.githubusercontent.com/kmille36/CaiWindowsChoLinux/main/InstallNET.sh' && bash InstallNET.sh -dd 'https://yourdirectdownloadlinkhere.gz'

Nhớ thay https://yourdirectdownloadlinkhere.gz bằng link tải file gz của bạn ( thường là up ở dropbox )

*Script này hỗ trợ cả MBR và UEFI.


Một số hình ảnh Demo:

- Chạy trên VPS Ubuntu tới đoạn này là đã hoàn tất chỉ cần đợi 20-30p để nó tự cài ( nếu Web VPS có hỗ trợ View Console có thể vào để xem quá trình cài đặt):
![Alt text](https://i.ibb.co/LZZ0WSy/image.png "Screenshot")
- Hình ảnh quá trình cài đặt sẽ bị đứng ở 0% như vậy là bình thường chỉ cẩn đợi khi chạy xong sẽ tự restart boot thẳng vào Windows
![Alt text](https://i.ibb.co/2Z5Jv7n/262202265-281488613935731-5683832719609328574-n.png "Screenshot")
- Sau khi đợi tầm 30p và đây là hình ảnh khi login vào VPS ở port 3389 ( nhớ phải mở port này mới connect được VPS khi cài xong)
![Alt text](https://i.ibb.co/VtZkKWF/image.png "Screenshot")


*Nguồn file sh: https://moeclub.org/
*Sửa đổi và viết hướng dẫn: https://fb.com/thuong,hai.581


