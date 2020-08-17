Những thứ cần thiết để tạo bộ cài Hackintosh trên macOS và Windows.

### Tạo bộ cài Hackintosh trên macOS
- Hackintosh Files: https://bit.ly/2PZpHkS
# Các phiên bản này down trực tiếp bằng App Store, chọn phiên bản nào là tuỳ lựa chọn của bạn
- macOS Catalina: https://apple.co/3iJOWE0
- macOS Mojave: https://apple.co/3iKyF1x
- macOS High Sierra: https://apple.co/3407Hiq
- macOS Sierra: https://apple.co/3iMkyZy
### Tạo bộ cài Hackintosh trên Windows
Lưu ý: Bộ cài khi giải nén ra sẽ có định dạng .raw, các bạn hãy sử dụng Etcher hoặc Win32DiskImager để ghi bộ cài ra USB
- macOS Catalina: https://bit.ly/3iOyaU2
- macOS Mojave: https://bit.ly/3iL8esv
- macOS High Sierra: https://bit.ly/31WKdIb
- macOS Sierra: https://bit.ly/3kRtWwQ
### Công cụ
# Đối với macOS:
- Etcher (chỉ sử dụng khi các bạn sử dụng bộ cài cho Windows trên macOS): bit.ly/3iOFEH0
# Đối với Windows:
- Etcher: https://bit.ly/3iOFEH0
- MiniTool Partition Wizard: https://bit.ly/3kJicfQ
- Explorer++: https://bit.ly/3h2bKy9
### Bootloader (Clover & OpenCore)
Nếu như các bạn tạo bộ cài trên Windows thì Clover đã được tích hợp sẵn vào USB, các bạn chỉ việc boot vào và cài đặt. Còn nếu như các bạn tạo bộ cài trên macOS thì hãy sử dụng Clover làm bootloader (vì OpenCore vẫn đang trong quá trình thử nghiệm và có thể gây lỗi bất cứ lúc nào).

- Clover Bootloader EFI: https://bit.ly/346KP0S
- OpenCore Bootloader: https://bit.ly/2Y66nGN
### Kexts
* Lưu ý: Trong bộ cài dành cho việc tạo USB trên Windows, tất cả các kext đều đã được tích hợp sẵn, các bạn không cần phải điều chỉnh gì cả.
* Đối với bộ cài trên macOS, bạn sẽ phải tích hợp kext thủ công
# Các kext tối quan trọng trên Hackintosh:
- FakeSMC: Nhằm giả lập hệ thống cảm biến giống như các máy Mac. https://bit.ly/3g3yk8k
- USBInjectAll: Nhằm fix lỗi các cổng USB trên máy. https://bit.ly/2FuVwzX
- Lilu: Giúp patch vá mềm on-the-fly cho các phần cứng mà không cần phải chỉnh sửa quá nhiều. https://bit.ly/2PUm53x
- WhateverGreen.kext: Giúp giải quyết các vấn đề của iGPU và dGPU: https://bit.ly/3109Bxo
# Các kext có thể phải thêm tuỳ thuộc vào phần cứng:
- AppleIntelE1000e: Kext card LAN cho các card Intel đời cũ. https://bit.ly/3h0AYNu
- IntelMausiEthernet: Kext card LAN cho các card LAN Intel: https://bit.ly/3kQw3RG
VoodooPS2Controller: Kext cho bàn phím và bàn rê chuột PS2 trên Laptop. https://bit.ly/3kSLCbk
- RealtekRTL8100: Kext cho card LAN Realtek. https://bit.ly/2DYSaEL
- RealtekRTL8111: Kext cho card LAN Realtek. https://bit.ly/3h2XUfa
- AtherosE2200Ethernet: Kext cho card LAN Atheros. https://bit.ly/311WyvK
- FakePCIID: Giúp fake thông tin những phần cứng không được hỗ trợ thành những phần cứng được Apple hỗ trợ. https://bit.ly/3iN5VFy
- GenericUSBXHCI: Fix cổng USB Controller 3.0 với các máy có cổng USB 3.0. Có thể dùng kèm USBInjectAll. https://bit.ly/30YJY0a
- AHCIPortInjector: Thêm các thông tin về ổ cứng để cho macOS có thể nhận ra. Nếu không thấy ổ cứng khi cài thì hãy dùng kext này. https://bit.ly/312yUix
- NullCPUPowerManagement: Dùng để kích hoạt processor power management trên các dòng CPU Pentium, chẳng hạn như G4560. https://bit.ly/2PTGN3o
# Hoàn thiện Hackintosh sau khi đã cài xong
- AppleALC: Nhằm kích hoạt âm thanh trong Hackintosh. https://bit.ly/340e1GG
- ACPIBatteryManager: Nhằm hiển thị phần trăm pin trên Laptop. https://bit.ly/30Z3x8s
- NightShiftUnlocker: Kích hoạt tính năng Night Shift trên các card màn hình cũ. https://bit.ly/34hVlT5
- CodecCommander: Fix lỗi mất âm thanh sau khi wake và lỗi tai nghe bị rè trên Laptop. https://bit.ly/3awMldu
- HibernationFixup: Fix lỗi hibernate trong Hackintosh. https://bit.ly/3217dpL
- EnableLidWake: Fix lỗi wake sau khi gập màn hình của laptop. https://bit.ly/2PWqJxT

Cảm ơn Olarila, Rehabman, InsanelyMac, Slice.... đã đóng góp cho Hackintosh. Nếu như có bất kỳ thắc mắc gì, có thể liên hệ với mình qua facebook cá nhân (https://www.facebook.com/onedotonedotonedotone)
                                                  Copyright © 2020 Trần Minh Quyết

