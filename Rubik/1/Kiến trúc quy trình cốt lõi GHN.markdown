# Kiến trúc Quy trình Cốt lõi của Giao Hàng Nhanh (GHN)

## 1. Tiếp nhận và xử lý đơn hàng (7 bước)
Quy trình này đảm bảo đơn hàng từ các shop hoặc sàn TMĐT được tiếp nhận và xử lý chính xác trước khi giao.

1. **Thu nhận thông tin đơn hàng**: Tiếp nhận đơn hàng từ shop hoặc sàn TMĐT (Shopee, Lazada, Tiki) qua API hoặc ứng dụng GHN.
2. **Kiểm tra thông tin đơn hàng**: Xác minh tính chính xác của thông tin như địa chỉ, số điện thoại, và mô tả hàng hóa.
3. **Mã hóa và nhập hệ thống**: Gán mã đơn hàng và nhập dữ liệu vào hệ thống quản lý để theo dõi.
4. **Phân loại đơn hàng**: Sắp xếp đơn hàng theo khu vực, loại dịch vụ (nhanh, tiết kiệm, siêu tốc) và mức độ ưu tiên.
5. **Chuyển đơn đến kho**: Gửi đơn hàng đến kho gần nhất để chuẩn bị cho quá trình phân loại và giao hàng.
6. **Cập nhật trạng thái đơn hàng**: Thông báo trạng thái “Đã tiếp nhận” đến shop và khách hàng qua ứng dụng hoặc SMS.
7. **Kiểm tra trước giao**: Đảm bảo đơn hàng được đóng gói đúng quy cách và sẵn sàng chuyển cho bưu tá.

## 2. Giao hàng và thu hộ (COD) (6 bước)
Quy trình này tập trung vào việc giao hàng đến khách và thu tiền hộ (nếu có) một cách an toàn, đúng hẹn.

1. **Nhận đơn từ kho**: Bưu tá nhận danh sách đơn hàng và hàng hóa từ kho để chuẩn bị giao.
2. **Lên kế hoạch giao hàng**: Sắp xếp thứ tự giao dựa trên lộ trình tối ưu được cung cấp bởi hệ thống.
3. **Liên hệ khách hàng**: Gọi điện hoặc nhắn tin xác nhận với khách hàng trước khi giao hàng.
4. **Thực hiện giao hàng**: Giao hàng đến địa chỉ khách hàng, đảm bảo hàng hóa nguyên vẹn.
5. **Thu tiền hộ (COD)**: Thu tiền từ khách hàng (nếu có), kiểm tra số tiền và ghi nhận vào hệ thống.
6. **Cập nhật trạng thái giao hàng**: Ghi nhận trạng thái “Giao thành công” hoặc “Giao không thành công” trên ứng dụng.

## 3. Chăm sóc khách hàng (8 bước)
Quy trình này đảm bảo giải quyết thắc mắc và khiếu nại, nâng cao trải nghiệm khách hàng.

1. **Tiếp nhận yêu cầu**: Ghi nhận thắc mắc hoặc khiếu nại từ khách hàng qua tổng đài, email hoặc ứng dụng.
2. **Xác minh thông tin**: Kiểm tra thông tin đơn hàng và tình trạng giao hàng trên hệ thống.
3. **Liên hệ khách hàng**: Gọi điện hoặc nhắn tin để làm rõ vấn đề và xác nhận nhu cầu của khách.
4. **Xử lý khiếu nại**: Giải quyết các vấn đề như giao sai, giao trễ, hoặc mất hàng theo chính sách GHN.
5. **Cập nhật giải pháp**: Thông báo kết quả xử lý (đền bù, giao lại) đến khách hàng và shop.
6. **Thu thập phản hồi**: Yêu cầu khách hàng đánh giá chất lượng dịch vụ sau khi xử lý.
7. **Lưu trữ dữ liệu**: Ghi nhận toàn bộ thông tin khiếu nại và giải pháp vào hệ thống để phân tích.
8. **Cải tiến dịch vụ**: Phân tích dữ liệu khiếu nại để đề xuất cải tiến quy trình giao hàng và chăm sóc.

