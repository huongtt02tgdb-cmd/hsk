# Hànyǔ – Ôn HSK 1 (bản riêng, link thứ hai)

- 500 từ HSK 1 (chuẩn HSK 3.0), 20 ngày × 25 từ, có Hán Việt, loại từ, câu ví dụ có nút nghe.
- Tab "Ngữ pháp" có Bài 1–5 (256 câu: nghe, đọc, viết, hiểu) theo sổ bài tập 新HSK教程 1. File `bai-tap-hsk-1-5.json` cùng nội dung, chỉ cần khi muốn nhập thủ công.
- Dữ liệu lưu riêng với Kotoba (khóa `hsk-...`), hai app không lẫn nhau dù cùng tên miền github.io.

## Đưa lên GitHub (link thứ hai)
1. GitHub Desktop → File → New repository → tên **hsk** → Create.
2. Chép TOÀN BỘ nội dung thư mục này (index.html, manifest.json, sw.js, icons, texts.json, tao_audio.py...) vào thư mục repo `hsk`.
3. Mở cmd **trong thư mục repo hsk** (thấy texts.json và tao_audio.py), chạy:
   `pip install edge-tts` rồi `python tao_audio.py` (giọng nữ Xiaoxiao, ~1050 file; chạy lại được, file nào có rồi sẽ bỏ qua).
4. GitHub Desktop → Commit → Publish repository (bỏ dấu tick "Keep this code private").
5. github.com → repo hsk → Settings → Pages → Branch `main`, thư mục `/ (root)` → Save.
6. Link: `https://huongtt02tgdb-cmd.github.io/hsk/` (đợi 1–2 phút).

## Bật đồng bộ chuỗi học
Xem file HUONG_DAN_DONG_BO.md.
