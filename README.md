# Báo cáo Bài 1: Khởi tạo Local Repository và Cấu hình danh tính

## 1. Khởi tạo Git repository
Lệnh sử dụng:
```bash
git init
```

## 2. Cấu hình danh tính cục bộ
Lệnh sử dụng để cấu hình tên và email cho dự án (sử dụng cờ `--local`):
```bash
git config --local user.name "Duy Ho"
git config --local user.email "duyho@example.com"
```

## 3. Tạo tệp, Add và Commit
Tạo một file text cơ bản, đưa vào vùng chuẩn bị và thực hiện commit:
```bash
New-Item -Path "test.txt" -ItemType File -Value "Initial file"
git add .
git commit -m "Initial commit"
```

## 4. Kết quả kiểm tra lệnh hiển thị cấu hình và lịch sử commit

### Cấu hình hiện tại của repository (`git config --local --list`):
```text
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
user.name=Duy Ho
user.email=duyho@example.com
```

### Lịch sử commit (`git log --oneline`):
```text
e0aaff0 Initial commit
```
