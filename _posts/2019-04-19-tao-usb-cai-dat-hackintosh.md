---
  title: Tạo usb cài đặt hackintosh
  author: Nguyen Van Hung
  tags: hackintosh usb
  toc:
---
Bạn sẽ cần macOS để thực hiện tạo usb vanilla hackintosh. Ngoài ra vẫn có cách khác để tạo usb vanilla mà không cần đến macOS nhưng mà để hiểu và ít lỗi xảy ra hãy làm theo cách này. Những cách khác mình sẽ viết sau.

## Chuẩn bị bộ cài, USB
- Bộ cài macOS gốc tải từ App Store:
  + [High Sierra 10.13.6](https://itunes.apple.com/ca/app/macos-high-sierra/id1246284741?mt=12)
  + [Mojave mới nhất](https://itunes.apple.com/us/app/macos-mojave/id1398502828?mt=12)
- Thường thì tải từ App Store rất chậm ở Việt Nam, bạn có thể tham khảo thêm một số nguồn bộ cài bên ngoài nhưng có thể gây lỗi. Mình sẽ đưa ra một nguồn mà mình hay sử dụng và cảm thấy ổn là từ [Olarila](https://olarila.com), tải về giải nén và cho vào thư mục Applications:
  + [High Sierra 10.13.6](https://drive.google.com/file/d/1h5npjpj630TTZzrRl-g69JlWtLmFxQA8/view)
  + [Mojave 10.14.3](https://drive.google.com/file/d/1aKOEm3dVFDuqmKZnQbl1Do8i5sK_5UXE/view)
  + [Mojave 10.14.4](https://drive.google.com/file/d/1eoHuYv9YxSzQEXTF4EDv7aEzt2r38o7K/view)
- Trong blog này mình sẽ chỉ hướng dẫn về cài các bản 10.13.6 và 10.14.x thôi do một số kext quan trọng ngưng support các bản cũ hơn. Hãy chắc rằng bạn đã có bộ cài trong thư mục Applications để thực hiện các bước tiếp theo.

## Format USB
  1. Cắm USB vào.Nếu bạn dùng máy ảo VMWare thì nếu usb không kết nối thì làm như sau: chọn VM ở trên thanh công cụ -> Removable Device -> chọn tên USB của bạn -> Connect.
  2. Mở app Disk Utility
  3. 
  3. Chọn USB của bạn ở cột bên trái
## Tích hợp bộ cài vào USB
