# Hướng dẫn sử dụng GIT

Dưới đây là những lệnh git thường dùng

## Lệnh đóng gói những file mới
```sh
git add <tên thư mục cần đóng gói>
```
Ví dụ:
1. Đóng gói tất cả file
```sh
git add .
```
2. Đóng gói 1 file
```sh
git add /html/index.html
```

## Lệnh dán nhãn cho gói đã đóng
```sh
git commit -m "<nội dung nhãn dán>"
```
Ví dụ
```sh
git commit -m "thay đổi file index.html"
```

## Lệnh lấy code từ github về
### Lấy về lần đầu tiên
```sh
git clone <url>
```
Ví dụ: 
```sh
git clone https://github.com/hoainam-99/f8thao.git
```
### Lấy về những lần tiếp theo
1. Lấy về từ nhánh hiện tại
```sh
git pull
```
2. Lấy về từ nhánh khác
```sh
git pull origin <tên nhánh>
```
Ví dụ:
- lấy về từ nhánh master
```sh
git pull origin master
```
- lấy về từ nhánh lhnam
```sh
git pull origin lhnam
```

## Lấy danh sách nhánh
```sh
git branch
```

## Tạo nhánh mới và chuyển nhánh
- Note: sau khi tạo nhánh mới sẽ tự động chuyển sang nhánh mới tạo luôn
```sh
git checkout -b <tên nhánh mới>
```
Ví dụ
```sh
git checkout -b cvthao
```

## Chuyển nhánh đã tồn tại
- Note: tên nhánh có thể lấy từ lệnh git branch
```sh
git checkout <tên nhánh đã tồn tại>
```
Ví dụ
```sh
git checkout cvthao
```

## Đẩy code lên nhánh đang sử dụng
```sh
git push
```

## Cách tạo mới repository
1. Tạo mới 1 repository ở trên github
2. Chạy terminal ở folder muốn đẩy lên github
3. Chạy lệnh theo thứ tự
```sh
git init
git add .
git commit -m "fisrt commit"
git remote add origin <url của repository>
git push -u origin master
```

## Sử dụng github hàng ngày
1. Kéo code từ nhánh chính (master) về vào lần đầu tiên code project trong ngày
```sh
git pull origin master
```

2. Các bước đẩy code đã thay đổi lên github
- Bước 1: Đóng hộp code thay đổi
- Bước 2: Dán nhãn cho hộp code vừa tạo
- Bước 3: Kéo code từ nhánh chính về trước khi đẩy
- Bước 4: Đẩy code lên nhánh đang sử dụng