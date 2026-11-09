# Lỗi Git: `FETCH_HEAD` Permission denied

## Prompt 3 thành phần

**Vai trò:** Bạn là trợ giảng tin học.  
**Bối cảnh:** Tôi đẩy code lên GitHub thì gặp `error: open(".git/FETCH_HEAD"): Permission denied`, chạy lại vẫn lỗi.  
**Yêu cầu:** Giải thích thật dễ hiểu và hướng dẫn cách xử lý an toàn.

**Giải thích:** Git không được phép mở tệp `FETCH_HEAD` trong thư mục nội bộ `.git`—giống như cần mở một ngăn hồ sơ nhưng bị khóa. Có thể do quyền truy cập hoặc tệp đang được chương trình khác sử dụng.

## Thử quyền quản trị viên

Mở Windows Terminal bằng **Run as administrator**, vào đúng thư mục dự án rồi chạy lại lệnh Git một lần. Nếu vẫn lỗi, dừng lại và nhờ giảng viên/IT kiểm tra; đừng tự xóa tệp hay thay đổi quyền hàng loạt.

## Ảnh minh họa

Chụp Terminal có dòng lỗi và kết quả thử lại bằng Snipping Tool (`Win + Shift + S`). Che tên tài khoản, đường dẫn riêng tư, email, token và mật khẩu. Không có môi trường Git thực tế ở đây nên cần tự chụp ảnh sau khi thử; không dùng ảnh dựng làm bằng chứng.

## Tin nhắn báo lỗi

**Tiêu đề:** Không đẩy được code — lỗi quyền truy cập Git

Chào thầy/cô, khi đẩy code lên GitHub em gặp lỗi `error: open(".git/FETCH_HEAD"): Permission denied`.  
**Các bước:** Mở Terminal tại dự án → chạy `[lệnh Git]` → lỗi xuất hiện. Em đã thử chạy lại và `[kết quả khi Run as administrator]`.

**Mong đợi:** Đẩy code thành công.  
**Thực tế:** Git không mở được `FETCH_HEAD`.  
**Môi trường:** Windows [phiên bản], Git [phiên bản].  
Em gửi kèm ảnh đã che thông tin cá nhân. Nhờ thầy/cô hướng dẫn kiểm tra quyền truy cập an toàn ạ.
