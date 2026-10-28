# BÀI 1 - PHÂN RÃ YÊU CẦU

## a) Viết 2 Feature

- Feature 1: Đặt suất ăn cho ngày hôm sau
- Feature 2: Quản lý lịch sử đặt và chi phí hàng tháng

## b) Viết 2 User Story

- User Story 1: Là Nhân viên, tôi muốn đặt suất ăn cho ngày hôm sau để không mất thời gian đi xuống trực tiếp canteen.
- User Story 2: Là Nhân viên, tôi muốn xem lịch sử đặt và tổng tiền ăn trong tháng để theo dõi chi phí của mình.

## c) Nêu 1 hạng mục công việc

# BÀI 2- CHẨN ĐOÁN VÀ VIẾT LẠI USER STORY

## Story A

### Tiêu chí INVEST vi phạm rõ nhất

- **Valuable:** Story không nêu rõ người dùng cần thực hiện việc gì và giá trị nghiệp vụ cụ thể nhận được  

### Viết lại

- Là nhân viên, tôi muốn đặt suất ăn trực tuyến trước 9h30, để không phải xuống sảnh ghi tên vào sổ giấy.

## Story B

### Tiêu chí INVEST vi phạm rõ nhất

- **Small:** Story gộp quá nhiều chức năng độc lập nên khó để ước lượng, triển khai và kiểm thử trong 1 Sprint

### Viết lại

- Là Nhân viên, tôi muốn huỷ suất ăn đã đặt trước 9h30 ngày ăn, để không bị tính tiền bữa mình không ăn

# BÀI 3 - VIẾT ACCEPTANCE CRITERIA

| Mã | Given | When | Then |
|---|---|---|---|
| AC-01 | Suất cơm đã được đặt và thời gina trước 9h30 ngày ăn | Nhân viên hủy suất cơm | Hệ thống huỷ thành công và không tính tiền |
| AC-02 | Suất cơm đã được đặt và thời gian đã qua 9h30 ngày ăn | Nhân viên huỷ suất cơm | Hệ thống từ chối huỷ và hiển thị thông báo đã quá giờ huỷ | 
| AC-03 | Chưa có suất cơm nào được đặt | Nhân viên huỷ suất cơm | Hệ thống hiển thị thông báo không tìm thấy suất cơm nào và không thay đổi dữ liệu |

# BÀI 4- ƯU TIÊN VÀ LẬP KẾ HOẠCH SPRINT

## a) MoSCoW

| Mã | Hạng mục | Story Point | MoSCoW |
|:---:|---|:---:|:---:|
| SC-01 | Nhân viên đặt suất ăn cho ngày hôm sau | 5 | Must |
| SC-02 | Nhân viên hủy suất ăn trước giờ chốt | 3 | Must |
| SC-03 | Hành chính xem báo cáo tổng hợp số suất theo món mỗi ngày | 8 | Must
| SC-04 | Nhân viên xem lịch sử đặt và số tiền phải trả trong tháng | 5 | Should |
| SC-05 | Nhân viên đánh giá món ăn sau bữa trưa | 3 | Could |
| SC-06 | Đăng nhập bằng tài khoản nội bộ của công ty | 8 | Must |
| SC-07 | Chia sẻ thực đơn tuần lên fanpage công ty | 2 | Won't |

**Giải trình:**

- SC-01 (Must): Chức năng cốt lõi của hệ thống, giải quyết trực tiếp vấn đề nhân viên phải ghi tên vào sổ giấy và giúp nhân viên ở xa đặt suất ăn
- SC-07 (Won't): Chia sẻ thực đơn tuần chưa cần thiết để triển khai trong phiên bản đầu tiên

## b) Chọn hạng mục đưa vào Sprint kế tiếp

- **Velocity trung bình:** 20 SP
- **Các hạng mục chọn:** SC-01, SC-02, SC-03, SC-05
- **Tổng SP:** 19 SP
- **Căn cứ lựa chọn:** Ưu tiên quy trình đặt và huỷ suất ăn, báo cáo cho hành chính mỗi ngày. SC-05 được thêm vào nếu nhóm còn thời gian để phát triển. Tổng SP nhỏ hơn Velocity trung bình.

## c) Sprint Goal

- Giúp nhân viên chủ động đặt hoặc hủy suất ăn đúng hạn, đồng thời giúp hành chính nắm được số lượng từng món để chuẩn bị bữa trưa chính xác hơn.

## d) Nhận xét tình hình Sprint

**Đến ngày làm việc thứ 5:**
- Đường lý tưởng: 10 SP.
- Đường thực tế: 15 SP.
-> Nhóm đang chậm tiến độ
Nhận xét: Sprint có nguy cơ không hoàn thành Sprint Goal nếu tốc độ xử lý không được cải thiện.
- Hành động cụ thể: SM tổ chức trao đổi ngắn với Developers để xác định các công việc đang bị chậm, thống nhất cách tháo gỡ và rà soát tiến độ hằng ngày, ưu tiên hoàn thành các hạng mục Must trước.