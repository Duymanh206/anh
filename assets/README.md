# 🌸 Hướng dẫn thay thế hình ảnh & âm nhạc (assets)

Thư mục này dùng để lưu trữ các tài nguyên ảnh và nhạc cho trang web quà tặng 20/10.

---

### 1. Danh sách các file tài nguyên:

| Tên file | Mô tả | Định dạng khuyến nghị | Gợi ý kích thước |
| :--- | :--- | :--- | :--- |
| `bouquet.jpg` (hoặc `.png`) | Ảnh bó hoa xuất hiện ở màn hình mở đầu (Giai đoạn 1) | PNG (tách nền trong suốt) hoặc JPG chất lượng cao | Vuông (800x800 px đến 1200x1200 px) |
| `music.mp3` | Nhạc nền phát khi người dùng chạm vào bó hoa | MP3 | Dưới 10MB để tải nhanh trên điện thoại |
| `photo1.jpg` đến `photo20.jpg` | Các bức ảnh kỷ niệm bay lơ lửng trong vũ trụ 3D (Giai đoạn 2) | JPG, PNG, WebP | Tỉ lệ 1:1, 4:5 hoặc 3:4 (khoảng 600x600 px hoặc 800x800 px) |

---

### 2. Cách thay đổi nhanh bằng ảnh của bạn:

1. **Thay nhạc nền:** 
   - Đổi tên file nhạc của bạn thành `music.mp3` và chép đè vào thư mục `assets/`.
2. **Thay ảnh bó hoa:** 
   - Đổi tên ảnh bó hoa bạn thích thành `bouquet.jpg` và chép đè vào thư mục `assets/`.
3. **Thay ảnh kỷ niệm:** 
   - Chuẩn bị từ 15 đến 20 bức ảnh kỷ niệm của hai bạn / người bạn muốn tặng.
   - Đặt tên theo thứ tự: `photo1.jpg`, `photo2.jpg`, `photo3.jpg`, ..., `photo20.jpg`.
   - Bỏ tất cả vào thư mục `assets/`.

---

### 3. Cấu hình trong `index.html`:

Toàn bộ thông tin hiển thị được gom gọn trong biến `CONFIG` ở ngay đầu thẻ `<script>` của file `index.html`:
```javascript
const CONFIG = {
    // Đường dẫn ảnh bó hoa chính
    bouquetImage: 'assets/bouquet.jpg',
    
    // Đường dẫn file nhạc nền
    musicUrl: 'assets/music.mp3',
    
    // Danh sách các bức ảnh kỷ niệm bay trong không gian 3D
    memoryPhotos: [
        'assets/photo1.jpg',
        'assets/photo2.jpg',
        // Hoặc có thể dùng link ảnh trực tiếp từ internet (Unsplash, Cloudinary, Imgur, ...)
    ],
    
    // Tiêu đề & nội dung bức thư tình
    letter: {
        title: "Thân gửi em,",
        content: "Chúc một nửa thế giới của anh luôn xinh đẹp, rạng rỡ, ngập tràn niềm vui và luôn nở nụ cười trên môi trong ngày 20/10 này nhé!",
        signature: "Mãi yêu em,"
    }
};
```

> **Mẹo:** Bạn có thể mở `index.html` bằng bất kỳ trình soạn thảo nào (VS Code, Notepad, v.v.) để chỉnh sửa lời chúc và chữ ký bất cứ lúc nào!
