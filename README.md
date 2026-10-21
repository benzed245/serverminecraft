# MC Server Studio — Hướng dẫn cài đặt và sử dụng

Ứng dụng tạo và quản lý **server Minecraft** cho bạn và bạn bè trên Windows.
Bấm vài nút là có server: tự tải Minecraft, tự lo Java, tự cấu hình, có bảng theo dõi và địa chỉ sẵn để gửi bạn bè.

---

## 1. Máy cần gì

| | Yêu cầu |
|---|---|
| Windows | Windows 10 / 11 bản 64-bit |
| Dung lượng trống | khoảng 3 GB cho ứng dụng + mỗi server thêm 1–3 GB (thế giới, mod, plugin) |
| RAM | 8 GB trở lên (server chơi nhóm 4–6 người nên cấp 4 GB) |
| .NET / Java | **Không cần cài gì** — bộ cài đã gồm sẵn .NET, Java thì ứng dụng tự tải khi cần |
| Mạng | Cần internet cho lần tạo server đầu tiên (khoảng 1 phút) |

## 2. Cài đặt

1. Bấm đúp vào **`MC-Server-Studio-Setup-3.0.0.msi`**.
2. Windows có thể hiện cảnh báo **"Windows protected your PC"** (do file cài chưa ký số).
   Bấm **More info** → **Run anyway** để tiếp tục.
3. Bấm **Install** và chờ khoảng một phút.

Sau khi cài xong bạn sẽ có:

- Biểu tượng **MC Server Studio** ngoài Desktop và trong Start Menu.
- Ứng dụng nằm ở `%LOCALAPPDATA%\Programs\MC Server Studio` — **cài theo từng người dùng nên không cần quyền admin**
  và dữ liệu server luôn ghi được bình thường.

> Không có quyền cài đặt? Dùng bản **`MC-Server-Studio-3.0.0-portable.zip`**: giải nén ra một thư mục rồi chạy `MCStudio.exe`.

## 3. Tạo server đầu tiên (làm một lần, khoảng 1 phút)

Mở ứng dụng → tab **Tạo server**. Có 4 bước, giữ nguyên các giá trị mặc định cũng chạy tốt:

| Bước | Việc cần làm |
|---|---|
| **1 · Thông tin** | Đặt tên server, chọn phiên bản Minecraft (mới nhất là tốt nhất), chọn loại server — **Paper** là lựa chọn tốt nhất cho chơi nhóm |
| **2 · Cách chơi** | Chế độ sinh tồn, độ khó bình thường, số người tối đa, cổng để `25565`, lời chào tuỳ thích |
| **3 · Hiệu năng & tiện ích** | Cấp RAM (máy 8 GB → 4 GB, máy 16 GB → 6 GB). Tick sẵn **bộ plugin cơ bản**, **menu trong game** và **chống X-ray** nếu muốn chơi nhóm ngay |
| **4 · Kiểm tra & tạo** | Xem lại tóm tắt, tick **đồng ý EULA của Minecraft**, bấm **Tạo server** |

Ứng dụng sẽ tự tải Minecraft server và Java (nếu máy thiếu), rồi tạo xong server.
Cùng lúc đó bạn vẫn có thể tạo thêm nhiều server khác — nút chọn server nằm ở góc trên bên trái.

## 4. Bật server và mời bạn bè

1. Bấm nút xanh **Chạy server** ở góc trên bên phải (hoặc nhấn **F5**).
2. Chờ khoảng 20–40 giây cho tới khi badge đổi thành **Đang chạy**.
3. Sang tab **Điều khiển** → mục *Địa chỉ cho bạn bè*:
   - **Trong cùng nhà / cùng Wi-Fi**: bấm **Sao chép** và gửi địa chỉ đó. Bạn bè mở Minecraft → **Multiplayer** → **Add Server** → dán địa chỉ → **Join**.
   - **Bạn bè ở xa (khác mạng)**: bấm **Tự mở cổng (UPnP)** → rồi **Kiểm tra kết nối**. Nếu báo chưa vào được, xem mục *Thiết lập nâng cao* ở tab **Bạn bè & Mạng** (mở cổng thủ công, hoặc dùng playit.gg miễn phí).

**Bạn bè cần cài gì?** Gần như không cần gì: chỉ cần Minecraft gốc và đúng phiên bản.
Plugin và mod phía server (bộ cài sẵn trong ứng dụng) không cần cài ở máy bạn bè; gói tài nguyên thì Minecraft của họ tự hỏi tải khi vào server.

> ⚠️ **Cảnh báo quan trọng**: nếu máy bạn đang bật **VPN / Cloudflare WARP**, bạn bè ở ngoài internet sẽ **không vào được**. Ứng dụng sẽ hiện cảnh báo vàng — hãy tắt VPN trước khi mời bạn bè ở xa (bạn bè cùng nhà vẫn chơi bình thường).

## 5. Các tab trong ứng dụng

