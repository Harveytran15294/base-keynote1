# Keynote1 · Work Operating System

Deck trình chiếu cho Enterprise AI Summit 2026 (Keynote 1). 19 slide, 2560×1280.

## Deploy trên Vercel
1. Push thư mục này lên nhánh `main` của repo.
2. Vercel → Add New → Project → Import Git Repository → chọn repo.
3. Framework Preset: **Other**. Build Command: để trống. Output Directory: `.`
4. Deploy. Mỗi lần push là Vercel tự cập nhật.

## Nội dung thư mục
- `index.html` — deck tự chứa (font Afacad, ảnh, screenshot đã nhúng).
- `mock-*.html` — 7 mock chạy động, nhúng trong slide qua iframe:
  `mock-request` (Base Requests), `mock-bpm`, `mock-bpm-feat` (Base Workflow),
  `mock-service` (kiến trúc #Service), `mock-eoffice`, `mock-projects-app`, `mock-meetings`.
- `assets/` — logo Base, icon ứng dụng, avatar dùng trong các mock.

Giữ nguyên cấu trúc thư mục; mock đọc ảnh theo đường dẫn `assets/...`.

## Điều khiển khi trình chiếu
- `→` / `Space`: bước tiếp · `←`: lùi · `Home` / `End`: đầu, cuối deck
- `R`: chạy lại animation của slide · `F`: toàn màn hình
- `H`: hiện/ẩn thanh điều khiển · `S`: thanh thumbnail · `N`: ghi chú người nói
- `P`: presenter view (mở thêm cửa sổ khán giả, hai cửa sổ đồng bộ)
- URL dạng `#/14/3` mở đúng slide 14, bước 3.

## Lưu ý màn hình LED 9 m
Vùng an toàn 160px ngang, 128px trên dưới. 10% dưới cùng bị ghế khán giả che, đã tránh đặt nội dung ở đó.
