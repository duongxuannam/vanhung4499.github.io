---
layout: article
titles:
  en      : &EN       Build PC
  vi      : &VI       Build PC
  en-GB   : *EN
  en-US   : *EN
  en-CA   : *EN
  en-AU   : *EN
key: page-build-pc
---
__Bài viết này sẽ hướng dẫn các bạn chọn mua linh kiện để ráp một bộ PC hackintosh tương thích tốt nhất.__

## Khung sườn chung

__Để build một bộ PC Hakcintosh tương thích tốt thì bạn chỉ cần dựa theo công thức sau:__

+ Main __Gigabyte__ hoặc __ASRock__
+ Cpu __Intel__
+ Card rời __AMD__

Các thành phần còn lại thì là tuỳ chọn, bạn thích chọn loại nào chọn. Nói chung build càng giống cái máy IMAC thì càng tốt.

## CPU

+ Ưu tiên chọn CPU Intel socket 1151 core i3, i5, i7, i9 đầu 6/7/8/9
+ Nếu bạn xác định không dùng card rời thì phải chọn cpu core i có card onboard sẵn, tránh mấy cái cpu đuôi F như i3-9100F, i5-9400F và cpu pentium, celeron có card onboard nhưng không sử dụng được trong mac
+ Không nên mua các loại cpu socket 1150, 1155 đầu 2/3/4 hoặc cũ hơn nữa vì trong các bản macOS mới đã dần ngưng hỗ trợ các cpu cũ, cụ thể mojave 10.14 đã ngưng hỗ trợ cpu sandy bridge đầu 2, cứ tịnh tiến dần bản catalina 10.15 ngưng hỗ trợ cpu ivy bridge đầu 3 và tiếp tục.
+ Chỉ mua CPU Xeon nếu bạn muốn tự thử thách bản thân, khó cài
+ Tránh mua cpu __AMD__ nếu bạn cần chơi hackintosh ổn định. Hiện tại thì cpu AMD có thể cài được nhưng vẫn còn nhiều lỗi không thể sửa được. Nếu bạn cần tìm hiểu thêm thì vào [amd-osx](https://amd-osx.com/) đọc. Mình sẽ viết hướng dẫn sau.

## Mainboard

+ Ưu tiên mua main __Gigabyte__ 
+ Các main hãng Gigabyte, ASRock, ASUS, MSI đều có thể cài hackintosh nhưng nên chọn loại main ít gây lỗi nhất là Gigabyte và tốt nhất nên tránh main MSI ra
+ Nếu bạn xác định không dùng card rời thì nên chọn main có cổng Displayport. Cổng HDMI và DVI thường sẽ không xuất được hình ra bị hiện tượng đen màn, có thể giải quyết bằng cách patch framebuffer nhưng không dễ làm. VGA thì hên xui lúc xuất được lúc không, nên tránh.
+ Không nên mua các loại main socket 1150, 1155 như H61/B75/H81/B85/Z97 hoặc cũ hơn, lí do như phía trên
+ Chỉ mua main dòng X nếu muốn tự thử thách bản thân bao gồm X99/X299/X399
+ Cũng như phía trên không nên mua main dành cho cpu AMD

## GPU Rời

+ __Đây là thành phần được quan tâm nhiều nhất đối với một bộ PC Hackintosh__
+ Ưu tiên chọn card rời __AMD__ để chạy native với macOS, cụ thể danh sách như sau:
  - Vega 20 series: Radeon VII (Là trùm cuối, ở Việt Nam gần như không thấy)
  - Vega 10 series: Vega 64 Liquid, Vega 64, Vega 56, Vega Frontier Edition, Radeon Pro WX 9100, Radeon Pro WX 7100
  - Radeon 400/500 series (Polaris): (Đa số card cũ trên thị trường toàn là trâu cày, chọn mua cẩn thận)
    - 400 series: RX 480, RX 470D, RX 470, RX 460
    - 500 series: RX 590, RX 580X, RX 580 __(Tránh mua bản 2048SP)__, RX 570X, RX 570, RX 560X, RX 560, WX 5100, WX 4100, WX 3100, WX 2100
  - Các loại card __AMD__ cũ hơn không nên mua nữa
+ Nếu mua card __NVIDIA__ thì chọn dòng lõi Kelper để chạy native macOS, mấy con này khá cũ rồi nên giá cũng rẻ, cụ thể

## SSD



##Wifi/Bluetooth (tuỳ chọn)



