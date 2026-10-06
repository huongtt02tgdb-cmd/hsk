# Hànyǔ – Ôn HSK 1 (bản riêng, link thứ hai)

- 500 từ HSK 1 (chuẩn HSK 3.0), 20 ngày × 25 từ, có Hán Việt, loại từ, câu ví dụ có nút nghe.
- Tab "Ngữ pháp": Bài 1–5 (256 câu: nghe, đọc, viết, hiểu) theo sổ bài tập 新HSK教程 1. File `bai-tap-hsk-1-5.json` cùng nội dung, chỉ cần khi muốn nhập thủ công.
- Tab "Tài liệu": xem PDF, Word (.docx), Excel, CSV, văn bản, ảnh, âm thanh, video ngay trên trang (xem bên dưới).
- Dữ liệu lưu riêng với Kotoba (khóa `hsk-...`), hai app không lẫn nhau dù cùng tên miền github.io.

## Đưa lên GitHub (link thứ hai)
1. Chép TOÀN BỘ nội dung thư mục này (index.html, manifest.json, sw.js, icons, lib, docs, texts.json...) vào thư mục repo `hsk`.
2. Tạo âm thanh: mở cmd **trong thư mục repo hsk** (thấy texts.json và tao_audio.py), chạy
   `pip install edge-tts` rồi `python tao_audio.py` (giọng nữ Xiaoxiao, ~1050 file; chạy lại được, file nào có rồi sẽ bỏ qua).
3. GitHub Desktop → Commit → Push (hoặc Publish repository nếu chưa lên mạng).
4. github.com → repo hsk → Settings → Pages → Branch `main`, thư mục `/ (root)` → Save.
5. Link: `https://huongtt02tgdb-cmd.github.io/hsk/`

## Thêm tài liệu cho tab "Tài liệu"
1. Bỏ file vào thư mục **docs** của repo (có thể chia thư mục con, mỗi thư mục con là một nhóm).
   Định dạng xem được ngay: PDF, Word (.docx), Excel (.xlsx/.xls), CSV, .txt/.md, ảnh, mp3, mp4. PowerPoint và Word cũ (.doc) chưa xem trực tiếp được (có nút Tải về); nên đổi sang PDF.
2. Commit và Push. Người dùng mở tab Tài liệu là thấy danh sách (app tự đọc danh sách từ GitHub; nếu muốn chắc chắn hơn thì chạy `python tao_danh_muc.py` để tạo docs/index.json rồi Push).
3. Người dùng cũng có thể bấm "Mở file từ máy" để xem file của riêng họ, không bị tải lên đâu cả.
Lưu ý: mỗi file tối đa 100 MB (giới hạn của GitHub); tổng cả trang khoảng 1 GB.

## Bật đồng bộ chuỗi học
Xem file HUONG_DAN_DONG_BO.md.
