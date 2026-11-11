# Bộ não tri thức

Trang khởi động để thêm **Bộ não tri thức** vào Màn hình chính iPhone với icon riêng (bật GitHub Pages: Settings → Pages → Deploy from a branch → `main` / root).

## Định dạng dữ liệu (đường chuyển sang app độc lập)

Trong app: ⚙ → *Dữ liệu của anh* → **Markdown .zip** hoặc **Sao lưu Google Drive** sẽ xuất:

```
bo-nao-tri-thuc/
  CLAUDE.md          ← bản đồ bộ não: các chòm sao, loại tri thức, mục cần nhớ, mục hay dùng
  du-lieu.json       ← dữ liệu gốc đầy đủ (khôi phục vào app bằng “Khôi phục JSON”)
  cong-viec/dia-chat/2026-11-11-ten-tri-thuc-xxxx.md
  gia-dinh/...
  ky-niem/...
```

Mỗi file `.md` có frontmatter (`id, title, brain, sub, kind, date, tags, pinned, views`), nội dung, và mục `## Liên kết` dạng `[[tiêu đề]] — loại quan hệ`.
Có thể giải nén thư mục này vào repo để dùng như “bộ não thứ hai” với Claude Code, hoặc nạp vào một app độc lập (Supabase + Claude API) sau này mà không mất gì.
