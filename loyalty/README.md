# Nifnail Studio Loyalty (PWA)

Ứng dụng web cài lên Màn hình chính iPhone, dùng cho nhân viên quản lý khách và tích điểm. Không cần Xcode, IPA hay dịch vụ build cloud.

## Tính năng hiện có
- Tổng quan: số khách, điểm tích hôm nay, tổng điểm đang lưu, lượt dịch vụ.
- Thêm khách, kiểm tra trùng số điện thoại, tìm theo tên / số điện thoại.
- Hồ sơ thành viên, số dư điểm và lịch sử riêng.
- Tích +1 điểm sau xác nhận hoàn thành dịch vụ.
- Đổi điểm từ 6 điểm trở lên; 1 điểm = 1% giảm giá.
- Tự tính số tiền giảm, khách thanh toán, số điểm còn lại.
- Lịch sử giao dịch, xuất và nhập JSON để sao lưu / khôi phục.
- Giao diện đen – vàng champagne, responsive cho iPhone.

## Quy tắc đổi điểm
- Khách phải có trên 5 điểm.
- Mỗi lần đổi phải dùng tối thiểu 6 điểm và không vượt số dư.
- Giới hạn 100 điểm cho một hóa đơn để mức giảm không vượt 100%.
- Điểm bị trừ sau khi nhân viên xác nhận giao dịch.

## Dữ liệu và quyền riêng tư
MVP lưu dữ liệu trong localStorage của trình duyệt trên thiết bị. Không có tài khoản, máy chủ hay đồng bộ giữa các iPhone. Không xóa dữ liệu Safari nếu chưa xuất JSON backup. Nhập JSON sẽ thay thế dữ liệu hiện có.

## Cài trên iPhone
1. Đưa thư mục `loyalty` lên GitHub Pages (sau khi merge branch vào nhánh được Pages publish).
2. Mở URL kết thúc bằng `/loyalty/` bằng Safari trên iPhone.
3. Chọn Chia sẻ → Thêm vào Màn hình chính → Thêm.
4. Mở biểu tượng Nifnail từ Màn hình chính.

## Lưu ý trước khi dùng chính thức
Bản MVP chưa có đăng nhập / phân quyền nhân viên, đồng bộ nhiều thiết bị, nhật ký kiểm toán chống sửa dữ liệu hoặc sao lưu tự động. Vì vậy chỉ nên thử nghiệm nội bộ, xuất backup định kỳ và không dùng dữ liệu khách thật nhạy cảm cho đến khi hoàn thiện bảo mật.
