# BÀI 4: NÂNG CAO BẢO MẬT ĐĂNG NHẬP BẰNG MFA

## 1. Bảng so sánh SMS OTP và TOTP

| Tiêu chí       | SMS OTP                           | TOTP (Google Authenticator)            |
| -------------- | --------------------------------- | -------------------------------------- |
| Chi phí        | Tốn phí gửi SMS.                  | Miễn phí sử dụng.                      |
| Độ bảo mật     | Dễ bị tấn công SIM Swapping.      | An toàn hơn, không phụ thuộc SIM.      |
| Tính tiện dụng | Dễ sử dụng, nhận mã qua tin nhắn. | Cần cài ứng dụng và thiết lập ban đầu. |
| Offline        | Cần sóng di động để nhận mã.      | Tạo mã không cần Internet.             |

## 2. Lựa chọn giải pháp

Chọn TOTP (Google Authenticator).

Lý do:

- Chống SIM Swapping tốt hơn SMS OTP vì mã không được gửi qua số điện thoại.
- Hoạt động offline, không cần Internet hoặc sóng di động.
- Không mất phí gửi tin nhắn, giúp tiết kiệm chi phí.
- Mã xác thực thay đổi sau mỗi 30 giây, hạn chế việc sử dụng lại mã cũ.

## 3. Kết luận

Lập trình viên nên ưu tiên Authenticator App sử dụng TOTP để tăng cường bảo mật đăng nhập, giảm nguy cơ bị chiếm đoạt tài khoản và tiết kiệm chi phí cho dự án Fintech.