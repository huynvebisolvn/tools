# Tools Dashboard - Ebisol

Bộ công cụ phát triển web được tổ chức trong một dashboard duy nhất.

Link web tools: https://huynvebisolvn.github.io/tools/

## Cấu trúc dự án

```
├── index.html          # Trang chính - Dashboard hiển thị tất cả tools
├── README.md           # Tài liệu hướng dẫn
├── assets/
│   └── style.css       # CSS styling cho dashboard
└── src/
    └── pages/          # Thư mục chứa các tools
        ├── external-api-signature.html
        ├── java-api-sha1.html
        └── ...
```

## Cách sử dụng

1. Mở file `index.html` trong trình duyệt
2. Dashboard sẽ hiển thị tất cả các tools có sẵn trong các cửa sổ riêng biệt
3. Mỗi tool có thể được làm mới hoặc mở trong tab mới

## Cách thêm tools mới

### Bước 1: Tạo file HTML mới
Tạo file HTML cho tool mới trong thư mục `src/`

### Bước 2: Cập nhật danh sách tools
Mở file `index.html` và thêm thông tin tool mới vào mảng `pages`:

```javascript
const pages = [
  { name: 'Tên Tools', path: 'src/ten-file.html'},
  // ... các tools khác
];
```

### Bước 3: Định dạng thuộc tính
- `name`: Tên hiển thị của tool
- `path`: Đường dẫn đến file HTML của tool  

## Ví dụ thêm tool mới

```javascript
{ name: 'Color Picker', path: 'src/color-picker.html'}
```
