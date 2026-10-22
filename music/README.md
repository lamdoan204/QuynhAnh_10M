# Thư mục nhạc

Bỏ file nhạc vào đây và sửa `CONFIG.music` trong `index.html` cho khớp. Hiện tại:

```text
JVKE_-_oh_to_be_loved_(Official_Lyric_Video).mp3
```

**Gợi ý:**

- Dùng `.mp3`; file hiện tại khoảng 5,3 MB.
- Nhạc tự phát khi bấm mở bìa thư, sau đó lặp lại.
- Nút `Nhạc` ở góc phải dùng để bật/tắt.
- Mở bằng `?letter=0` sẽ không tự phát; bấm nút để bật.
- Muốn ẩn nút nhạc? Đặt `music: ""` trong `CONFIG`.
- Âm lượng mặc định 0.38; tìm `audio.volume = 0.38` trong JavaScript nếu muốn đổi.
