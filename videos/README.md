# Video

Bỏ video kỷ niệm vào thư mục này, đặt tên:

```text
01.mp4
02.mp4
```

Rồi mở `index.html`, sửa `CONFIG.videos` cho khớp:

```js
videos: [
  {
    src: "videos/01.mp4",
    poster: "images/01.jpg",
    caption: "Một đoạn ngắn",
    date: "2026"
  }
]
```

- `src`: đường dẫn video, thường là `.mp4` (H.264 + AAC là dễ chạy nhất). `.webm` cũng được; khi đó thêm `type: "video/webm"` hoặc để trang tự nhận theo đuôi file.
- `poster`: ảnh hiển thị trước khi video chạy. Có thể để `""` nếu không cần.
- `caption` / `date`: chữ hiện dưới khung video.
- Video **không tự phát**. Người xem bấm nút play trên trình duyệt.
- Nếu chưa có file, khung sẽ hiện “Một thước phim đang chờ” thay vì video lỗi.
- Nên nén video khoảng 1080p, dưới 20–30 MB mỗi clip để trang mở nhanh.
- Có thể thêm hoặc bớt phần tử trong `CONFIG.videos`; giao diện tự chia 2 cột trên desktop, 1 cột trên mobile.
