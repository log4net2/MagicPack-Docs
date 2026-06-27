# Config Auto Load
- Config Auto Load chỉ áp dụng cho vật phẩm và không áp dụng cho mấy vật phẩm như Giáp, Cung
- Cách hoạt động rất đơn giản, thay vì phải tạo riêng config cho từng vật phẩm thì ta chỉ cần tạo một config chung và ném toàn bộ file `.bbmodel` vào là xong
## Tạo Cấu Hình config Auto Load
- Cấu hình sẽ chứa loại vật liệu và tên loại cấu hình
- Tên vật liệu có thể tìm chính xác tại [Bukkit Material](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/Material.html)
- Lưu cấu hình thành `config.yml`, Định dạng đuôi phải là `.yml` nếu khác sẽ không hoạt động được
Ví Dụ:
```yaml
LoadType: AUTO_LOAD
Material: coal
```
![image_46.png](image_46.png)
## Ném Các File MCModel Lên
- Thứ tự tên của file `.bbmodel` có thể ảnh hưởng đến cách sắp xếp và Custom ID. Ưu tiên dùng lên có số ở trước ví dụ `01_Tên.bbmodel, 02_Tên.bbmodel, 03_Tên.bbmodel`
- Nó sẽ tự tìm Custom ID lớn nhất chưa tồn tại và gán cho model được thêm vào
![image_47.png](image_47.png)

## Xây Dựng Gói Pack
- Khi đã ném xong tệp tệp `.bbmodel` lên cùng thư mục với `config.yml` thì ta vào game và chạy lệnh **/magicpack build**
- Ta có thể xem và lấy vật phẩm đó bằng lệnh **/magicpack all**
![image_48.png](image_48.png)