# RoTik — Chính sách riêng tư / Privacy Policy

_Cập nhật / Updated: 2026-11-20_

## Tiếng Việt

RoTik là app quản lý router tại nhà. App **không thu thập, không gửi và không bán** dữ liệu cá nhân nào cho nhà phát triển hay bên thứ ba. App không có tài khoản người dùng phía nhà phát triển, không có máy chủ riêng, không có quảng cáo, không có công cụ theo dõi hay phân tích. Dữ liệu chỉ nằm trên điện thoại của bạn, trên router của bạn, hoặc đi tới bot do chính bạn tạo (xem bên dưới).

- **Kết nối tới router:** app chỉ kết nối tới router do bạn nhập, trong mạng nhà hoặc qua tên DDNS của router, bằng HTTPS.
- **Đường riêng (khi bạn bật):** nếu router không vào được từ ngoài, bạn có thể bật "đường riêng" khi đang ở nhà. App gửi gói UDP mã hoá chỉ tới chính router của bạn, không qua máy chủ nào của nhà phát triển. Khoá riêng của điện thoại được sinh trên điện thoại và chỉ nằm trong Keychain / Keystore; router chỉ giữ khoá công khai. Đây không phải VPN hệ thống: app không cài hồ sơ VPN và không chuyển lưu lượng nào khác của điện thoại.
- **Lần đầu vào router (SSH):** với router mới còn cấu hình nhà máy, app có thể chạy một vài lệnh cố định qua SSH, bằng tài khoản quản trị bạn gõ một lần. Tài khoản và mật khẩu đó chỉ dùng cho lần kết nối ấy, đi thẳng tới router của bạn, và app không lưu lại. App chỉ ghi nhớ dấu vân tay khoá SSH của router để cảnh báo nếu nó đổi.
- **Bot Telegram và Zalo (khi bạn bật):** điện thoại gọi API bot của Telegram hoặc Zalo để kiểm token bot và ghép chat. Token và mã chat chỉ được lưu trên router của bạn; chính router gửi thông báo tới bot của bạn (app tắt vẫn nhận), và nhận lệnh của bạn qua bot đó. Tên người nhận thêm chỉ nằm trên điện thoại. Nhà phát triển không có bot, không thấy token và không thấy tin nhắn. Telegram và Zalo có chính sách riêng đối với nội dung đi qua dịch vụ của họ.
- **Tài khoản người nhà (khi chủ router dùng):** chủ router tạo cho mỗi điện thoại người nhà một tài khoản trên chính router của chủ. Lời mời là một liên kết hoặc mã QR chứa mật khẩu tạm dùng một lần; điện thoại của chủ không lưu mật khẩu đó. Chủ tự gửi liên kết (ví dụ qua Zalo), nên chỉ gửi cho người bạn tin; tin nhắn ấy đi qua dịch vụ nhắn tin bạn chọn, không qua nhà phát triển. Máy người nhà dùng mật khẩu tạm để vào rồi tự đổi mật khẩu. Tài khoản nằm trên router của chủ, không ở nhà phát triển, và chủ thu hồi được bất cứ lúc nào trong Cài đặt → Tài khoản người nhà.
- **Lưu trên điện thoại:** địa chỉ router, tên đăng nhập và mật khẩu router được lưu trong kho bảo mật của hệ điều hành (Keychain / Keystore) trên điện thoại. Tên thiết bị, cảnh báo và cài đặt app cũng chỉ lưu trên điện thoại.
- **Thay đổi trên router:** mọi thay đổi app thực hiện (chặn mạng, lịch Internet, đặt tên thiết bị, cập nhật RouterOS…) được ghi trên router của bạn và chỉ khi bạn yêu cầu.
- **Kiểm tra bản mới:** chỉ trên Android, app tải tệp `latest.json` công khai từ GitHub để biết có bản mới; yêu cầu này không chứa thông tin của bạn. Bản iPhone chỉ phát hành qua App Store và không dùng việc này (App Store tự cập nhật).
- **Xoá dữ liệu:** xoá router trong app hoặc gỡ app sẽ xoá dữ liệu lưu trên điện thoại. Dữ liệu trên router (tài khoản người nhà, tệp bot…) do bạn quản lý trên router; app có chức năng gỡ.

Liên hệ: tuanlong.sav@gmail.com

## English

RoTik manages a home router. The app **does not collect, transmit or sell** any personal data to the developer or third parties. There are no developer-side user accounts, no server of our own, no ads, trackers or analytics. Data stays on your phone, on your router, or goes to a bot that you created yourself (see below).

- **Connections to your router:** the app only connects, over HTTPS, to the router address you enter (on your home network or via the router's DDNS name).
- **Private path (when you switch it on):** if the router cannot be reached from outside, you can switch on a "private path" while at home. The app sends encrypted UDP packets only to your own router, never through a server of the developer. The phone's private key is generated on the phone and kept only in the Keychain / Keystore; the router keeps only the public key. This is not a system VPN: the app installs no VPN profile and carries no other traffic of the phone.
- **First-time setup over SSH:** for a new router still in its factory configuration, the app can run a few fixed commands over SSH using the admin account you type once. That user name and password are used only for that connection, go straight to your router, and are not stored by the app. The app only remembers the router's SSH host-key fingerprint, to warn you if it changes.
- **Telegram and Zalo bots (when you switch them on):** the phone calls the Telegram or Zalo bot API to check the bot token and pair your chat. The token and chat id are stored only on your router; the router itself sends notifications to your bot (they arrive even when the app is closed) and receives your commands through it. Names of extra recipients stay on the phone. The developer has no bot and sees neither the token nor the messages. Telegram and Zalo have their own policies for what passes through their services.
- **Family accounts (when the router owner uses them):** the owner creates, for each family member's phone, an account on the owner's own router. The invite is a link or QR code that holds a one-time temporary password; the owner's phone does not keep that password. The owner sends the link themself (for example through Zalo), so send it only to people you trust; that message travels through the messaging service you choose, not through the developer. The family member's phone uses the temporary password to sign in and then changes it. The account lives on the owner's router, not with the developer, and the owner can revoke it at any time in Settings → Family accounts.
- **On your phone:** the router address, user name and password are kept in the operating system's secure storage (Keychain / Keystore) on your phone. Device names, alerts and app settings also stay on the phone.
- **Changes on the router:** any change the app makes (blocking, Internet schedules, device names, RouterOS updates…) is written to your router, only when you ask for it.
- **Update check:** on Android only, the app downloads a public `latest.json` file from GitHub to learn about new builds; the request carries no information about you. The iPhone build is distributed only through the App Store and does not do this (the App Store updates the app).
- **Deleting data:** removing a router in the app or deleting the app removes the data stored on the phone. Data on the router (family accounts, bot files…) is under your control on the router; the app can remove it.

Contact: tuanlong.sav@gmail.com
