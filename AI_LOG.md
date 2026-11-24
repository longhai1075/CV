# 🤖 AI_LOG.md – Nhật ký hỗ trợ AI

> Tài liệu này ghi lại toàn bộ quá trình sử dụng AI (Google Antigravity – Gemini) hỗ trợ phát triển dự án Portfolio CV.

---

## Thông tin chung

| Mục | Chi tiết |
|-----|----------|
| **Dự án** | Portfolio CV – Nguyễn Long Hải |
| **Phiên bản** | v2.0.0 |
| **Công cụ AI** | Google Antigravity (Gemini / Claude Sonnet 4.6 Thinking) |
| **Thời gian** | 25/11/2026 |
| **Tổng số phiên** | 1 phiên làm việc |

---

## 📅 Phiên làm việc – 25/11/2026

### Phiên 01 — Nâng cấp toàn diện trang CV

**Thời gian:** 01:13 → 01:38 (giờ Việt Nam)  
**Công cụ AI:** Gemini (chuyển sang Claude Sonnet 4.6 Thinking)  
**Yêu cầu người dùng:** *"Tôi cần trang CV này đẹp, chi tiết và chuyên nghiệp hơn."*

#### Phân tích trước khi thực hiện

AI đọc và phân tích file `index.html` và `assets/css/styles.css` gốc, nhận diện các vấn đề:

| Vấn đề | Mức độ |
|--------|--------|
| Phần kỹ năng liệt kê nội dung không chuyên nghiệp ("chơi game", "đẹp trai"...) | 🔴 Cao |
| Mô tả dự án quá sơ sài ("Dream màu đỏ") | 🔴 Cao |
| Thiếu phần học vấn / kinh nghiệm | 🟡 Trung bình |
| Không có form liên hệ | 🟡 Trung bình |
| Không có hamburger menu mobile | 🟡 Trung bình |
| Chưa có animation / scroll effects | 🟢 Thấp |
| Font mặc định system-ui (chưa có Google Fonts) | 🟢 Thấp |

#### Thay đổi AI đã thực hiện

**`index.html` – Thêm/sửa:**

- ✅ Thêm Google Fonts (Inter) vào `<head>`
- ✅ Thêm hamburger menu button cho mobile
- ✅ Thêm section `#education` với timeline học vấn 3 mốc
- ✅ Hero section: thêm eyebrow dot animation, gradient title, mini stats bar (3+ Dự án, 1+ Năm, 5+ Công nghệ), nút "Tải CV", avatar badge
- ✅ Phần kỹ năng: thay nội dung bằng kỹ năng lập trình thực (HTML/CSS 85%, JS 70%...) với progress bar + skill chips kỹ thuật + kỹ năng mềm
- ✅ Project cards: thêm card-media-wrap, overlay hover, badge, card-footer với link GitHub
- ✅ Mô tả dự án 4 (xe Dream) chuyên nghiệp hơn
- ✅ Contact: thêm 4 contact-card (Email, GitHub, LinkedIn, Phone) và form liên hệ đầy đủ
- ✅ Footer: thêm brand mark, cải thiện layout
- ✅ JavaScript: hamburger toggle, active nav on scroll, skill bar animation, card fade-in, form feedback

**`assets/css/styles.css` – Viết lại hoàn toàn:**

- ✅ Mở rộng Design Tokens (thêm `--color-success`, `--color-chip-soft`, `--shadow-sm/md/lg`, `--ease-out`, `--radius-xl`...)
- ✅ Hamburger menu styles + animation 3 gạch → X
- ✅ Hero blob decorations (CSS pseudo-element)
- ✅ Skill progress bar với CSS custom property `--pct` và transition
- ✅ Timeline component (vertical line, dot, content card)
- ✅ Card overlay hover effect
- ✅ Card badge (absolute position)
- ✅ Contact info cards + form styles
- ✅ Scroll-triggered fade-in animations (`opacity: 0 → 1`)
- ✅ Cải thiện responsive breakpoints (640px, 768px, 1024px, 1280px)

---

### Phiên 02 — Xoá phần "Sẵn sàng thực tập"

**Thời gian:** 01:25 (giờ Việt Nam)  
**Yêu cầu người dùng:** *"Xoá Sẵn sàng thực tập / Phản hồi trong vòng 24 giờ"*

**Thay đổi:**
- ✅ Xoá block `.availability-box` (HTML) gồm badge dot, tiêu đề và mô tả

---

### Phiên 03 — Tạo tài liệu dự án

**Thời gian:** 01:38 (giờ Việt Nam)  
**Yêu cầu người dùng:** *"Viết README.md chuyên nghiệp, hướng dẫn cài đặt/sử dụng. AI_LOG.md, Release note và Evidence index"*

**Thay đổi:**
- ✅ Tạo `README.md` – Hướng dẫn đầy đủ
- ✅ Tạo `AI_LOG.md` – Nhật ký AI (file này)
- ✅ Tạo `RELEASE_NOTES.md` – Lịch sử phiên bản
- ✅ Tạo `EVIDENCE_INDEX.md` – Bảng chứng cứ kỹ thuật

---

## 🔍 Phân tích rủi ro & Quyết định AI

| Quyết định | Lý do |
|-----------|-------|
| Giữ nguyên nội dung dự án gốc (3 dự án web) | Tôn trọng thông tin thực của người dùng |
| Thay kỹ năng "chơi game/đẹp trai" → kỹ năng IT | Phù hợp với ngữ cảnh CV Frontend Developer |
| Dùng Vanilla JS thay vì framework | Phù hợp với level sinh viên, không phụ thuộc build tool |
| Không xoá hình ảnh xe Dream | Chỉ cải thiện mô tả, không thay nội dung |
| Dùng IntersectionObserver cho animation | Hiệu năng tốt hơn scroll event listener |

---

## 📊 Thống kê thay đổi code

| File | Trước | Sau | Thay đổi |
|------|-------|-----|----------|
| `index.html` | 312 dòng | ~600 dòng | +92% |
| `assets/css/styles.css` | 455 dòng | ~700 dòng | +54% |

---

## ✅ Checklist tuân thủ

- [x] AI không tự ý thay đổi thông tin cá nhân (email, tên, lớp)
- [x] AI giữ nguyên cấu trúc thư mục gốc
- [x] AI không cài thêm dependency không được yêu cầu
- [x] AI thực hiện đúng yêu cầu xoá (Availability box)
- [x] Code có comment đầy đủ, dễ đọc
- [x] Không có lỗi HTML validation cơ bản

