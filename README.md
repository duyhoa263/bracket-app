# ⚽ Cúp Đấu Loại Trực Tiếp

App tạo bảng đấu loại trực tiếp (knockout bracket) chạy trên iPhone dưới dạng web-app. Toàn bộ app nằm trong 1 file duy nhất: `index.html`.

## Cách đưa lên iPhone (chọn 1 trong 3 cách)

### Cách 1 — Netlify Drop (dễ nhất, miễn phí, ~1 phút)
1. Mở https://app.netlify.com/drop trên máy tính
2. Kéo thả **thư mục `bracket-app`** vào trang đó
3. Nhận được link dạng `https://ten-gi-do.netlify.app` — mở link này trên iPhone

### Cách 2 — GitHub Pages
1. Tạo repo mới trên GitHub, upload file `index.html`
2. Settings → Pages → bật GitHub Pages từ branch chính
3. Mở link `https://<user>.github.io/<repo>/` trên iPhone

### Cách 3 — Gửi file trực tiếp
Gửi `index.html` qua Zalo/AirDrop/iCloud → trên iPhone lưu vào app **Tệp (Files)** → chạm để mở bằng Safari. (Cách này chạy được nhưng cách 1/2 mượt hơn.)

## Cài như app thật trên iPhone
Mở link bằng **Safari** → nút **Chia sẻ** (ô vuông mũi tên) → **Thêm vào MH chính (Add to Home Screen)** → app chạy toàn màn hình như app native.

## Tính năng

### 🏟️ Giải đấu
- Bảng đấu loại trực tiếp **4 / 8 / 16 / 32 đội**, tùy chọn **tranh hạng 3**
- Nhập tỉ số từng trận; khi hòa tự hiện ô nhập **luân lưu 11m**; đội thắng tự đi tiếp
- **🎲 Bốc thăm** xáo trộn cặp đấu ngẫu nhiên

### 🛡️ Logo
- **Logo THẬT** của CLB 6 giải: Ngoại hạng Anh, La Liga, Serie A, Bundesliga, Ligue 1 (đủ ~20 CLB mỗi giải, logo chính thức) và V-League (9 CLB)
- **Quốc kỳ** ~85 quốc gia
- Tự tải logo lên hoặc tự thiết kế huy hiệu (chọn màu + chữ)
- Nếu mất mạng, logo thật tự thay bằng huy hiệu màu áo CLB

### 🎖️ Chế độ 2 HLV (Bên A đấu Bên B)
- Bật trong tab Đội, đặt tên 2 HLV. Nửa đầu danh sách = Bên A, nửa sau = Bên B
- **Bốc thăm đảm bảo 2 đội cùng bên KHÔNG gặp nhau ở vòng 1** — từ vòng sau đấu bình thường
- Đội bên nào vô địch → HLV bên đó chiến thắng (hiện ở banner, ảnh xuất và thống kê)

### 🔗 Chia sẻ cho người khác xem
- **Chia sẻ ảnh**: nút 📸 Xuất ảnh → Chia sẻ/Lưu → gửi PNG qua Zalo/Messenger
- **Chia sẻ link** (mới): nút 🔗 Chia sẻ link ở tab Sơ đồ — toàn bộ dữ liệu giải được nén vào trong link (~1KB). Người nhận mở link là xem được **nguyên sơ đồ tương tác** (vòng đấu, tỉ số, luân lưu, HLV, ghi chú) và có thể nhấn **📥 Lưu giải này về máy** để giữ lại. Không cần server, không cần tài khoản
- Lưu ý: link chỉ hoạt động khi app đã đưa lên mạng (Netlify/GitHub Pages); logo tự tải lên sẽ được thay bằng huy hiệu chữ trong link để link không quá dài

### 📸 Xuất ảnh + Ghi chú
- Nhấn Xuất ảnh → nhập **ghi chú** (tùy chọn) → ghi chú in ở **góc trái dưới ảnh**
- Ảnh PNG nét cao: đầy đủ sơ đồ, luân lưu, nhãn A/B, vô địch, hạng 3, HLV thắng
- Nút Chia sẻ/Lưu để lưu thẳng vào Ảnh trên iPhone

### 🗂 Lịch sử & 📊 Thống kê
- **💾 Lưu vào lịch sử** ở tab Sơ đồ (lưu lần 2 sẽ cập nhật, không tạo bản trùng)
- Tab Lịch sử: xem lại các giải (vô địch, á quân, HLV thắng, ghi chú), **Mở lại** hoặc Xóa
- Tab Thống kê (cộng dồn từ các giải đã lưu):
  - Số lần **vô địch / á quân** từng đội
  - Số lần thắng của mỗi **HLV**
  - **BXH cộng dồn**: Trận, Thắng, Hòa, Thua, Bàn thắng/thua, Điểm (T=3đ, H=1đ, B=0đ)
  - Trận phân định bằng luân lưu tính là **hòa** cho cả 2 đội (mỗi đội 1 điểm)

## Lưu ý
- Logo thật và quốc kỳ tải từ mạng (jsDelivr / flagcdn / thesportsdb) — cần internet lần đầu
- Dữ liệu + lịch sử lưu trên máy (localStorage của Safari) — không xóa dữ liệu Safari nếu muốn giữ lịch sử
