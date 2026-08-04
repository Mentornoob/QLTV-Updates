# QLTV-Updates

Trang giới thiệu và metadata cập nhật công khai cho QLTV Desktop.

## Website

Website tĩnh chạy trực tiếp trên GitHub Pages:

- Giới thiệu ứng dụng và tính năng chính.
- Tự đọc phiên bản mới nhất từ `update.json`.
- Hiển thị lịch sử phát hành từ GitHub Releases.
- Liên kết tải bộ cài và tệp kiểm tra SHA-256.
- Giao diện responsive cho máy tính và điện thoại.

## Chạy cục bộ

```powershell
python -m http.server 8000
```

Mở `http://localhost:8000`.

## Triển khai

Workflow `.github/workflows/pages.yml` tự triển khai khi có thay đổi trên nhánh `main` hoặc `master`. Trong **Settings → Pages**, chọn nguồn **GitHub Actions**.

Mã nguồn chính của QLTV hiện được giữ riêng tư.
