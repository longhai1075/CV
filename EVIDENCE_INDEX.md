# 📑 EVIDENCE INDEX – Bảng chứng cứ kỹ thuật

> Tài liệu này lập chỉ mục các kỹ thuật, kiến thức và tiêu chí học tập được áp dụng trong dự án **Portfolio CV – Nguyễn Long Hải (KT A2.1)**.  
> Dùng để đối chiếu với rubric/tiêu chí đánh giá môn học.

---

## 1. HTML5 Semantics (Ngữ nghĩa HTML)

| STT | Yếu tố | Vị trí trong code | Mô tả |
|-----|--------|-------------------|-------|
| E01 | `<header>` | `index.html` – dòng 20 | Phần đầu trang với logo và nav |
| E02 | `<nav>` | `index.html` – dòng 28 | Điều hướng chính với `aria-label` |
| E03 | `<main>` | `index.html` – dòng 42 | Nội dung chính trang |
| E04 | `<section>` | `index.html` – dòng 44, 86, 107, 170, 234 | 5 section có `id` anchor |
| E05 | `<article>` | `index.html` – dòng 120, 154, 187, 220 | Thẻ dự án độc lập |
| E06 | `<figure>` | `index.html` – dòng 90 | Ảnh đại diện với ngữ nghĩa |
| E07 | `<footer>` | `index.html` – dòng 296 | Phần cuối trang |
| E08 | `<form>` | `index.html` – dòng 272 | Form liên hệ có `novalidate` |
| E09 | `<label>` | `index.html` – dòng 275, 280, 285, 290 | Label liên kết `for`/`id` |
| E10 | `<button>` | `index.html` – dòng 23 | Hamburger button với ARIA |

---

## 2. CSS Flexbox

| STT | Selector | File – Dòng | Thuộc tính Flexbox | Mục đích |
|-----|----------|------------|---------------------|----------|
| F01 | `.header-inner` | styles.css – dòng ~115 | `display:flex`, `justify-content:space-between`, `align-items:center` | Layout logo + nav ngang |
| F02 | `.nav-list` | styles.css – dòng ~135 | `display:flex`, `flex-direction:row`, `gap` | Danh sách nav ngang |
| F03 | `.hero-inner` | styles.css – dòng ~180 | `display:flex`, `flex-direction:column→row` | Hero 1 cột (mobile) → 2 cột (tablet) |
| F04 | `.hero-actions` | styles.css – dòng ~215 | `display:flex`, `flex-wrap:wrap`, `gap` | Nhóm nút bấm tự xuống dòng |
| F05 | `.hero-stats` | styles.css – dòng ~195 | `display:flex`, `align-items:center`, `gap` | Stats bar căn giữa |
| F06 | `.hero-role` | styles.css – dòng ~175 | `display:flex`, `flex-wrap:wrap`, `align-items:center` | Role text với gap |
| F07 | `.skill-grid` | styles.css – dòng ~300 | `display:flex`, `flex-wrap:wrap`, `gap` | Chip kỹ năng tự xuống dòng |
| F08 | `.skill-bar-list` | styles.css – dòng ~275 | `display:flex`, `flex-direction:column`, `gap` | Danh sách thanh kỹ năng |
| F09 | `.timeline-item` | styles.css – dòng ~325 | `display:flex`, `gap` | Dot + content song song |
| F10 | `.card` | styles.css – dòng ~390 | `display:flex`, `flex-direction:column` | Nội dung card theo cột |
| F11 | `.card-body` | styles.css – dòng ~415 | `display:flex`, `flex-direction:column`, `flex:1` | Body card căng đều chiều cao |
| F12 | `.card-footer` | styles.css – dòng ~440 | `display:flex`, `justify-content:space-between` | Link + GitHub link 2 đầu |
| F13 | `.contact-info` | styles.css – dòng ~465 | `display:flex`, `flex-direction:column`, `gap` | Danh sách contact card |
| F14 | `.contact-card` | styles.css – dòng ~470 | `display:flex`, `align-items:center`, `gap` | Icon + text |
| F15 | `.footer-inner` | styles.css – dòng ~530 | `display:flex`, `flex-wrap:wrap`, `justify-content:space-between` | Footer 3 phần |

---

## 3. CSS Grid

| STT | Selector | File – Dòng | Thuộc tính Grid | Mục đích |
|-----|----------|------------|-----------------|----------|
| G01 | `.project-grid` | styles.css – dòng ~385 | `display:grid`, `grid-template-columns:1fr` → `repeat(2,1fr)` | Grid dự án responsive |
| G02 | `.skills-wrapper` | styles.css – dòng ~260 | `display:grid`, `gap` → `grid-template-columns:1fr 1fr` | 2 cột kỹ năng trên tablet |
| G03 | `.contact-wrapper` | styles.css – dòng ~460 | `display:grid`, `gap` → `grid-template-columns:1fr 1fr` | 2 cột liên hệ trên tablet |
| G04 | `.brand-mark` | styles.css – dòng ~108 | `display:grid`, `place-items:center` | Căn giữa chữ trong logo mark |
| G05 | `.timeline-dot` | styles.css – dòng ~335 | `display:grid`, `place-items:center` | Căn giữa icon trong dot |
| G06 | `.contact-icon` | styles.css – dòng ~480 | `display:grid`, `place-items:center` | Căn giữa icon trong contact |
| G07 | `.card-overlay` | styles.css – dòng ~405 | `display:grid`, `place-items:center` | Căn giữa overlay button |

---

## 4. Responsive Design / Media Queries