| Tab | Dùng để làm gì |
|---|---|
| **Tổng quan** | Xem toàn bộ server của bạn, số người đang chơi, RAM đang dùng và các gợi ý cần làm (bật chống X-ray, bật sao lưu…) |
| **Tạo server** | Tạo server mới (wizard 4 bước); cuối trang có danh sách server đã có để mở, chạy hoặc xoá |
| **Điều khiển** | Bật/tắt/khởi động lại server, xem 6 thông số trực tiếp (CPU, RAM, TPS, người chơi, thời gian chạy, dung lượng thế giới), địa chỉ cho bạn bè, danh sách người đang chơi, thao tác nhanh (lưu thế giới, sao lưu map, whitelist, cấp OP, icon server, xem lỗi gần nhất) |
| **Mod & Plugin** | 4 tab: **Khám phá** (bộ cài sẵn + tìm trên Modrinth), **Đã cài** (bật/tắt, xoá, kiểm tra cập nhật), **Menu trong game** (luật + hướng dẫn hiện cho người chơi), **Gói tài nguyên** (phát file .zip cho bạn bè tự tải) |
| **Người chơi** | 4 tab: **Trực tuyến** (cấp/thu OP, đổi chế độ, kick, ban), **Whitelist**, **Quản trị viên**, **Đã ban** |
| **Cấu hình** | 4 tab: **Chung** (MOTD, cổng, chế độ, độ khó, PvP, whitelist…), **Hiệu năng & Java** (RAM, preset, chống X-ray, đổi phiên bản, sửa Java), **Thế giới** (dung lượng, seed, icon, xoá thế giới), **Tự động hóa** (sao lưu định kỳ, tự khởi động lại) |
| **Bạn bè & Mạng** | Địa chỉ LAN, địa chỉ internet, mở cổng, kiểm tra kết nối, hướng dẫn cho bạn bè ở xa |
| **Console** | Xem log trực tiếp, gõ lệnh server, lịch sử lệnh (mũi tên ↑ ↓), lọc chỉ hiện lỗi, lưu log ra file |

**Phím tắt:** `Ctrl+1` … `Ctrl+8` chuyển nhanh giữa các tab · `F5` chạy/dừng server.

## 6. Dữ liệu nằm ở đâu, sao lưu thế nào

- Mỗi server là một thư mục riêng trong `%LOCALAPPDATA%\Programs\MC Server Studio\Data\servers\<tên server>`
  (chứa thế giới, mod, plugin, cấu hình, log).
- Nút **Mở thư mục dữ liệu** ở chân thanh bên trái mở đúng thư mục đó.
- **Sao lưu thế giới**: tab **Điều khiển** → **Sao lưu map** (file nén được lưu trong `backups` của server).
- **Sao lưu tự động**: tab **Cấu hình** → **Tự động hóa** → bật và chọn chu kỳ. Nên bật nếu server chạy thường xuyên.
- Muốn chuyển server sang máy khác: sao chép cả thư mục server trong `Data\servers` là xong.

## 7. Gỡ cài đặt

Mở **Settings → Apps → Installed apps** → tìm **MC Server Studio** → **Uninstall**.

> Lưu ý: gỡ cài đặt sẽ xoá cả thư mục `Data` (tức là toàn bộ server, thế giới, mod). Nếu muốn giữ, hãy **sao chép thư mục `Data` ra chỗ khác trước khi gỡ**.

## 8. Khi có trục trặc

| Hiện tượng | Cách xử lý |
|---|---|
| Windows báo "Unknown publisher" khi cài | Bấm **More info** → **Run anyway** (file cài chưa ký số) |
| Server khởi động rồi tự tắt | Tab **Điều khiển** → **Xem lỗi gần nhất**; hoặc mở tab **Console** xem dòng lỗi cuối |
| "Java quá cũ cho phiên bản này" | Tab **Cấu hình** → **Hiệu năng & Java** → **Sửa Java ngay** (ứng dụng tự tải bản đúng) |
| Cổng đang bị chiếm | Mở Task Manager, tìm `java.exe` và tắt, hoặc đổi cổng ở tab **Cấu hình** (ví dụ 25566) |
| Bạn bè báo "Outdated client/server" | Phiên bản Minecraft của họ phải trùng phiên bản server (xem ở tab **Cấu hình** → **Phiên bản**) |
| Bạn bè báo "not whitelisted" | Tab **Người chơi** → **Whitelist** → thêm tên họ, hoặc tắt whitelist ở tab **Cấu hình** |
| Không vào được từ internet | Tắt VPN/WARP, mở cổng (tab **Bạn bè & Mạng**), rồi bấm **Kiểm tra kết nối** |
| Server lag, TPS thấp | Tab **Cấu hình** → **Hiệu năng** → chọn preset **Máy yếu**, hoặc tăng RAM, hoặc bỏ bớt mod nặng |
| Muốn xem lại log để báo lỗi | Tab **Console** → **Lưu log** (file lưu trong `Data\logs`) |

## 9. Về bản quyền

- Đây là công cụ quản lý server, **không kèm tài nguyên có bản quyền của Mojang** (hình ảnh trong ứng dụng do chương trình tự vẽ, font dùng giấy phép mở SIL OFL).
- Ứng dụng tải Minecraft server chính thức từ Mojang khi bạn tạo server, và bạn cần **đồng ý với EULA của Minecraft** (`https://aka.ms/MinecraftEULA`) — đây là điều kiện bắt buộc để chạy server.

---

*MC Server Studio 3.0.0 — chúc bạn và hội bạn chơi vui!*
