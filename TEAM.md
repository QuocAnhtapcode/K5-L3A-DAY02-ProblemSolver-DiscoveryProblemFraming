# Team — Problem Solver

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: **Problem Solver**
- Candidate problem nhóm chọn (1 câu): Dev/tester mất thời gian mở đúng màn và trạng thái app để chụp ảnh đối chiếu với frame Figma trong báo cáo cho khách hàng.
- Quyết định đề xuất trong báo cáo: **Not Yet** cho triển khai; giữ app/Figma là hướng chính và xác minh dữ liệu, quyền truy cập, khả năng mở màn trước pilot.
- Repo nhóm: [K5-L3A-DAY02-ProblemSolver-DiscoveryProblemFraming](https://github.com/QuocAnhtapcode/K5-L3A-DAY02-ProblemSolver-DiscoveryProblemFraming)

## Thành viên

| STT | Họ và tên         | MSSV        | Vai trò trong nhóm                                                                                              | Tài khoản GitHub                                        |
| --: | ----------------- | ----------- | --------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------- |
|   1 | Hoàng Quốc Anh    | 2A202603707 | Đề xuất 3 candidate: app/Figma, điều tra bug Jira, thủ tục trực tuyến; cung cấp bối cảnh của bài toán được chọn | [QuocAnhtapcode](https://github.com/QuocAnhtapcode)     |
|   2 | Đỗ Thị Thanh Bình | 2A202603709 | Đề xuất 3 candidate: thuế hộ kinh doanh, đăng ký tín chỉ, tìm việc/CV                                           | [ecaep7](https://github.com/ecaep7)                     |
|   3 | Lê Gia Hưng       | 2A202603713 | Đề xuất candidate kiểm soát hàng tồn kho                                                                        | [LeGiaHung29805](http://github.com/LeGiaHung29805)      |
|   4 | Hà Quang Vinh     | 2A202003720 | Đề xuất 2 candidate: tuyển dụng đa nền tảng, biên bản và hỏi–đáp cuộc họp                                       | [hqvinh2210-stack](https://github.com/hqvinh2210-stack) |

## Phân công theo checkpoint — đề xuất để nhóm xác nhận

| Checkpoint                                 | Người chính       | Người hỗ trợ      | Sản phẩm                                                      |
| ------------------------------------------ | ----------------- | ----------------- | ------------------------------------------------------------- |
| CP3 — Hội tụ nhóm                          | Hoàng Quốc Anh    | Cả nhóm           | Rà lại 9 candidate, cluster, OST và bảng điểm đề xuất         |
| CP4 — Kiểm chứng                           | Lê Gia Hưng       | Hoàng Quốc Anh    | Hẹn 2–3 dev/tester ngoài nhóm; ghi snapshot từ buổi hỏi thật  |
| CP4 — Research                             | Đỗ Thị Thanh Bình | Hà Quang Vinh     | Tự kiểm nguồn Figma, Maestro, deep links và điều kiện áp dụng |
| CP5 — Quy trình trước/sau                  | Hoàng Quốc Anh    | Lê Gia Hưng       | Xác nhận luồng mở màn, điều kiện dữ liệu và đo thời gian      |
| CP5 — Problem Statement v0                 | Hoàng Quốc Anh    | Đỗ Thị Thanh Bình | Rà actor, bottleneck, metric và boundary                      |
| CP6 — Mức can thiệp + Problem Statement v1 | Hà Quang Vinh     | Hoàng Quốc Anh    | So sánh 4 mức, chốt eval và phạm vi v1                        |
| CP6 — Quyết định                           | Cả nhóm           | Cả nhóm           | Xác nhận 4 rủi ro, điều kiện pilot và ngưỡng dừng             |

## Cá nhân

### HoangQuocAnh-2A202603707

**Phần việc phụ trách:**

- Chuẩn bị Scan problem và 3 Problem Card về app/Figma, Jira và thủ tục trực tuyến.
- Cung cấp bối cảnh thực tế của báo cáo ảnh app và thông tin 9 candidate/shortlist của nhóm.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Cung cấp trải nghiệm đội dev/tester 6 người mất 2 tuần hoàn thành một đợt báo cáo, xác nhận bước nghẽn là mở đúng màn/trạng thái.
- Xác nhận lựa chọn app/Figma là hướng chính của nhóm; cung cấp thông tin các thành viên và phương án họ đề xuất.
- Phối hợp với AI biên soạn bản nháp báo cáo cá nhân và nhóm; xác nhận nhóm chưa phỏng vấn người ngoài, phần hỏi–đáp trong bản nháp là mô phỏng.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo cá nhân](report/individual/2A202603707_HoangQuocAnh.md): mục 2–3 và nhật ký dùng AI.
- [Báo cáo nhóm](report/team/group_report.md): danh sách 9 candidate, shortlist, bài toán app/Figma và phần trạng thái kiểm chứng.

**Điều mình học được từ phần nhóm:**

- Cần tách thời gian lịch khỏi giờ công, đo theo màn-trạng thái và kiểm phương án Rule trước khi tăng mức tự động hóa.

### LeGiaHung-2A202603713

**Phần việc phụ trách:**

- Chuẩn bị CP1 với 10 problem và CP2 với 3 Problem Card: thông báo học tập bị trôi, phát hiện/xử lý sự cố website và tồn kho đa kênh.
- Pitch ba candidate cá nhân trước khi nhóm hội tụ.
- Phụ trách chính CP4 validation và hỗ trợ CP5 xác nhận quy trình, điều kiện dữ liệu và thời gian từng bước.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Hoàn thiện báo cáo cá nhân CP1–CP2, gồm dấu hiệu thật, metric, phương án không dùng AI và ba quy trình nháp.
- Thống nhất theo quyết định nhóm chọn candidate app/Figma làm hướng chính cho CP3–CP6.
- Chuẩn bị khung phỏng vấn dev/tester về lần gần nhất làm báo cáo ảnh, thời gian từng bước, bottleneck, cách xử lý hiện tại và tín hiệu phản bác.
- Theo dõi lập luận chọn Rule và quyết định Not Yet vì baseline, quyền truy cập và khả năng tái tạo trạng thái chưa được xác nhận đầy đủ.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo cá nhân](report/individual/2A202603713_LeGiaHung.md): mục 2–3, mục 4 và nhật ký dùng AI.
- [Báo cáo nhóm](report/team/group_report.md): mục 3 về trạng thái validation, mục 4–5 về quy trình/Problem Statement và mục 6–8 về mức Rule cùng quyết định Not Yet.

**Điều mình học được từ phần nhóm:**

- Tôi nhận ra một bài toán có nhiều bước chưa chắc cần AI. Cần đo baseline, metric, các dữ liệu thực tế, kiểm tra phương án checklist/Rule và xác nhận rủi ro dữ liệu trước khi chọn mức can thiệp cao hơn.
### DoThiThanhBinh-2A202603709

**Phần việc phụ trách:**

- Người chính: bóc tách quy trình hiện tại (as-is) và tương lai (to-be) cho candidate #1 ở CP5.
- Hỗ trợ: gom cluster và chấm điểm shortlist ở CP3; chia sẻ trải nghiệm và đề xuất giả định cho Assumption Map ở CP4.
- Đọc và nhận xét: Problem Statement v0/v1, mức can thiệp AI và quyết định ở CP6.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch 3 candidate: hộ kinh doanh kê khai thuế (#4), đăng ký tín chỉ (#5), đối chiếu CV với JD (#6); sửa Job Story tín chỉ sau phản biện của nhóm.
- Góp ý cách chia 9 candidate thành 3 cluster và giải thích lý do chia; hỗ trợ các thành viên chấm điểm shortlist theo 7 tiêu chí.
- Chia sẻ trải nghiệm, minh chứng thực tế và đề xuất ý tưởng cho các giả định trong Assumption Map.
- Viết quy trình hiện tại 6 bước kèm actor, input, output, thời gian và bottleneck; quy trình tương lai có điểm kiểm của con người, boundary, phương án quay về; bảng before/after.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md` mục 2.1 (candidate #4–#6), mục 2.2 (cluster), mục 2.4 (bảng chấm điểm).
- `group_report.md` mục 3.1 (Assumption Map).
- `group_report.md` mục 4.1, 4.2, 4.3 (quy trình trước/sau và before/after).

**Điều mình học được từ phần nhóm:**

Tôi nhận ra rằng muốn tạo ra được một sản phẩm thành công, điều đầu tiên cần làm và phải đầu tư nhất là nghiên cứu bài toán phù hợp, tìm hiểu và đưa ra giải pháp sao cho giải quyết đúng được pain của khách hàng, đồng thời phải xem xét, cân nhắc lợi ích và lợi nhuận cho sản phẩm sao cho phù hợp với chiến lược của doanh nghiệp, chứ không chỉ đơn thuần là thấy hay thì triển khai.