| STT | Breakpoint | File – Dòng | Thay đổi áp dụng |
|-----|-----------|------------|------------------|
| R01 | `min-width: 640px` | styles.css – dòng ~600 | 2 cột dự án, 2 cột liên hệ |
| R02 | `min-width: 768px` | styles.css – dòng ~615 | Nav ngang, Hero 2 cột, Skills 2 cột, hamburger ẩn |
| R03 | `min-width: 1024px` | styles.css – dòng ~645 | Font h1 tăng lên 3.5rem |
| R04 | `min-width: 1280px` | styles.css – dòng ~655 | Điều chỉnh project grid |
| R05 | `prefers-reduced-motion` | styles.css – dòng ~665 | Tắt animation cho người dùng nhạy cảm |

---

## 5. CSS Custom Properties (Design Tokens)

| Nhóm | Biến | Giá trị | Mục đích |
|------|------|---------|----------|
| Màu | `--color-primary` | `#2563eb` | Màu xanh chủ đạo |
| Màu | `--color-accent` | `#7c3aed` | Màu tím nhấn |
| Màu | `--color-success` | `#059669` | Màu xanh lá (badge) |
| Font | `--fs-xs` → `--fs-h1` | 0.75rem → 3.5rem | Hệ thống kích thước chữ |
| Spacing | `--space-1` → `--space-6` | 0.5rem → 4rem | Hệ thống khoảng cách |
| Shadow | `--shadow-sm/md/lg` | các giá trị box-shadow | Hệ thống đổ bóng |
| Border | `--radius-sm/radius/lg/xl` | 6px → 28px | Bo góc nhất quán |
| Easing | `--ease-out` | cubic-bezier(0.16,1,0.3,1) | Easing mượt cho animation |

---

## 6. JavaScript / DOM / Web API

| STT | Tính năng | Vị trí | API sử dụng |
|-----|-----------|--------|-------------|
| J01 | Hamburger menu toggle | `index.html` – script | `classList.toggle()`, `setAttribute()` |
| J02 | Đóng menu khi click link | `index.html` – script | `querySelectorAll()`, `addEventListener()` |
| J03 | Active nav on scroll | `index.html` – script | `IntersectionObserver` |
| J04 | Skill bar animation | `index.html` – script | `IntersectionObserver`, `classList.add()` |
| J05 | Card / timeline fade-in | `index.html` – script | `IntersectionObserver`, CSS transition |
| J06 | Form submit feedback | `index.html` – script | `addEventListener('submit')`, `preventDefault()`, `setTimeout()` |

---

## 7. Accessibility (Tiếp cận)

| STT | Kỹ thuật | Vị trí | Mô tả |
|-----|----------|--------|-------|
| A01 | `aria-label` | `<nav>`, `<button>` | Mô tả cho screen reader |
| A02 | `aria-expanded` | Hamburger button | Trạng thái mở/đóng |
| A03 | `aria-hidden="true"` | Icon SVG | Ẩn icon trang trí với screen reader |
| A04 | `:focus-visible` | styles.css – dòng ~660 | Outline khi điều hướng bàn phím |
| A05 | `alt` trên mọi `<img>` | index.html | Mô tả ảnh đầy đủ |
| A06 | Semantic HTML | Toàn trang | `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>` |
| A07 | `scroll-padding-top` | styles.css – dòng ~65 | Tránh header che khuất section khi jump |
| A08 | `rel="noopener noreferrer"` | Các link ngoài | Bảo mật khi mở tab mới |

---

## 8. Hiệu năng (Performance)

| STT | Kỹ thuật | Mô tả |
|-----|----------|-------|
| P01 | `loading="lazy"` | Ảnh tải lười (không bắt buộc, có thể thêm) |
| P02 | `max-width: 100%` trên `img` | Tránh ảnh tràn layout |
| P03 | `IntersectionObserver` | Hiệu năng tốt hơn scroll event listener |
| P04 | CSS `transition` thay JS animation | GPU-accelerated |
| P05 | `transform: translateY()` cho hover | Composite layer, không gây reflow |
| P06 | `will-change` (tiềm năng) | Có thể thêm cho card hover |
| P07 | `preconnect` Google Fonts | Giảm latency tải font |

---

## 9. File Structure & Assets

| File | Kích thước (ước tính) | Mô tả |
|------|----------------------|-------|
| `index.html` | ~20 KB | HTML chính |
| `assets/css/styles.css` | ~18 KB | Toàn bộ CSS |
| `assets/img/*.jpg` | 50-200 KB/file | Ảnh dự án và avatar |

---

## 10. Tự đánh giá

| Tiêu chí | Mức độ đạt | Ghi chú |
|----------|-----------|---------|
| Sử dụng Flexbox | ✅ Xuất sắc | 15+ use case khác nhau |
| Sử dụng CSS Grid | ✅ Xuất sắc | 7 use case, responsive grid |
| Responsive Design | ✅ Xuất sắc | 4 breakpoints, mobile-first |
| HTML Semantic | ✅ Tốt | Dùng đúng thẻ ngữ nghĩa |
| CSS Custom Properties | ✅ Xuất sắc | 20+ biến, hệ thống đầy đủ |
| JavaScript DOM | ✅ Tốt | 6 tính năng interactive |
| Accessibility | ✅ Tốt | ARIA, focus, alt text |
| Code chất lượng | ✅ Tốt | Comment rõ ràng, cấu trúc sạch |

---

*Tài liệu này được tạo ngày 25/11/2026 bởi Nguyễn Long Hải với sự hỗ trợ của AI (Google Antigravity).*

