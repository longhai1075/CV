# 📦 RELEASE NOTES – Portfolio CV Nguyễn Long Hải

Tài liệu ghi lại lịch sử các phiên bản của dự án Portfolio CV.

---

## [v2.0.0] – 2026-11-25 🚀 Major Release

> **"Professional Upgrade"** — Nâng cấp toàn diện giao diện và nội dung

### ✨ Tính năng mới (Features)

#### Hero Section
- Thêm gradient background với decorative blob animation
- Tên hiển thị gradient màu (xanh → tím)
- Thêm eyebrow dot nhấp nháy (pulse animation)
- Thêm **mini stats bar**: 3+ Dự án · 1+ Năm · 5+ Công nghệ
- Thêm nút thứ 3: "Tải CV" (ghost button)
- Avatar có khung viền gradient + box shadow đẹp

#### Navigation
- Thêm **hamburger menu** cho thiết bị di động
- Animation hamburger → X khi mở/đóng
- **Active nav link** tự động highlight khi cuộn trang
- Đóng menu tự động khi click link (UX cải thiện)

#### Kỹ năng (Skills)
- Thêm **progress bar** với animation khi scroll đến section
- Tách thành 2 cột: Kỹ thuật (bars) | Công nghệ + Mềm (chips)
- Thêm section "Kỹ năng mềm": Làm việc nhóm, Tư duy sáng tạo...
- Mở rộng chip công nghệ: Bootstrap, VS Code, REST API...

#### Học vấn & Kinh nghiệm (Education) — **Mục mới**
- Thêm section `#education` với **vertical timeline**
- 3 mốc thời gian: Sinh viên CNTT → Tự học Frontend → Mục tiêu thực tập
- Timeline dot có icon SVG, màu primary/accent
- Scroll fade-in animation cho từng timeline item

#### Dự án (Projects)
- Thêm **card overlay** với nút "Xem dự án" khi hover
- Thêm **card badge** (Hoàn thành / Nổi bật)
- Thêm **GitHub link** cho mỗi dự án
- Card image có **zoom effect** khi hover
- Cải thiện mô tả dự án 4 (Xe Dream → Trang giới thiệu xe)
- Scroll fade-in animation

#### Liên hệ (Contact)
- Thêm **4 contact info cards** (Email, GitHub, LinkedIn, Phone)
- Icon màu sắc cho từng loại liên hệ
- Thêm **form liên hệ** đầy đủ (tên, email, chủ đề, nội dung)
- Form submit feedback: nút đổi màu xanh "✓ Đã gửi" trong 3s

#### Footer
- Thêm brand mark (logo chữ N) vào footer
- Nút "Lên đầu" có icon SVG, border radius pill

### 🎨 Cải thiện giao diện (UI Improvements)

- Dùng font **Inter** (Google Fonts) thay system-ui
- Mở rộng Design Tokens: thêm `--shadow-sm/md/lg`, `--ease-out`, `--radius-xl`, `--color-success`...
- Thêm `-webkit-font-smoothing: antialiased` cho chữ mượt hơn
- Scroll padding top (72px) để section không bị header che khuất
- Transition và hover effect thống nhất toàn trang

### 📐 Responsive (Điều chỉnh breakpoints)

| Breakpoint cũ | Breakpoint mới | Ghi chú |
|--------------|----------------|---------|
| `768px` | `640px` | Thêm breakpoint tablet nhỏ |
| `768px` | `768px` | Nav ngang, Hero 2 cột |
| *(không có)* | `1024px` | Desktop font scale |
| `1280px` | `1280px` | Giữ nguyên |

### ♿ Accessibility

- `scroll-padding-top: 72px` cho sticky header
- `aria-expanded` đúng trên hamburger button
- `rel="noopener noreferrer"` cho external links
- `aria-label` cho các icon-only buttons

### 🐛 Sửa lỗi (Bug Fixes)

- Xoá DOCTYPE khai báo 2 lần (`<!DOCTYPE html>` trùng lặp ở dòng 1-2)
- Comment `/* box-shadow: var(--shadow); */` không cần thiết đã được dọn dẹp

---

## [v1.0.0] – 2026-11-24 (Phiên bản gốc)

> **"Initial Release"** — Phiên bản đầu tiên do sinh viên tự xây dựng

### Tính năng ban đầu

- ✅ Sticky header với navigation 4 mục
- ✅ Hero section: tên, vai trò, mô tả, 2 nút, avatar
- ✅ Phần kỹ năng: 6 chip (nội dung cơ bản)
- ✅ Phần dự án: 4 card với ảnh, mô tả, tag
- ✅ Phần liên hệ: danh sách text (email, GitHub, LinkedIn)
- ✅ Footer với copyright
- ✅ Responsive cơ bản (768px, 1280px)
- ✅ CSS Design Tokens với Custom Properties
- ✅ Mobile-first approach

### Thư viện & Phụ thuộc

- Không có phụ thuộc ngoài
- Chỉ dùng system font

---

## Lộ trình phát triển (Roadmap)

### [v2.1.0] – Dự kiến
- [ ] Dark mode toggle
- [ ] Thêm section "Chứng chỉ / Certificates"
- [ ] Animation: typing effect cho hero role
- [ ] Back-to-top button smooth scroll

### [v3.0.0] – Dự kiến
- [ ] Chuyển sang React (nếu học)
- [ ] Form liên hệ kết nối EmailJS (gửi email thực)
- [ ] Multi-language (Tiếng Việt / English)
- [ ] PWA (Progressive Web App)

---

*Release notes được cập nhật bởi Nguyễn Long Hải với sự hỗ trợ của AI (Google Antigravity).*

