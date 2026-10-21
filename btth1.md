## phần 1. phân tích
- notepad bị đơ vì file 800mb quá lớn, tốn ram.
- cmd ko có lệnh cat nên báo lỗi.
- powershell dùng đc cat vì nó là tên khác của get-content.

## phần 2. lệnh powershell

xem toàn bộ file theo từng dòng
```powershell
Get-Content server_log_800MB.log | Out-Host -Paging
```

xem 10 dòng cuối
```powershell
Get-Content server_log_800MB.log -Tail 10
```
