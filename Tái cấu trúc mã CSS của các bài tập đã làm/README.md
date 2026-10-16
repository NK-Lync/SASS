# Tái cấu trúc mã CSS bằng SCSS

## 1. Giới thiệu

Dự án thực hiện tái cấu trúc mã CSS của bài tập Website Template sang SCSS nhằm tổ chức mã nguồn rõ ràng, dễ bảo trì và tái sử dụng.

## 2. Công nghệ sử dụng

- HTML5
- CSS3
- SCSS (Sass)
- PowerShell và Visual Studio Code

## 3. Cấu trúc dự án

```text
.
├── index.html
├── README.md
├── css/
│   ├── style.css
│   └── style.css.map
├── images/
├── layout/
│   ├── _header.scss
│   └── _footer.scss
└── scss/
    ├── main.scss
    ├── abstracts/
    │   ├── _variables.scss
    │   └── _mixins.scss
    ├── base/
    │   └── _base.scss
    └── components/
        ├── _navigation.scss
        ├── _products.scss
        └── _statistics.scss
```

## 4. Nội dung tái cấu trúc

- **Variables:** Tập trung các biến màu sắc, phông chữ, khoảng cách và breakpoint.
- **Mixins:** Tái sử dụng các quy tắc Flexbox, container và responsive.
- **Base:** Quản lý các quy tắc CSS cơ bản.
- **Components:** Chia mã giao diện thành các phần điều hướng, dịch vụ và thống kê.
- **Layout:** Tách riêng phần header và footer.
- **main.scss:** Tập hợp các module SCSS bằng `@use`.

## 5. Biên dịch SCSS

Cài đặt hoặc sử dụng Sass trước khi chạy:

```powershell
sass --version
```

Biên dịch SCSS sang CSS:

```powershell
sass .\scss\main.scss .\css\style.css
```

Mở `index.html` trên trình duyệt để xem giao diện.

## 6. Kết quả

Mã nguồn CSS được chia thành các module SCSS, giúp quản lý biến, tái sử dụng quy tắc và tổ chức giao diện dễ dàng hơn.