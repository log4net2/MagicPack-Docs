# Model Cung Tên (2D)
## Lưu Ý
- Để thêm được vật phẩm ta cần tệp tin hình ảnh sẽ ở định dạng ảnh `.png` 
- Với cung tên 2D thì cũng sẽ có 4 trạng thái khác nhau nên ta cũng cần bốn tệp hình ảnh `.png`

| Đuôi File      | Thông Tin                           |
|----------------|-------------------------------------|
| _standby.png   | Là trạng thái cung đứng yên         | 
| _pulling_0.png | Trạng thái cung được kéo căng mức 1 | 
| _pulling_1.png | Trạng thái cung được kéo căng mức 2 | 
| _pulling_2.png | Trạng thái cung được kéo căng mức 3 | 

- Nếu không có đủ model thì có thể copy một trạng thái _standby để tạo 3 trạng thái còn lại!
- Tên của tệp `.png` phải có đuôi là trạng thái của cung. Nếu không thì sẽ bị lỗi model
![image_23.png](image_23.png)

## Tạo Thư Mục
- Để thêm model vật phẩm ta tiến hành tạo thư mục trong `plugins/MagicPacks/items` và có thể tạo tự do
![image_24.png](image_24.png)

## Tạo Cấu Hình
- Cấu hình sẽ chứa tên model, loại vật liệu và số custom model id
- Tên vật liệu có thể tìm chính xác tại [Bukkit Material](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/Material.html)
- Lưu cấu hình thành `config.yml`, Định dạng đuôi phải là `.yml` nếu khác sẽ không hoạt động được
```yaml

CustomName: "&fBow 2D"
Material: bow
CustomModelID: 1
```
![image_19.png](image_19.png)
## Ném File PNG
- Khi đã tạo xong cấu hình thì ta ném bốn tệp hình ảnh `.png` với bốn trạng thái lên cùng thư mục chứa `config.yml`
![image_25.png](image_25.png)
- 
## Xây Dựng Gói Pack
- Khi đã ném xong thì ta vào game và chạy lệnh **/magicpack build**
- Ta có thể xem và lấy vật phẩm đó bằng lệnh **/magicpack all**
![image_26.png](image_26.png)