# Thư mục ảnh kỷ niệm

Trang **không tự quét thư mục này**. Ảnh trong album do được khai báo trong `CONFIG.gallery`; ảnh nền trang nằm trong `.page-bg-track`.

## Thêm ảnh vào album

1. Bỏ ảnh vào thư mục này. Tên file có thể giữ nguyên, không bắt buộc `01.jpg`.
2. Mở `index.html`, tìm `CONFIG.gallery`.
3. Thêm một dòng với đúng tên file:

```js
{
  src: "images/ten-file.jpg"
}
```

Nếu chỉ copy ảnh vào thư mục mà không thêm vào `CONFIG.gallery`, trang sẽ không biết ảnh đó tồn tại.

## Gợi ý

- Ảnh được crop theo khung dọc **4:5**; nên chọn ảnh có chủ thể ở giữa.
- Resize về khoảng 1200–1600px chiều ngang để trang nhẹ.
- Dùng `.jpg`, `.png` hoặc `.webp`; chỉ cần sửa đuôi file trong `src`.
- Ảnh dọc/ngang đều được, trang tự crop.
- Album hiện dùng toàn bộ 21 ảnh có sẵn, không caption; có thể thêm hoặc bớt dòng trong `CONFIG.gallery`.

Nếu ảnh thiếu, trang hiện khung giấy “Một khung hình đang chờ”. Bấm vào khung sẽ mở lightbox với lời nhắc thêm ảnh.

## Ảnh nền trang

Đặt ảnh muốn dùng làm nền chung vào thư mục này, rồi thêm/sửa `src` trong `.page-bg-track` ở đầu `<body>` của `index.html`:

```html
<div class="page-bg-track" id="pageBgTrack">
  <img src="images/ten-file.jpg" alt="" decoding="async" onerror="this.remove()">
</div>
```

Các ảnh trong track xếp dọc và lần lượt xuất hiện khi cuộn. Ảnh nền hero nằm trong `CONFIG.heroPhotos`, không dùng chung với album này.
