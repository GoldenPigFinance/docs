# Hướng dẫn sử dụng HeoVang
## Quy trình tạo ví thanh toán


Khi người dùng có tài khoản đăng nhập trên website **Heo Vàng CMS**	thì cũng có thể đăng nhập trên app **Heo Vàng**.


1. Quy trình tạo ví thanh toán:

B1: Chủ thương hiệu đăng nhập tài khoản và mật khẩu được cấp tại website Heovang Merchant: [https://business.heovang.vn/#login](https://business.heovang.vn/#login)

 ![Màn hình Đăng nhập](/images/admin/login.png)

B2: Ví thanh toán
- Tại màn hình trang chủ, chủ thương hiệu chọn **Quản lý tài khoản** > **Ví thanh toán**
- Ở màn hình **Danh sách ví thanh toán**, chủ thương hiệu chọn **Tạo ví**.

![Màn hình Danh sách ví thanh toán](/images/admin/dsvtt.png)

B3: Tạo mới ví thanh toán
- Khi chủ thương hiệu chọn **Tạo ví**, màn hình tạo ví mới sẽ hiển thị ra, chủ thương hiệu nhập các thông tin cần thiết.
- Sau khi chủ thương hiệu nhập đầy đủ thông tin, chủ thương hiệu chọn **Lưu**.
> Ghi chú: Chủ thương hiệu có thể tải file excel để tạo ví thanh toán 1 cách nhanh chóng.


![Màn hình tạo mới ví thanh toán](/images/admin/tmvtt.png)

## Tạo ví thanh toán hàng loạt bằng Excel

Chức năng này phù hợp khi cần tạo nhiều ví thanh toán cho khách hàng trong cùng một lần thao tác.

### Bước 1: Vào danh sách Ví thanh toán

Từ trang chủ HeoVang Merchant, chọn **Quản lý tài khoản** > **Ví thanh toán**.

Tại màn hình **Danh sách Ví Thanh Toán**, chọn nút **Import**.

### Bước 2: Tải file Excel mẫu

Tại màn hình **Nhập danh sách Ví thanh toán**, chọn **Tải file mẫu** để tải biểu mẫu Excel về máy.

Bạn cũng có thể tải biểu mẫu tại đây: [Tải file Excel mẫu](https://raw.githubusercontent.com/GoldenPigFinance/docs/main/assets/templates/HEOVANG_CREATE_ACCOUNT.xlsx).

### Bước 3: Chuẩn bị dữ liệu trong file Excel

Không thay đổi tên các cột trong file mẫu. Mỗi dòng dữ liệu tương ứng với một ví thanh toán cần tạo hoặc cập nhật.

| Cột | Nội dung | Lưu ý |
| --- | --- | --- |
| `STT` | Số thứ tự dòng | Dùng để dễ đối chiếu kết quả import; có thể để trống. |
| `TÊN KHÁCH HÀNG` | Tên hiển thị của ví thanh toán | Nên điền đầy đủ để nhận diện ví. |
| `EMAIL` | Email của người dùng liên kết với ví | Điền khi cần tạo hoặc liên kết tài khoản người dùng. |
| `MÃ NỘI BỘ` | Mã định danh ví trong doanh nghiệp | Bắt buộc. Mỗi mã phải là duy nhất trong doanh nghiệp. |
| `Mật khẩu` | Mật khẩu của tài khoản người dùng mới | Dùng khi tạo user mới. Nếu để trống, hệ thống có thể dùng mật khẩu mặc định. |
| `NHÓM KHÁCH HÀNG` | Mã nhóm khách hàng của ví | Không bắt buộc. Mã nhóm cần được tạo trước trên hệ thống. |

> **Lưu ý:** không thêm cột hoặc đổi tên cột nếu chưa được hướng dẫn. Giữ nguyên định dạng Excel `.xlsx` hoặc `.xls`.

### Bước 4: Chọn file và tạo danh sách import

1. Chọn **Choose File**.
2. Chọn file Excel đã chuẩn bị.
3. Nếu cần tạo tài khoản người dùng cùng với ví, chọn **Tạo mới User**.
4. Hệ thống hiển thị thông báo đang xử lý danh sách và chuyển đến màn hình xem trước dữ liệu import.

Chỉ tải file có dung lượng không quá 1 MB.

### Bước 5: Kiểm tra và xác nhận dữ liệu

Tại màn hình xem trước, kiểm tra các thông tin như mã nội bộ, tên ví, nhóm khách hàng, email và trạng thái tạo user.

Nếu thông tin đúng, chọn **Xác nhận** để hệ thống tạo hoặc cập nhật các ví trong danh sách.

Sau khi hoàn tất, quay lại **Danh sách Ví Thanh Toán** để kiểm tra các ví vừa import.

### Lưu ý khi import

- Không dùng lại `MÃ NỘI BỘ` của một ví khác trong cùng doanh nghiệp.
- Nếu `NHÓM KHÁCH HÀNG` chưa tồn tại, ví có thể được tạo nhưng chưa được gán nhóm.
- Nếu dữ liệu trong file không đúng định dạng, hãy sửa file Excel và thực hiện import lại.
- Nên thử import một vài dòng dữ liệu trước khi import danh sách lớn.

### Video hướng dẫn

<video controls preload="metadata" style="width: 100%; max-width: 900px;">
  <source src="https://raw.githubusercontent.com/GoldenPigFinance/docs/main/assets/videos/huong-dan-tao-vi-thanh-toan-hang-loat.mp4" type="video/mp4">
  Trình duyệt của bạn không hỗ trợ phát video. Bạn có thể <a href="https://raw.githubusercontent.com/GoldenPigFinance/docs/main/assets/videos/huong-dan-tao-vi-thanh-toan-hang-loat.mp4">tải video hướng dẫn</a> để xem.
</video>
