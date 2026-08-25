# G-Labs Video Downloader

[English](README.md) | **Tiếng Việt**

Ứng dụng desktop tải video từ **YouTube, TikTok, Facebook, Instagram, X/Twitter, Twitch, Vimeo, Reddit, SoundCloud, Bilibili và hơn 1.800 trang khác** — với engine tải đa nền tảng tự cập nhật đóng gói sẵn. Mọi thứ nằm trong app, không cần cài thêm gì.

![Cửa sổ chính](docs/screenshots/01-main.png)

## Tính năng

- **Dán gì cũng được**: video lẻ, playlist, cả kênh, YouTube Shorts — dán nhiều link mỗi dòng một link; nút **?** mở hướng dẫn chi tiết mọi nền tảng & kiểu link hỗ trợ
- **Định dạng**: MP4 (tốt nhất / 1080p / 720p / 480p) · MP3 192 kbps · ảnh thumbnail JPG · phụ đề SRT · **chế độ chỉ-lấy-kèm** (thumbnail/phụ đề mà không tải video)
- **Hàng đợi song song**: 1–10 luồng, hiển thị %, tốc độ, thời gian còn lại; **lọc theo trạng thái** (đang xử lý / hoàn thành / lỗi / huỷ) + tick chọn hàng và "chạy mục chọn"
- **Xem trước playlist / kênh**: lấy danh sách trước, tick đúng video muốn tải (kênh YouTube có tab Video/Shorts)
- **Chống tải trùng**: lịch sử tải bền vững, tự bỏ qua video đã tải (theo định dạng) — bấm một nút nếu muốn tải lại
- **Thử lại**: từng video hoặc tất cả video lỗi (engine cũng tự retry với backoff)
- **Xuất CSV**: hàng đợi + lỗi, mở đẹp trong Excel (UTF-8 BOM); nhật ký hoạt động có nút copy/xuất
- **Nhập cookie siêu nhanh**: dán định dạng NÀO cũng được — `cookies.txt` Netscape, JSON từ extension trình duyệt, hoặc chuỗi header thô `a=1; b=2` — theo từng nền tảng hoặc dùng chung, để tải nội dung giới hạn tuổi / cần đăng nhập
- **Proxy pool**: dán DANH SÁCH proxy (định dạng nào cũng được — `host:port:user:pass`, `user:pass@host:port`, URL `socks5://` đầy đủ, IPv6) — mỗi video tải lần lượt xoay vòng; nút "kiểm tra tất cả"
- **Engine tự cập nhật**: engine tải tự update mỗi 24h (+ nút thủ công) nên YouTube đổi gì cũng không sợ hỏng
- **App tự cập nhật**: kiểm tra GitHub Releases, tải và cài ngay trong app
- **6 ngôn ngữ**: English, Tiếng Việt, 简体中文, Español, العربية (RTL), Русский

## Ảnh màn hình

| Xem trước playlist / kênh | Hướng dẫn link hỗ trợ |
|---|---|
| ![Preview](docs/screenshots/02-preview.png) | ![Help](docs/screenshots/03-help.png) |

| Nhập cookie nhanh | Proxy pool (xoay vòng) |
|---|---|
| ![Cookies](docs/screenshots/04-cookies.png) | ![Proxy](docs/screenshots/05-proxy.png) |

| Lịch sử tải | RTL (العربية) |
|---|---|
| ![History](docs/screenshots/06-history.png) | ![RTL](docs/screenshots/07-rtl-arabic.png) |

## Cài đặt

Tải bản mới nhất tại [Releases](https://github.com/duckmartians/G-Labs-Video-Downloader/releases):

- **Windows**: `GLabsVideoDownloader-<version>-setup.exe`
- **macOS (Apple Silicon)**: `GLabsVideoDownloader-<version>-arm64.dmg` — chưa ký; mở lần đầu: chuột phải → Open, hoặc `xattr -dr com.apple.quarantine "/Applications/G-Labs Video Downloader.app"`

Thiết lập và lịch sử nằm trong thư mục dữ liệu người dùng của HĐH (`%APPDATA%\G-Labs Video Downloader` trên Windows, `~/Library/Application Support/G-Labs Video Downloader` trên macOS). Video tải về mặc định vào `Documents/G-Labs Video Downloader`.