## 4. Quản lý kho bãi và phân loại (7 bước)
Quy trình này đảm bảo hàng hóa được lưu trữ, đóng gói và phân loại hiệu quả trước khi giao.

1. **Tiếp nhận hàng hóa**: Nhận hàng từ shop hoặc sàn TMĐT tại kho bãi của GHN.
2. **Kiểm tra hàng hóa**: Xác minh số lượng, chất lượng và tình trạng hàng hóa để đảm bảo không hư hỏng.
3. **Lưu trữ hàng hóa**: Sắp xếp hàng hóa vào kho theo khu vực hoặc loại dịch vụ giao hàng.
4. **Phân loại tự động**: Sử dụng hệ thống phân loại tự động để chia đơn hàng theo lộ trình và điểm đến.
5. **Đóng gói hàng hóa**: Đóng gói hàng hóa theo tiêu chuẩn, đặc biệt với hàng dễ vỡ hoặc cồng kềnh.
6. **Chuyển giao cho bưu tá**: Chuyển hàng hóa đã phân loại đến bưu tá hoặc đội vận chuyển.
7. **Báo cáo kho bãi**: Cập nhật dữ liệu tồn kho và tình trạng phân loại để tối ưu hóa hoạt động.

## 5. Vận hành giao hàng siêu tốc (6 bước)
Quy trình này tập trung vào giao hàng trong 2-4 giờ tại các thành phố lớn.

1. **Tiếp nhận đơn siêu tốc**: Xác nhận đơn hàng yêu cầu giao siêu tốc từ hệ thống hoặc ứng dụng.
2. **Ưu tiên phân loại**: Chuyển đơn siêu tốc đến khu vực xử lý ưu tiên trong kho.
3. **Phân công bưu tá gần nhất**: Gán đơn hàng cho bưu tá ở khu vực gần khách hàng nhất.
4. **Thực hiện giao hàng**: Bưu tá giao hàng trong khung thời gian 2-4 giờ, đảm bảo đúng hẹn.
5. **Cập nhật trạng thái thời gian thực**: Thông báo trạng thái giao hàng cho khách hàng qua ứng dụng hoặc SMS.
6. **Đánh giá hiệu quả**: Ghi nhận thời gian giao và phản hồi khách hàng để cải thiện dịch vụ siêu tốc.

## 6. Kiểm soát chất lượng giao hàng (8 bước)
Quy trình này đảm bảo chất lượng dịch vụ giao hàng đạt tiêu chuẩn và giảm thiểu sai sót.

1. **Xác định tiêu chí chất lượng**: Đặt ra các tiêu chí như tỷ lệ giao hàng thành công, thời gian giao và mức độ hài lòng của khách.
2. **Thu thập dữ liệu giao hàng**: Ghi nhận thông tin từ bưu tá và khách hàng về trạng thái giao hàng.
3. **Phân tích hiệu suất**: Đánh giá tỷ lệ giao thành công, giao trễ, hoặc các trường hợp hoàn hàng.
4. **Xử lý sai sót**: Điều tra và giải quyết các trường hợp giao sai, mất hàng hoặc hư hỏng.
5. **Đền bù theo chính sách**: Thực hiện đền bù (tối đa 50 triệu VNĐ/đơn) nếu lỗi thuộc về GHN.
6. **Đào tạo cải tiến**: Tổ chức đào tạo cho bưu tá hoặc nhân viên kho để giảm sai sót trong tương lai.
7. **Lập báo cáo chất lượng**: Tổng hợp báo cáo định kỳ về chất lượng dịch vụ để báo cáo cho ban quản lý.
8. **Cải tiến quy trình**: Đề xuất thay đổi quy trình hoặc công nghệ dựa trên phân tích dữ liệu chất lượng.