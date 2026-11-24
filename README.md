# 🧑‍💻 Portfolio CV – Nguyễn Long Hải

> Trang CV cá nhân dạng Single-Page Application (SPA) xây dựng hoàn toàn bằng **HTML5 thuần** và **CSS3 thuần**, không phụ thuộc framework hay thư viện ngoài.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📋 Mục lục

- [Giới thiệu](#giới-thiệu)
- [Tính năng](#tính-năng)
- [Cấu trúc thư mục](#cấu-trúc-thư-mục)
- [Cài đặt & Sử dụng](#cài-đặt--sử-dụng)
- [Tuỳ chỉnh nội dung](#tuỳ-chỉnh-nội-dung)
- [Responsive Breakpoints](#responsive-breakpoints)
- [Trình duyệt hỗ trợ](#trình-duyệt-hỗ-trợ)
- [Tác giả](#tác-giả)

---

## Giới thiệu

Dự án **Portfolio CV** là trang web cá nhân dạng một trang (Single Page), được thiết kế để giới thiệu bản thân, kỹ năng, học vấn và các dự án đã thực hiện. Mục tiêu là tạo ra một trang CV trực quan, chuyên nghiệp, dễ tuỳ chỉnh và hoạt động ngay mà **không cần server**.

---

## Tính năng

| Tính năng | Mô tả |
|-----------|-------|
| ✅ Responsive Design | Mobile-first, hỗ trợ 360px → 1440px+ |
| ✅ Sticky Header | Navigation cố định khi cuộn trang |
| ✅ Hamburger Menu | Menu thu gọn trên thiết bị di động |
| ✅ Active Nav | Highlight link nav theo vị trí cuộn |
| ✅ Skill Progress Bar | Thanh tiến trình kỹ năng có animation |
| ✅ Timeline | Phần học vấn & kinh nghiệm theo dòng thời gian |
| ✅ Project Cards | Thẻ dự án với overlay hover effect |
| ✅ Contact Form | Form liên hệ với phản hồi trực quan |
| ✅ Scroll Animations | Fade-in khi cuộn đến phần tử |
| ✅ Smooth Scroll | Cuộn mượt giữa các section |
| ✅ Accessibility | Focus styles, ARIA labels, semantic HTML |
| ✅ Zero Dependencies | Không dùng thư viện ngoài (trừ Google Fonts) |

---

## Cấu trúc thư mục

```
KT A2.1/
│
├── index.html              # File HTML chính (toàn bộ nội dung trang)
│
├── assets/
│   ├── css/
│   │   └── styles.css      # Toàn bộ CSS (design tokens, layout, components)
│   │
│   └── img/
│       ├── 5a7a45214be2cbbc92f3.jpg   # Ảnh đại diện (avatar)
│       ├── DuAn01.jpg                 # Ảnh dự án 1 – Landing Page
│       ├── DuAN02.jpg                 # Ảnh dự án 2 – Todo List
│       ├── DuAn03.jpg                 # Ảnh dự án 3 – Weather Dashboard
│       └── 75f7421e4bddcb8392cc.jpg   # Ảnh dự án 4 – Xe Dream
│
├── README.md               # Tài liệu dự án (file này)
├── AI_LOG.md               # Nhật ký hỗ trợ AI
├── RELEASE_NOTES.md        # Lịch sử phiên bản
└── EVIDENCE_INDEX.md       # Bảng chứng cứ kỹ thuật
```

---

## Cài đặt & Sử dụng

### ▶️ Cách 1 – Mở trực tiếp (nhanh nhất)

```bash
# Clone hoặc tải về dự án
# Sau đó mở file index.html trong trình duyệt
```

1. Tải toàn bộ thư mục `KT A2.1` về máy
2. Mở **File Explorer** (Windows) hoặc **Finder** (macOS)
3. Vào thư mục `KT A2.1`
4. Nhấp đúp vào `index.html` → trang mở ngay trong trình duyệt

> **Lưu ý:** Cách này hoạt động hoàn toàn tốt vì dự án không dùng API hay backend.

---

### ▶️ Cách 2 – Dùng Live Server (VS Code)

Cách này giúp trang tự reload khi bạn chỉnh sửa code — rất tiện khi phát triển.

**Bước 1:** Cài đặt extension **Live Server** trong VS Code

```
Extensions (Ctrl+Shift+X) → Tìm "Live Server" → Install
```

**Bước 2:** Mở thư mục dự án trong VS Code

```bash
# Mở terminal và chạy:
code "KT A2.1"
```

Hoặc: `File → Open Folder → Chọn thư mục KT A2.1`

**Bước 3:** Khởi động Live Server

- Click nút **Go Live** ở thanh dưới cùng VS Code, hoặc
- Chuột phải vào `index.html` → **Open with Live Server**
- Trang sẽ mở tại `http://127.0.0.1:5500`

---

### ▶️ Cách 3 – Dùng Python HTTP Server

```bash
# Di chuyển vào thư mục dự án
cd "KT A2.1"

# Python 3
python -m http.server 8080

# Mở trình duyệt tại:
# http://localhost:8080
```

---

### ▶️ Cách 4 – Deploy lên GitHub Pages (miễn phí)

1. Tạo repository mới trên [GitHub](https://github.com)
2. Upload toàn bộ file dự án lên repo
3. Vào **Settings → Pages → Branch: main → Save**
4. Trang sẽ được deploy tại:
   ```
   https://<username>.github.io/<repo-name>/
   ```

---

## Tuỳ chỉnh nội dung

Toàn bộ nội dung nằm trong `index.html`. Tìm và thay thế các phần sau:

### Thông tin cá nhân (Hero section)

```html
<!-- Dòng ~51: Tên -->
<h1 class="hero-title">Nguyễn Long Hải</h1>

<!-- Dòng ~54: Vai trò -->
<span class="role-static">Frontend Developer</span>

<!-- Dòng ~57-60: Mô tả bản thân -->
<p class="hero-desc">
  Sinh viên ngành Công nghệ thông tin – lớp <strong>CNTT 17-09</strong>. 
  ...
</p>
```

### Ảnh đại diện

```html
<!-- Thay tên file ảnh -->
<img src="assets/img/YOUR_PHOTO.jpg" alt="Ảnh đại diện" ... />
```

### Kỹ năng (progress bar)

```html
<!-- Thay tên kỹ năng và phần trăm -->
<li class="skill-bar-item">
  <div class="skill-bar-label">
    <span>HTML5 / CSS3</span>
    <span class="skill-pct">85%</span>  <!-- % hiển thị -->
  </div>
  <div class="skill-track">
    <div class="skill-fill" style="--pct:85%"></div>  <!-- % thanh bar -->
  </div>
</li>
```

### Màu sắc chủ đạo

Mở `assets/css/styles.css` và chỉnh biến CSS trong `:root`:

```css
:root {
  --color-primary: #2563eb;   /* Màu xanh chính → thay bằng màu bạn thích */
  --color-accent:  #7c3aed;   /* Màu tím nhấn */
}
```

---

## Responsive Breakpoints

| Breakpoint | Màn hình | Thay đổi |
|------------|----------|----------|
| Mặc định   | < 640px  | 1 cột, hamburger menu |
| `≥ 640px`  | Tablet nhỏ | 2 cột dự án, 2 cột liên hệ |
| `≥ 768px`  | Tablet | Nav ngang, Hero 2 cột, Skills 2 cột |
| `≥ 1024px` | Desktop | Font lớn hơn (h1: 3.5rem) |
| `≥ 1280px` | Desktop lớn | 2 cột dự án |

---

## Trình duyệt hỗ trợ

| Trình duyệt | Phiên bản tối thiểu |
|-------------|---------------------|
| Chrome      | 90+ |
| Firefox     | 88+ |
| Safari      | 14+ |
| Edge        | 90+ |
| Opera       | 76+ |

> Tính năng sử dụng: CSS Custom Properties, CSS Grid, Flexbox, IntersectionObserver API, `backdrop-filter`.

---

## Tác giả

**Nguyễn Long Hải**
- 📧 Email: [lhai05577@gmail.com](mailto:lhai05577@gmail.com)
- 🐙 GitHub: [github.com/NguyenLongHai](https://github.com/NguyenLongHai)
- 💼 LinkedIn: [linkedin.com/in/NguyenLongHai](https://linkedin.com/in/NguyenLongHai)
- 🎓 Lớp: CNTT 17-09

---

<p align="center">
  Thiết kế &amp; xây dựng bằng ❤️ &nbsp;·&nbsp; HTML5 + CSS3 + Vanilla JS
</p>

