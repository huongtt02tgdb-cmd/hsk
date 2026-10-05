# Hànyǔ – Ôn HSK 1 (bản riêng, link thứ hai)

Gồm 500 từ HSK 1 (chuẩn HSK 3.0) chia 20 ngày × 25 từ, có Hán Việt, loại từ, câu ví dụ có nút nghe.
Dữ liệu lưu riêng với Kotoba (khóa `hsk-...`), nên hai app không lẫn vào nhau dù cùng tên miền github.io.

## Đưa lên GitHub (link thứ hai)
1. GitHub Desktop → File → New repository → tên **hsk** → Create.
2. Chép TOÀN BỘ nội dung thư mục này (index.html, manifest.json, sw.js, icons, texts.json, tao_audio.py...) vào thư mục repo `hsk`.
3. Tạo âm thanh (làm trước khi đẩy lên): mở cmd **trong thư mục repo hsk**, chạy
   `pip install edge-tts` rồi `python tao_audio.py` (giọng nữ Xiaoxiao, ~980 file, chạy lại được, file nào có rồi sẽ bỏ qua).
4. GitHub Desktop → Commit → Publish repository (bỏ dấu tick "Keep this code private").
5. Trên github.com: repo hsk → Settings → Pages → Branch `main`, thư mục `/ (root)` → Save.
6. Link sẽ là `https://huongtt02tgdb-cmd.github.io/hsk/` (đợi 1–2 phút).

## Cách nhập thêm / sao lưu
Giống Kotoba: nhập file Excel (cột Ngày | Pinyin | Hán tự | Nghĩa), sao lưu và khôi phục, xóa.
Ngữ pháp: tab "Ngữ pháp" đang trống, sẽ thêm bài tập khi bạn gửi tiếp và bảo làm.
