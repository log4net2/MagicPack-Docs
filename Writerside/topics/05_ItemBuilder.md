# Model Vật Phẩm
## Lưu Ý
- Để thêm được vật phẩm ta cần tệp tin sẽ ở định dạng `.bbmodel` và có thể xem cách chuyển đổi tại mục **BlockBench**
![image_10.png](image_10.png)
## Tạo Thư Mục
- Để thêm model vật phẩm ta tiến hành tạo thư mục trong `plugins/MagicPacks/items` và có thể tạo tự do đảm bảo trong một thư mục sẽ có một tệp `config.yml` và `model.bbmodel`
![image_11.png](image_11.png)
## Tạo Cấu Hình
- Cấu hình sẽ chứa tên model, loại vật liệu và số custom model id
- Tên vật liệu có thể tìm chính xác tại [Bukkit Material](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/Material.html)
- Lưu cấu hình thành `config.yml`, Định dạng đuôi phải là `.yml` nếu khác sẽ không hoạt động được
```yaml 
CustomName: "&fXảng"
Material: DIAMOND_SHOVEL 
CustomModelID: 1
```
![image_12.png](image_12.png)
![image_13.png](image_13.png)
## Ném File BBMODEL
- Khi đã tạo xong cấu hình thì ta ném tệp `.bbmodel` đã xuất ra từ BlockBench lên cùng thư mục chứa `config.yml`
![image_14.png](image_14.png)
## Xây Dựng Gói Pack
- Khi đã ném xong tệp tệp `.bbmodel` lên cùng thư mục với `config.yml` thì ta vào game và chạy lệnh **/magicpack build**
- Ta có thể xem và lấy vật phẩm đó bằng lệnh **/magicpack all**
![image_15.png](image_15.png)
![image_16.png](image_16.png)