# Đồ án Vincinema của Nguyễn Duy Thái Sơn

## 1. Tổng quan
**Vincinema** là một ứng dụng đặt vé xem phim online, mang đến cho người dùng khả năng duyệt danh sách các phim đang chiếu, trạng thái đặt vé ở nhiều rạp chiếu phim thuộc hệ thống Vincinema trên toàn quốc và thanh toán, đặt vé tiện lợi.

## 2. Các đối tượng cần được hệ thống mô tả:
- **Khách hàng** (bao gồm tài khoản, số dư và các thông tin cá nhân như tên, tuổi, số điện thoại
- **Phim** (Tên phim, thể loại, thời lượng, miêu tả, ...)
- **Suất chiếu của phim** (Phim gì, ở rạp nào, phòng nào, từ lúc nào đến lúc nào)
- **Rạp chiếu phim** (Tên rạp, địa chỉ)
- **Phòng chiếu phim** (Ở rạp nào, tên phòng, loại phòng, sơ đồ phòng)
- **Sơ đồ phòng chiếu phim** (Số hàng, số cột) (cơ bản)
- **Ghế** (Mã ghế, loại ghế, phòng nào)
- **Lệnh đặt vé** (Suất chiếu nào, ghế nào, thời gian đặt lệnh, ai đặt, giá thành, trạng thái (chưa thanh toán, đã thanh toán, đã hủy...)) (mỗi một vé là 1 lệnh đặt vé, trường hợp mua nhiều thì sẽ có từng ấy lệnh đặt vé)
- **Đồ mua kèm** (Tên (nước ngọt, bỏng ngô, đồ sưu tầm), giá thành, mô tả, đơn vị, trạng thái tồn hàng)
- **Lệnh đặt đồ mua kèm** (Món đồ mua kèm gì, giá thành, ai đặt, thời gian đặt lệnh)

## 3. Các đối tượng trong hệ thống
- **Khách hàng**: là người có như cầu đặt vé xem phim tại bất kì rạp nào thuộc hệ thống Vincinema
- **Vận hành**: là nhân viên làm việc tại hệ thống Vincinema

## 4. Các chức năng của hệ thống
- (Tất cả) **Xem danh sách các phim đang chiếu, suất chiếu và tình trạng đặt chỗ của suất chiếu**
- (Khách hàng) **Đặt vé **
  - Nếu thành công, vé sẽ được thêm vào tài khoản của khách hàng và có thể được sử dụng để xem suất chiếu tương ứng
  - Có thể thất bại nếu như trong lúc khách hàng chờ đặt thì ghế khách hàng chọn đã bị người khác đặt mất, hoặc khách đặt vé quá 15 phút từ lúc phim chiếu
  - Tự hủy nếu sau 30 phút khách không hoàn thành việc thanh toán
- (Vận hành)**Bán vé tại rạp**
  - Chủ yếu để thử nghiệm làm thế nào để đồng bộ thông tin tình trạng đặt chỗ giữa vé bán tại rạp và vé bán trên các nền tảng online
  - Có thể thất bại nếu như trong lúc thao tác bán vé thì ghế đã được người khác chọn và thanh toán mất
- (Khách hàng) **Hủy đặt vé**
  - Nếu thành công, khách hàng sẽ chỉ được hoàn lại phần tiền sau khi đã trừ phí hoàn vé
  - Có thể thất bại nếu như đã quá sát giờ chiếu của suất chiếu
- (Khách hàng) **Xem vé đã đặt**
  - Xem thông tin các vé đã đặt của mình
  - Không thể xem được nếu khách hàng chưa đăng nhập
- (Khách hàng) **Nạp tiền vào hệ thống**
  - Giả lập việc nạp tiền bằng hình thức thẻ cào 

## 5. Use case diagram

![image](https://user-images.githubusercontent.com/94212764/144996249-e23de6bf-4e4f-4420-9b4e-702a8984085f.png)

