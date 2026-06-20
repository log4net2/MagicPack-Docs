# Model Cung Tên (3D)
## Lưu Ý
- Để thêm được vật phẩm ta cần tệp tin sẽ ở định dạng `.bbmodel` và có thể xem cách chuyển đổi tại mục **BlockBench**
- Riêng đối với cung tên thì sẽ có 4 trạng thái khác nhau nên ta cũng cần bốn tệp `.bbmodel`

| Đuôi File        | Thông Tin                           |
|------------------|-------------------------------------|
| _standby.bbmodel | Là trạng thái cung đứng yên         | 
| _pulling_0.bbmodel       | Trạng thái cung được kéo căng mức 1 | 
| _pulling_1.bbmodel       | Trạng thái cung được kéo căng mức 2 | 
| _pulling_2.bbmodel       | Trạng thái cung được kéo căng mức 3 | 

- Nếu không có đủ model thì có thể copy một trạng thái _standby để tạo 3 trạng thái còn lại!
- Tên của tệp `.bbmodel` phải có đuôi là trạng thái của cung. Nếu không thì sẽ bị lỗi model
![image_17.png](image_17.png)

## Tạo Thư Mục
- Để thêm model vật phẩm ta tiến hành tạo thư mục trong `plugins/MagicPacks/items` và có thể tạo tự do
![image_18.png](image_18.png)

## Tạo Cấu Hình
- Cấu hình sẽ chứa tên model, loại vật liệu và số custom model id
- Tên vật liệu có thể tìm chính xác tại [Bukkit Material](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/Material.html)
- Lưu cấu hình thành `config.yml`, Định dạng đuôi phải là `.yml` nếu khác sẽ không hoạt động được
```yaml

CustomName: "&aViên Độc Cung"
Material: bow
CustomModelID: 10
```
![image_19.png](image_19.png)
## Ném File BBMODEL
- Khi đã tạo xong cấu hình thì ta ném bốn tệp `.bbmodel` với bốn trạng thái đã xuất ra từ BlockBench lên cùng thư mục chứa `config.yml`
![image_20.png](image_20.png)
## Xây Dựng Gói Pack
- Khi đã ném xong bốn tệp tệp `.bbmodel` lên cùng thư mục với `config.yml` thì ta vào game và chạy lệnh **/magicpack build**
- Ta có thể xem và lấy vật phẩm đó bằng lệnh **/magicpack all**
![image_21.png](image_21.png)
![image_22.png](image_22.png)