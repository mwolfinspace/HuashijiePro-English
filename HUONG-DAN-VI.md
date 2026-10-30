# Huashijie Pro 3.4.6 — Bản tiếng Anh, tải về là vẽ (không cần cài đặt)

**Huashijie Pro** (画世界Pro) là phần mềm vẽ tranh chuyên nghiệp: minh hoạ, comic, làm
animation, hơn 150 cọ vẽ, layer nâng cao, filter, xuất PSD / PNG / JPG / TIFF / GIF / MP4.

Bản gốc chỉ có tiếng Trung. Đây là bản **đã dịch toàn bộ giao diện sang tiếng Anh** và
đóng gói sẵn để **chạy trực tiếp — không cài đặt, không cần quyền admin, không cần đăng ký**.

---

## 1. Tải về

| Nơi tải | Link |
|---|---|
| **GitHub** (trang chính) | https://github.com/mwolfinspace/HuashijiePro-English/releases/latest |
| **Tải trực tiếp file zip** | https://github.com/mwolfinspace/HuashijiePro-English/releases/download/v3.4.6/HuashijiePro-English-3.4.6-win64.zip |

- Dung lượng: **257 MB** (giải nén ra khoảng 530 MB)
- SHA-256: `3200deaffa59f56f1360f2f6c0b8b5301188733f71c990400a9c946d2f798d8e`

---

## 2. Cách dùng — 3 bước

**Bước 1.** Tải file `HuashijiePro-English-3.4.6-win64.zip`.

**Bước 2.** Chuột phải vào file → **Extract All…** → chọn một thư mục → **Extract**.
(Không mở file trực tiếp trong cửa sổ nén — phải giải nén ra thư mục.)

**Bước 3.** Mở thư mục vừa giải nén → nhấp đúp vào:

> **`Start Huashijie Pro (English).exe`**

Xong. App mở lên, bấm **New** để tạo canvas và vẽ.

### Lần đầu mở
- Windows có thể hiện *“Windows protected your PC”* → bấm **More info** → **Run anyway**.
  App không có chữ ký số nên Windows hay cảnh báo; đây là file bình thường.
- Lần đầu hơi chậm vài giây vì app tạo cache. Những lần sau mở rất nhanh.

---

## 3. Vì sao phải bấm file `Start...` mà không phải `hsjpro.exe`?

Lần chạy đầu, app tự tạo thư viện cọ trong `%LOCALAPPDATA%\HuashijiePro` và lấy tên cọ từ đó.
File `Start...` sẽ chép sẵn **bộ cọ đã dịch tiếng Anh** vào (chỉ khi máy chưa có), rồi mới mở app.

Nếu bạn mở thẳng `hsjpro.exe` thì app vẫn chạy và vẽ bình thường, chỉ là **tên cọ sẽ là tiếng Trung**.
Mở bằng `Start...` một lần là đủ, sau đó thích mở file nào cũng được.

---

## 4. Có gì trong bản này

- Toàn bộ menu, bảng công cụ, hộp thoại, tooltip → **tiếng Anh**.
- **26 nhóm cọ** và **359 tên cọ** đã dịch; tên bảng phím tắt, bảng màu, danh sách quốc gia cũng đã dịch.
- **Sửa lỗi:** vùng chọn (selection) giờ **đi theo Flip Canvas** (bản gốc chỉ lật hình, vùng chọn đứng yên).
  Đúng cho cả Lasso, Magic Wand và **Ctrl+click vào layer** (chọn theo vùng của layer) — vùng chọn lật
  đúng tâm canvas, không bị lệch.
- Chạy **portable**: không ghi vào `Program Files`, không cần cài Qt / runtime, không cần quyền admin.

---

## 5. Dữ liệu của bạn nằm ở đâu?

Tranh và cài đặt được lưu ở:

```
%LOCALAPPDATA%\HuashijiePro
```

(ví dụ `C:\Users\TênBạn\AppData\Local\HuashijiePro`)

- **Sao lưu:** copy nguyên thư mục này.
- **Reset về mặc định:** đóng app, xoá thư mục này (nhớ xuất tranh ra trước!).

---

## 6. Lưu ý quan trọng

- **Đừng bấm “Check for updates”** trong app. Cập nhật sẽ tải bản gốc tiếng Trung và ghi đè
  bản tiếng Anh. Muốn lên bản mới thì tải lại bản portable tiếng Anh.
- Vẽ, layer, filter, xuất ảnh/video: **dùng offline bình thường**.
- Đồng bộ cloud, đăng nhập, chia sẻ: cần server của nhà phát triển, có thể không dùng được
  ngoài Trung Quốc.
- Trang đăng nhập WeChat / số điện thoại vẫn là **tiếng Trung** — đó là trang web của hãng,
  cố ý giữ nguyên.

---

## 7. Câu hỏi thường gặp

**Bấm vào mà không thấy gì xảy ra?**
Bạn đang chạy file từ trong cửa sổ nén. Giải nén ra thư mục rồi chạy lại.

**Antivirus báo?**
File `hsjpro_engine.dll` đã được sửa để dịch và fix vùng chọn, nên đôi khi bị nhận nhầm.
Thêm ngoại lệ (exclusion) cho thư mục app là được.

**Máy cần cấu hình gì?**
Windows 10 hoặc 11, 64-bit. Không cần cài thêm gì (Qt, codec, runtime đã đóng gói sẵn).

**Có cần tài khoản không?**
Không. Vẽ offline bình thường, không cần đăng nhập.

**Dùng được bảng vẽ (Wacom, XP-Pen…)?**
Có, app hỗ trợ áp lực bút (pressure).

---

## 8. Miễn trừ trách nhiệm

Đây là bản dịch **không chính thức**, chia sẻ cho mục đích cá nhân. Phần mềm và toàn bộ tài
nguyên (brush, hình ảnh, nội dung) thuộc bản quyền của nhà phát triển gốc. Không bảo hành
dưới bất kỳ hình thức nào.
