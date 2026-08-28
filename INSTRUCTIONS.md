# 🚀 Hướng Dẫn Kích Hoạt GitHub Profile README

Để biến file này thành giao diện Profile chính thức trên trang cá nhân GitHub của bạn:

---

### Bước 1: Tạo Special Repository trên GitHub
1. Truy cập [GitHub](https://github.com) và tạo một Repository mới (**New repository**).
2. Đặt tên Repository **trùng hoàn toàn với GitHub Username của bạn** (Ví dụ: nếu username là `nguyenvana`, repository name phải là `nguyenvana`).
3. Đảm bảo chọn chế độ **Public** và tick chọn **Add a README file** (hoặc tạo repo trống).

---

### Bước 2: Tùy chỉnh thông tin cá nhân trong `README.md`
Mở file [README.md](file:///d:/FPT/project/ReadmeProfileGithub/README.md) và thay thế các từ khóa giữ chỗ sau bằng thông tin của bạn:
- `YOUR_NAME`: Tên hiển thị của bạn (Ví dụ: `Nguyen Van A`)
- `YOUR_GITHUB_USERNAME`: Username GitHub của bạn (Ví dụ: `nguyenvana`)
- `YOUR_LINKEDIN`: Đường dẫn hoặc username LinkedIn
- `YOUR_EMAIL`: Địa chỉ email nhận liên hệ
- `YOUR_FACEBOOK`: Username hoặc link trang cá nhân Facebook
- `YOUR_PORTFOLIO_OR_WEBSITE`: Website cá nhân hoặc blog của bạn (nếu chưa có có thể tạm bỏ badge này)
- Tech stack: Bạn có thể thêm/bớt icon công nghệ tuỳ theo sở trường thực tế (Java, Go, NestJS, Spring Boot, Docker, Redis, Postgres,...).

---

### Bước 3: Kích hoạt Game Rắn (Snake Contribution Animation)
File workflow tự động đã được chuẩn bị sẵn tại [.github/workflows/snake.yml](file:///d:/FPT/project/ReadmeProfileGithub/.github/workflows/snake.yml).

1. Sau khi push toàn bộ thư mục lên repository `<username>/<username>` của bạn trên GitHub.
2. Vào tab **Settings** của repository -> mục **Actions** -> **General**.
3. Cuộn xuống phần **Workflow permissions** -> Chọn **Read and write permissions** -> Bấm **Save**.
4. Chuyển sang tab **Actions** -> Chọn workflow **Generate Snake Animation** ở cột trái -> Bấm nút **Run workflow** để chạy thử lần đầu.
5. Sau khi chạy xong, nhánh `output` sẽ tự động được tạo và file SVG rắn ăn ô commit sẽ hiển thị mượt mà trên Profile của bạn!

---

### Bước 4: Tự động cập nhật Blog Posts (Tùy chọn)
Nếu bạn có Blog cá nhân (Substack, Dev.to, Medium, hoặc RSS feed):
- Bạn có thể dùng action `gautamkrishnar/blog-post-workflow` để tự động kéo bài viết mới nhất vào giữa 2 thẻ `<!-- BLOG-POST-LIST:START -->` và `<!-- BLOG-POST-LIST:END -->`.
