# 🌸 Bó hoa ảnh - Chúc mừng Ngày Phụ Nữ Việt Nam 20/10 💖

> Trang web quà tặng 3D tương tác lãng mạn, tinh tế và ngọt ngào dành tặng người phụ nữ bạn yêu thương nhân ngày 20/10.

---

## ✨ Điểm nổi bật & Tính năng chính

### 1. 🌌 Vũ trụ lãng mạn & Sao băng
- Hiệu ứng bầu trời đêm màu tím than chuyển sắc (`#07040a` đến `#1a0926`) với quầng sáng hồng tím kỳ ảo.
- Hàng trăm ngôi sao lấp lánh (twinkling stars) cùng sao băng (shooting stars) bay ngang trời ngẫu nhiên.
- Phông chữ tiếng Việt nghệ thuật Google Font **Mali** mềm mại và ngọt ngào.
- Tối ưu SEO & Thẻ Open Graph (hiển thị ảnh preview tuyệt đẹp khi chia sẻ link qua Zalo, Messenger, Facebook).

### 2. 🌹 Giai đoạn 1: Bó hoa tương tác
- Bó hoa hồng phấn bay lơ lửng nhẹ giữa màn hình với quầng sáng lung linh.
- **Tương tác 1 (Chạm vào bó hoa):** Phát bản nhạc lãng mạn và 6 khung ảnh Polaroid bất ngờ bung nở xung quanh bó hoa với hiệu ứng nảy (spring animation).
- **Tương tác 2 (Ấn giữ bó hoa 1.5s):** Bó hoa rung nhẹ, tích tụ ánh sáng qua vòng đo năng lượng, rồi bùng nổ chuyển cảnh sang Vũ trụ tình yêu 3D.

### 3. 🪐 Giai đoạn 2: Vũ trụ tình yêu 3D (Three.js WebGL)
- Không gian 3D tương tác 360 độ: kéo chuột / vuốt ngón tay để xoay, cuộn chuột hoặc chụm 2 ngón để phóng to/thu nhỏ.
- **18 - 20 khung ảnh kỷ niệm Polaroid** bay lơ lửng, chuyển động nhịp nhàng (bấm vào ảnh bất kỳ để mở xem to).
- **Các câu chúc 20/10 phát sáng Neon hồng** bay lơ lửng trong không gian:
  - *"Chúc mừng 20/10 thật hạnh phúc ❤️"*
  - *"Chúc em luôn xinh đẹp ✨"*
  - *"Mãi yêu em 💖"*
  - *"Chúc em luôn vui vẻ và hạnh phúc 🌸"*
  - *"Mong mọi điều dịu dàng sẽ đến với em 💫"*
  - *"Chúc em thật nhiều may mắn 🍀"*
  - *"Chúc em luôn yêu đời 💐"*
- Hàng chục **trái tim 3D đỏ/hồng** xoay nhịp nhàng và hàng trăm hạt đom đóm / bụi sao lấp lánh.

### 4. 💌 Bức thư tình & Nút điều khiển (Glassmorphism)
- **Nút Bức thư:** Mở chiếc thiệp tình yêu màu hồng phấn (`#ffe6eb`) với hiệu ứng gõ chữ từng chữ (typewriter effect) chân thật và chữ ký ngọt ngào.
- **Nút Bật/Tắt nhạc:** Điều khiển âm thanh tiện lợi với thanh sóng âm động.
- **Nút Đóng (X):** Quay trở lại màn hình Bó hoa ban đầu bất cứ lúc nào.

---

## 📂 Cấu trúc thư mục

```tree
├── index.html          # Toàn bộ mã nguồn HTML5, CSS3, Three.js 3D & Animation
├── assets/             # Thư mục chứa tài nguyên ảnh và nhạc
│   ├── bouquet.jpg     # Ảnh bó hoa chính
│   ├── music.mp3       # Nhạc nền lãng mạn
│   └── README.md       # Hướng dẫn chi tiết cách thay đổi ảnh và nhạc
└── README.md           # Giới thiệu dự án và hướng dẫn sử dụng
```

---

## 🛠️ Tùy biến nội dung (CONFIG)

Mở file `index.html`, bạn sẽ thấy đối tượng `CONFIG` ngay ở đầu thẻ `<script>`:

```javascript
const CONFIG = {
    bouquetImage: 'assets/bouquet.jpg',   // Ảnh bó hoa chính
    musicUrl: 'assets/music.mp3',         // Nhạc nền
    memoryPhotos: [ ... ],                // Danh sách link ảnh kỷ niệm
    greetings: [ ... ],                   // Các câu chúc bay trong 3D
    letter: {                             // Nội dung thiệp tình yêu
        title: "Thân gửi em,",
        content: "Chúc một nửa thế giới của anh luôn xinh đẹp, rạng rỡ, ngập tràn niềm vui...",
        signature: "Mãi yêu em,"
    }
};
```

---

## 🚀 Triển khai (Deploy lên Vercel)

Dự án là trang tĩnh 100% chuẩn HTML/CSS/JS, không cần cài đặt dependencies hay build phức tạp:

1. Đăng nhập vào [Vercel](https://vercel.com).
2. Chọn **"Add New..."** -> **"Project"**.
3. Import GitHub repository: `Duymanh206/anh`.
4. Bấm **"Deploy"** — trang web sẽ online chỉ sau vài giây với tên miền miễn phí!
