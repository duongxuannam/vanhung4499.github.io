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
__Bài viết này sẽ hướng dẫn cơ bản các bạn chọn mua linh kiện để ráp một bộ PC hackintosh tương thích tốt nhất.__

## Khung sườn chung

__Để build một bộ PC Hakcintosh tương thích tốt thì bạn chỉ cần dựa theo công thức sau:__

+ Main __Gigabyte__ hoặc __ASRock__
+ Cpu __Intel__
+ Card rời __AMD__

Các thành phần còn lại thì là tuỳ chọn, bạn thích chọn loại nào chọn. Nói chung build càng giống cái máy IMAC thì càng tốt. Trong bài viết này mình ưu tiên những linh kiện đời mới hơn

## CPU

+ Ưu tiên chọn CPU Intel socket 1151 core i3, i5, i7, i9 đầu 6/7/8/9
+ Nếu bạn xác định không dùng card rời thì phải chọn cpu core i có card onboard sẵn, tránh mấy cái cpu đuôi F như i3-9100F, i5-9400F và cpu pentium, celeron có card onboard nhưng không sử dụng được trong mac
+ Không nên mua các loại cpu socket 1150, 1155 đầu 2/3/4 hoặc cũ hơn nữa vì trong các bản macOS mới đã dần ngưng hỗ trợ các cpu cũ, cụ thể mojave 10.14 đã ngưng hỗ trợ cpu sandy bridge đầu 2, cứ tịnh tiến dần bản catalina 10.15 ngưng hỗ trợ cpu ivy bridge đầu 3 và tiếp tục.
+ Chỉ mua CPU Xeon nếu bạn muốn tự thử thách bản thân, khó cài
+ Tránh mua cpu __AMD__ nếu bạn cần chơi hackintosh ổn định. Hiện tại thì cpu AMD có thể cài được nhưng vẫn còn nhiều lỗi không thể sửa được. Nếu bạn cần tìm hiểu thêm thì vào [amd-osx](https://amd-osx.com/) đọc. Mình sẽ viết hướng dẫn sau.

## Mainboard

+ Ưu tiên mua main __Gigabyte__ 
+ Các main hãng Gigabyte, ASRock, ASUS, MSI (xếp theo thứ độ ổn) đều có thể cài hackintosh nhưng nên chọn loại main ít gây lỗi nhất là Gigabyte và tốt nhất nên tránh main MSI ra
+ Nếu bạn xác định không dùng card rời thì nên chọn main có cổng Displayport. Cổng HDMI và DVI thường sẽ không xuất được hình ra bị hiện tượng đen màn, có thể giải quyết bằng cách patch framebuffer nhưng không dễ làm. VGA thì hên xui lúc xuất được lúc không, nên tránh.
+ Không nên mua các loại main socket 1150, 1155 như H61/B75/H81/B85/Z97 hoặc cũ hơn, lí do như phía trên
+ Chỉ mua main dòng X nếu muốn tự thử thách bản thân bao gồm X99/X299/X399
+ Cũng như phía trên không nên mua main dành cho cpu AMD

## GPU Rời

+ __Đây là thành phần được quan tâm nhiều nhất đối với một bộ PC Hackintosh__
+ Ưu tiên chọn card rời __AMD__ để chạy native với macOS, cụ thể danh sách như sau:
  - Vega 20 series: Radeon VII (Là trùm cuối, ở Việt Nam gần như không thấy)
  - Vega 10 series: Vega 64, Vega 56 (Cũng khá ít chỗ bán)
  - Radeon 400/500 series (Polaris): (Đa số card cũ trên thị trường là trâu cày, chọn mua cẩn thận)
    - 400 series: RX 480, RX 470, RX 460
    - 500 series: RX 590, RX 580X, RX 580 __(Tránh mua bản 2048SP)__
  - Các loại card __AMD__ cũ hơn không nên mua nữa
  - Card RX 5700 và RX 5700XT hiện tại chưa được hỗ trợ, trong tương lai khả năng cao được hỗ trợ.
  - __Không nên mua__ card từ các hãng: __XFX__, __HIS__. Do các card hay dính lỗi về vbios, cần phải được phải flash lại, mình cũng không biết làm.
+ Không nên mua card __NVIDIA__ để chơi hackintosh, nếu ít tiền thì mua card lõi Kelper giá rẻ để chạy native macOS, cụ thể:  GTX 650(GK 107 core), GT 640(GK 107/208 core), GT 630(GK 107/208 core), GT 740, GT 730(GK208 core), GT 720, GT 710

## SSD

+ Ưu tiên mua ổ SSD SAMSUNG: SATA 860 EVO, NVME 970 EVO/EVO PLUS/PRO, PM961, ... __tránh PM981__
+ Gần như tất cả các loại ổ cứng SATA hay NVME đều có thể cài được macOS, nhưng nếu đã mua thì mua loại cho tốt luôn để dùng lâu dài, hãng mình thấy ổn: SAMSUNG, CRUCIAL
+ SSD SAMSUNG PM981 không dùng được trong macOS, tính cả real mac luôn, sẽ gây hiện tượng giật khựng máy
+ SSD 970 EVO PLUS phải được update firmware nếu không cũng giống như PM981
+ Không nên mua SSD Intel để cài hackintosh

## Wifi/Bluetooth (tuỳ chọn)

+ Nếu cần wifi, bluetooth, airdrop, handoff thì nên mua còn nếu chỉ cần wifi không thì có thể dùng usb wifi, còn không cần luôn thì cứ LAN mà dùng.
+ Nếu main có sẵn khe M2.WIFI thì có thể mua card BCM94352Z = DW1560 hoặc BCM943602 = DW1830 và lắp đặt hoặc thay thế vào.
+ Nếu main không có khe M2.WIFI thì chỉ có cách mua card wifi kèm adapter chuyển sang PCIE, cụ thể:
  - BCM94331CSAX: 3 râu, chuẩn N, tốc độ lý thuyết tối đa 450 Mbps
  + BCM9460CS2: 2 râu, chuẩn AC, tốc độ lý thuyết tối đa 1200 Mpbs
  + BCM94602CS: 3 râu, chuẩn AC, tốc độ lý thuyết tối đa 1750 Mbps

## Tổng kết

Build PC Hackintosh bạn chỉ cần quan tâm tới những linh kiện trên. Mình cũng chưa có quá nhiều kinh nghiệm về build PC chỉ biết cài hackintosh là nhiều thôi. Các vấn đề về các linh kiện khác cần tham khảo thêm bên bán máy hoặc những người có kinh nghiệm hơn.

__Bạn nào build pc xong rồi mà chưa biết cài hackintosh nữa thì hãy đọc các bài viết trong blog này. Nếu không làm được nữa thì mình có cài [dịch vụ Hackintosh](/service), các tham khảo rồi [liên hệ](contact).__