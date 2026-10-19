# 🌸 Món Quà 20/10 Dành Tặng Ánh Tuyết 💖

> Trang web tương tác 3D lãng mạn, tinh tế với nghệ thuật ánh sáng, hoa hồng ma thuật, thiệp kính mờ Glassmorphism và Ngân hà Điều Ước dành riêng cho cô bé Ánh Tuyết nhân ngày Phụ nữ Việt Nam 20/10.

---

## ✨ Điểm nổi bật & Trải nghiệm tương tác

### 1. 🌌 Vũ trụ đêm & Cánh hoa bay (Background)
- Nền vũ trụ đêm mộng mơ chuyển sắc từ tím than đậm (`#07040a`) sang hồng tím pastel nhẹ ở tâm.
- Hàng trăm ngôi sao lấp lánh (twinkling stars), đom đóm phát sáng và sao băng (shooting stars) bay ngang qua.
- Những cánh hoa hồng phát sáng bay lượn nhẹ nhàng trong không gian.
- Phông chữ nghệ thuật Google Font **Mali** hỗ trợ tiếng Việt mềm mại, đáng yêu.

### 2. 🌹 Giai đoạn 1: Bó hoa ma thuật (Màn hình mở đầu)
- Bó hoa hồng phấn bay lơ lửng ở giữa màn hình, tỏa hào quang hồng dịu.
- Dòng chữ phát sáng: **"Chạm vào bó hoa nhé"**.
- **Tương tác 1 (Chạm vào bó hoa):** Bật nhạc nền piano lãng mạn và làm xuất hiện 5 từ khóa dễ thương bay lên từ bó hoa với hiệu ứng nảy đàn hồi:
  - 🌸 *Xinh đẹp*
  - 💖 *Đáng yêu*
  - ☀️ *Vui vẻ*
  - 🎀 *Hồn nhiên*
  - 🍀 *May mắn*
- Dòng chữ đổi thành: **"Ấn giữ bó hoa để mở điều bất ngờ"**.
- **Tương tác 2 (Ấn giữ 1.5s):** Bó hoa rung nhẹ tích tụ năng lượng ánh sáng, rồi bung tỏa ngàn hạt sáng rực rỡ để bước vào Giai đoạn 2.

### 3. 🪐 Giai đoạn 2: Ngân hà Điều Ước 3D (Three.js WebGL)
- Không gian 3D tương tác 360 độ (xoay, cuộn, chụm 2 ngón tay trên điện thoại để phóng to/thu nhỏ).
- **12 Tấm thiệp pha lê (Glassmorphism Cards)** viền sáng neon hồng, trang trí icon hoa, ngôi sao, mặt trăng với những lời chúc ý nghĩa (chạm vào thiệp để xem phóng to).
- **Các câu chúc 3D phát sáng Neon hồng** bay lơ lửng dành riêng cho Ánh Tuyết:
  - *"Chúc cô bé Ánh Tuyết 20/10 ngập tràn niềm vui ✨"*
  - *"Luôn giữ nụ cười tươi và sự hồn nhiên này nhé"*
  - *"Mong mọi điều dịu dàng nhất sẽ đến với em"*
  - *"Chúc em luôn xinh đẹp và rạng rỡ 🌸"*
  - *"Hôm nay của cô nhóc thế nào? Nhớ luôn vui vẻ nha!"*
  - *"Chúc em luôn gặp nhiều may mắn và bình an"*
  - *"Học tập thật tốt và luôn yêu đời nhé"*
- Hàng chục trái tim 3D và bụi sao lung linh bay xung quanh.

### 4. 💌 Bức thư tình dành riêng cho Ánh Tuyết (UI Overlay)
- Nút Phong bì thư ở góc phải có **hiệu ứng nhịp đập thu hút (heartbeat)**.
- **Popup bức thư màu hồng kem ấm áp (`#fff0f3`):**
  - Tiêu đề: **"Gửi Ánh Tuyết nhỏ, 🌸"**
  - Nội dung gõ chữ từng chữ một (**typewriter effect**):
    > *"Nhân ngày 20/10, anh có một món quà nhỏ tự tay chuẩn bị dành tặng cho cô bé. Chúc Ánh Tuyết của anh luôn xinh đẹp, rạng rỡ, học thật giỏi và lúc nào cũng cười tươi thế này nhé. Mong rằng mọi điều tốt đẹp nhất sẽ luôn ở bên em!"*
  - Chữ ký: **"Từ một người luôn quan tâm em ✨"**
- Nút Quay lại (X) để quay về màn hình bó hoa ban đầu bất cứ lúc nào.
- Nút Bật/Tắt nhạc nền với thanh sóng âm chuyển động.

---

## 🛠️ Cấu hình dễ dàng thay đổi (`CONFIG`)

Toàn bộ thông tin được gom gọn tại đối tượng `CONFIG` ở ngay đầu thẻ `<script>` của [index.html](file:///d:/HOÀNG%20DUY%20MẠNH/2/index.html):
```javascript
const CONFIG = {
    crushName: "Ánh Tuyết",
    bouquetImage: 'assets/bouquet.jpg',
    musicUrl: 'assets/music.mp3',
    keywords: [ ... ],       // Từ khóa bay lên ở Giai đoạn 1
    crystalCards: [ ... ],   // 12 Tấm thiệp pha lê 3D
    greetings: [ ... ],      // Câu chúc Neon 3D
    letter: { ... }          // Bức thư gửi Ánh Tuyết
};
```

---

## 🚀 Triển khai (Deploy lên Vercel)

Dự án là trang web tĩnh HTML/CSS/Three.js thuần túy:
1. Đăng nhập [vercel.com](https://vercel.com) với tài khoản GitHub.
2. Chọn **"Add New..."** ➔ **"Project"**.
3. Import repository **`Duymanh206/anh`**.
4. Nhấn **"Deploy"** để nhận link web trực tuyến gửi tặng Ánh Tuyết!
