# Báo cáo nhóm — Day 02 Discovery & Problem Framing

## 1. Thông tin nhóm

- Tên nhóm: **Problem Solver**.
- Thành viên: **Hoàng Quốc Anh, Đỗ Thị Thanh Bình, Lê Gia Hưng, Hà Quang Vinh**. Thông tin và đóng góp đã biết được khai trong [TEAM.md](../../TEAM.md).
- Repo nhóm: [K5-L3A-DAY02-ProblemSolver-DiscoveryProblemFraming](https://github.com/QuocAnhtapcode/K5-L3A-DAY02-ProblemSolver-DiscoveryProblemFraming).
- Candidate problem được chọn: **Dev/tester mất nhiều thao tác để mở đúng màn và trạng thái của app theo thiết kế Figma khi chuẩn bị báo cáo ảnh cho khách hàng.**
- Hướng giải pháp chính: chuẩn hóa liên kết thiết kế ↔ màn/trạng thái app, rồi thử mở màn và chụp ảnh bằng kịch bản cố định; con người kiểm trước khi bàn giao.
- Mức can thiệp đề xuất: **Rule**; chỉ xét Workflow có AI khi phép thử cho thấy Rule chưa đủ.
- Quyết định đề xuất: **Not Yet — giữ hướng chính, kiểm chứng điều kiện triển khai trước pilot.**

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch — 9 candidate

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện luyện tập |
|---:|---|---|---|---|---|
| 1 | Hoàng Quốc Anh | Khi cần báo cáo ảnh app để đối chiếu Figma, tôi muốn mở đúng màn/trạng thái theo thiết kế, để lấy đủ ảnh chính xác mà không phải tìm lại nhiều lần. | Dev, tester | Mở đúng màn/trạng thái | Mỗi màn cần qua bao nhiêu thao tác? Hai tuần gồm bao nhiêu giờ thực làm và bao nhiêu thời gian chờ? |
| 2 | Hoàng Quốc Anh | Khi nhận ticket bug Jira trong source lớn, tôi muốn khoanh vùng luồng xử lý và vị trí code có căn cứ, để bắt đầu sửa đúng chỗ. | Dev nhận ticket | Lần từ triệu chứng đến module/file/hàm | Mất thời gian ở tái hiện, tìm code hay kiểm giả thuyết? Ticket và công cụ tìm kiếm hiện tại đã đủ chưa? |
| 3 | Hoàng Quốc Anh | Khi làm thủ tục đóng phạt trực tuyến mà hướng dẫn chưa rõ, tôi muốn biết cần chuẩn bị gì và đi tiếp thế nào, để hoàn thành đúng cách. | Người tự làm thủ tục | Hiểu rõ quy trình, biết được mình cần làm bước nào trước | Vướng cụ thể ở bước nào? Một hướng dẫn rõ theo bước đã đủ chưa? |
| 4 | Đỗ Thị Thanh Bình | Khi đến kỳ kê khai thuế, tôi muốn biết cần chuẩn bị thông tin và hồ sơ gì cho hộ kinh doanh của mình, để kê khai đầy đủ và giảm số lần bổ sung. | Chủ hộ kinh doanh nhỏ ở Việt Nam | Xác định yêu cầu và đối chiếu hồ sơ | Lần kê khai gần nhất gặp lỗi gì? Có người dùng thật và nguồn chính thức cho đúng trường hợp không? |
| 5 | Đỗ Thị Thanh Bình | Khi đăng ký tín chỉ cho kỳ tới, tôi muốn chọn các môn còn thiếu, đủ điều kiện và không trùng lịch, để tiến gần kế hoạch tốt nghiệp sớm. | Sinh viên | Đối chiếu môn còn thiếu, tiên quyết và lớp đang mở | Vướng ở xác định môn cần học hay thiếu chỗ? Những ràng buộc nào là cố định? |
| 6 | Đỗ Thị Thanh Bình | Khi ứng tuyển, tôi muốn biết kinh nghiệm thật của mình đáp ứng yêu cầu nào trong JD, để trình bày CV phù hợp và thấy phần còn thiếu. | Người tìm việc | Đối chiếu kinh nghiệm với yêu cầu | Đo “phù hợp” bằng gì? Làm sao không thêm kinh nghiệm không có thật? |
| 7 | Lê Gia Hưng | Khi kiểm tra tồn kho trước khi bán hoặc nhập hàng, tôi muốn biết số lượng thực tế và mặt hàng sắp thiếu/dư, để hạn chế bán vượt tồn và nhập sai. | Người quản lý kho/cửa hàng | Đối chiếu giao dịch với tồn thực tế | Sai lệch ở nhập, xuất hay kiểm đếm? Đã có dữ liệu nhất quán để áp dụng quy tắc chưa? |
| 8 | Hà Quang Vinh | Khi tuyển một vị trí từ nhiều nền tảng, tôi muốn đối chiếu và sàng lọc hồ sơ theo tiêu chí thống nhất, để tìm ứng viên phù hợp mà không xử lý trùng. | HR, quản lý tuyển dụng | Gom hồ sơ, loại trùng và so tiêu chí | Có quyền dùng dữ liệu từ nền tảng nào? Ai xác định tiêu chí và quyết định cuối? |
| 9 | Hà Quang Vinh | Khi cần kiểm tra nội dung sau cuộc họp, tôi muốn tra được điều đã nói, quyết định và căn cứ trong bản ghi, để trả lời câu hỏi mà không nghe lại toàn bộ. | Nhân viên tham gia họp | Tìm đúng đoạn trong bản ghi/biên bản | Nhu cầu chính là ghi biên bản hay hỏi đáp? Có bản ghi được phép dùng và cách kiểm câu trả lời theo nguồn không? |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Tìm đúng vị trí/ngữ cảnh trong công việc phần mềm | #1 App/Figma; #2 Jira/source code | Đã biết kết quả cần đạt nhưng mất thời gian lần đến đúng màn, trạng thái hoặc vị trí xử lý |
| B — Đáp ứng điều kiện và hoàn thiện hồ sơ | #3 Thủ tục trực tuyến; #4 Thuế; #5 Tín chỉ; #6 CV/JD | Đối chiếu thông tin hiện có với yêu cầu trước khi hoàn thành một việc |
| C — Đối chiếu dữ liệu vận hành và tra cứu | #7 Tồn kho; #8 Tuyển dụng; #9 Biên bản/hỏi đáp họp | Thông tin chưa được tổ chức đủ để tra cứu và ra quyết định nhất quán |

Cluster giúp thấy pattern, không có nghĩa các candidate cần cùng một giải pháp. Cây OST sau tập trung vào outcome của candidate #1 để giữ phạm vi đủ hẹp.

### 2.3. Opportunity Solution Tree rút gọn

```text
OUTCOME: Giảm ít nhất 50% thời gian thực làm trên mỗi màn-trạng thái-thiết bị
         khi chuẩn bị báo cáo ảnh, đồng thời giữ đủ và đúng ảnh theo phạm vi đã chốt.
├── Opportunity A: Mất thời gian mở đúng màn và trạng thái cần chụp.
├── Opportunity B: Thông tin để tái tạo trạng thái chưa được mô tả đầy đủ.
└── Opportunity C: Dễ lẫn phiên bản, trạng thái hoặc cặp ảnh khi bàn giao.
```

### 2.4. Chấm điểm shortlist (1–5)

Shortlist theo lựa chọn nhóm: **#1 App/Figma, #2 Jira, #9 Biên bản và hỏi đáp họp**. Mỗi tiêu chí tối đa 5, tổng tối đa 35, trọng số bằng nhau. Bảng điểm là đề xuất theo thông tin hiện có để nhóm chốt bằng lập luận.

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #1 — Mở đúng màn/trạng thái app theo Figma | 5 | 5 | 3 | 4 | 5 | 5 | 3 | **30** |
| #2 — Khoanh vùng code từ ticket Jira | 5 | 4 | 3 | 3 | 3 | 5 | 3 | **26** |
| #9 — Biên bản và hỏi đáp cuộc họp | 4 | 4 | 1 | 2 | 4 | 5 | 2 | **22** |

**Candidate được chọn:** #1 — mở đúng màn/trạng thái app theo Figma để phục vụ báo cáo ảnh.

**Vì sao chọn:** đây là hướng chính nhóm đã chốt; so với hai candidate còn lại, phép thử nhỏ rõ hơn, đúng/sai kiểm được và có phương án không dùng AI làm mốc so sánh.

**Vì sao chưa chọn hai candidate còn lại:** #2 cần thêm dữ liệu và quyền hệ thống để kiểm nguyên nhân bug; #9 cần xác nhận nhu cầu và quyền sử dụng bản ghi. Hai hướng được giữ cho vòng discovery tiếp theo.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Dev/tester ngoài nhóm cũng mất đáng kể thời gian mở đúng màn/trạng thái khi làm báo cáo ảnh. | Value | 5 | 4 | Có, Quốc Anh từng làm việc này |
| 2 | Mở đúng màn/trạng thái chiếm tỷ trọng lớn trong thời gian thực làm, không phải chờ build/dữ liệu. | Value | 5 | 3 | Có, bấm giờ từng bước trên 10 trường hợp |
| 3 | Các trạng thái mục tiêu tái tạo được bằng dữ liệu test và thao tác/kịch bản ổn định. | Feasibility | 5 | 3 | Có, kiểm trên một nền tảng |
| 4 | Setup và bảo trì ánh xạ/kịch bản tốn ít hơn thời gian tiết kiệm qua các đợt báo cáo. | Feasibility | 5 | 1 | Có, ghi riêng rồi tính lợi ích ròng |
| 5 | Tester kiểm nhanh được ảnh đúng màn/trạng thái và phát hiện sai trước khi bàn giao. | Usability | 4 | 2 | Có, quan sát bước review và chấm eval |
| 6 | Nhóm có quyền dùng thiết kế, build và dữ liệu test trong môi trường phù hợp. | Viability | 5 | 1 | Có, xác nhận quyền trước pilot |

### 3.2. Kiểm chứng và bộ hỏi–đáp luyện tập

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Điều chưa biết / phản chứng cần tìm |
|---|---:|---|---|
| Trải nghiệm một thành viên làm công việc dev/tester | 1 nguồn; một đợt báo cáo | Đội 6 người tham gia, đợt báo cáo kéo dài 2 tuần; Quốc Anh xác nhận vướng nhất ở mở đúng màn/trạng thái | Chưa biết giờ công, tần suất báo cáo và tỷ trọng thời gian chờ |

**Bộ hỏi đáp mô phỏng bằng AI để luyện phản biện, câu trả lời là giả định thảo luận.**

| # | Góc phản biện | Câu hỏi | Câu trả lời dự kiến để luyện tập |
|---:|---|---|---|
| 1 | PM hoài nghi | Vì sao chọn bài này thay vì Jira hoặc biên bản họp? | Actor, đầu ra và bước nghẽn của bài app/Figma cụ thể hơn; có thể thử trên 10 trường hợp. Chưa kết luận hai bài kia ít giá trị hơn khi có thêm dữ liệu. |
| 2 | Tester | Làm sao biết bottleneck là mở màn chứ không phải đối chiếu ảnh? | Quốc Anh xác nhận vướng ở mở màn/trạng thái; để kiểm tỷ trọng cần bấm giờ riêng từng bước, không dùng 2 tuần làm bằng chứng định lượng cho một bước. |
| 3 | Dev | Figma có cho biết đường đi trong app không? | Frame mô tả giao diện đích, chưa đủ chỉ ra đường đi và dữ liệu. Cần ánh xạ đã được dev/tester kiểm, không suy đoán route chỉ từ hình ảnh. |
| 4 | PM hoài nghi | Nếu checklist đã đủ thì vì sao phải dùng AI? | Có thể không cần AI. So checklist chuẩn hóa trước; chỉ thêm Rule khi thao tác lặp vẫn tốn thời gian, chỉ xét Workflow khi Rule còn thiếu và có bằng chứng. |
| 5 | Tester | Màn nhìn giống nhau nhưng khác trạng thái thì xử lý thế nào? | Mỗi mục phải có điều kiện dữ liệu, trạng thái và tiêu chí xác nhận riêng; tester kiểm ảnh trước khi đánh dấu hoàn tất. |
| 6 | Dev vận hành | App thay đổi thì công sức bảo trì có vượt phần tiết kiệm không? | Phải ghi setup và bảo trì, tính lợi ích ròng qua các đợt; nếu không còn lợi ích thì quay về checklist. |
| 7 | Người phụ trách dữ liệu | Kịch bản có thể chạm dữ liệu thật hoặc giao dịch không? | Phạm vi chỉ dùng môi trường/tài khoản/data được duyệt; thao tác có tác động ngoài phạm vi là điều kiện dừng. |
| 8 | Người chấm | Đã đủ bằng chứng để Go chưa? | Chưa. Hướng chính đã chọn nhưng chưa kiểm với người ngoài nhóm, chưa đo baseline và chưa xác nhận khả năng tái tạo trạng thái; kết luận hiện tại là Not Yet. |

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link chính thức | Giải bước nào? | Nội dung nguồn xác nhận | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Figma REST API — file endpoints | [File endpoints](https://developers.figma.com/docs/rest-api/file-endpoints/) | Bước 1: xác định frame/node và ảnh thiết kế cần đối chiếu | Có endpoint đọc file/node theo ID và render ảnh node | Suy luận của nhóm: dữ liệu thiết kế không tự cho biết route hoặc trạng thái app đang chạy | Giữ ID/version thiết kế và ánh xạ sang screen/state đã được người có ngữ cảnh kiểm |
| Maestro — openLink và takeScreenshot | [openLink](https://docs.maestro.dev/reference/commands-available/openlink), [takeScreenshot](https://docs.maestro.dev/reference/commands-available/takescreenshot) | Bước 2–3: mở đường dẫn và chụp ảnh trong kịch bản | Tài liệu mô tả lệnh mở URL/deep link và lưu ảnh PNG | Cần app hỗ trợ đường vào, tài khoản/dữ liệu và thao tác đúng; không chứng minh tự suy route từ ảnh Figma | Thử công cụ có sẵn cho kịch bản cố định trước khi nghĩ đến xây Agent |
| Android Developers — deep links | [Create deep links](https://developer.android.com/training/app-links/create-deeplinks) | Pattern mở đúng vị trí trong app ở bước 2 | App Android cần cấu hình intent filter phù hợp để nhận URI tương ứng | Chỉ áp dụng nếu nền tảng là Android và app thực sự hỗ trợ; hiện chưa biết app của nhóm có điều kiện này | Kiểm khả năng mở trực tiếp trước; nếu không có, thử đường đi bằng thao tác cố định |

**Kết luận research:** công cụ có sẵn hỗ trợ lấy thiết kế và chạy thao tác/chụp ảnh, nhưng chưa lấp được khoảng trống đặc thù là ánh xạ đúng frame → màn/trạng thái → đường đi → dữ liệu test.

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

```text
HIỆN TẠI — ƯỚC LƯỢNG 30 PHÚT / TRƯỜNG HỢP

[1 Xác định màn/trạng thái và bản thiết kế: 5']
→ [2 Mở app đến đúng màn/trạng thái: 15'] ← BOTTLENECK
→ [3 Chụp + lưu ảnh: 1']
→ [4 Đối chiếu ảnh app với thiết kế: 3']
→ [5 Ghép ảnh + ghi nhận khác biệt: 4']
→ [6 Kiểm tra đủ/đúng + bàn giao: 2']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú / handoff |
|---:|---|---|---|---|---|
| 1 | Dev/tester nhận yêu cầu | Danh sách cần báo cáo, bản thiết kế và phiên bản app | Màn/trạng thái/cấu hình được chọn | Ước lượng 5 phút/trường hợp | Chốt đầu vào trước khi điều hướng |
| 2 | Dev/tester lấy ảnh | Mục tiêu, tài khoản và điều kiện dữ liệu | App ở đúng màn/trạng thái | Ước lượng 15 phút/trường hợp | Bottleneck đã xác nhận về bản chất; chưa bấm giờ |
| 3 | Dev/tester lấy ảnh | App ở trạng thái mục tiêu | Ảnh có định danh | Ước lượng 1 phút/trường hợp | Chuyển ảnh cho người đối chiếu |
| 4 | Tester/người đối chiếu | Ảnh app và đúng thiết kế | Kết quả đối chiếu, ghi chú | Ước lượng 3 phút/trường hợp | Con người xác nhận khác biệt, không tự coi mọi khác biệt là bug |
| 5 | Người tổng hợp | Cặp ảnh và ghi chú | Mục báo cáo hoàn chỉnh | Ước lượng 4 phút/trường hợp | Chuyển bản nháp để review |
| 6 | Người chịu trách nhiệm báo cáo | Danh sách và báo cáo | Báo cáo được duyệt/bàn giao | Ước lượng 2 phút/trường hợp | Quay lại bước trước nếu sai/thiếu |

**Bottleneck chính:** bước 2. Cần đo số thao tác, điều kiện dữ liệu, số lần quay lại và thời gian chờ để hiểu nguyên nhân trong bước này.

### 4.2. Quy trình tương lai

Trước mỗi đợt, xác nhận bảng ánh xạ: **frame/design version → screen ID → trạng thái → điểm vào/đường đi → tài khoản/dữ liệu test → ảnh cần có**. Tạo/bảo trì bảng và kịch bản là chi phí thiết lập riêng.

```text
TƯƠNG LAI — MỤC TIÊU MINH HỌA 15 PHÚT / TRƯỜNG HỢP

[1 Người chọn mục tiêu từ ánh xạ đã kiểm: 3']                  ← CON NGƯỜI
→ [2 Kịch bản mở đúng màn/trạng thái: 3']                      ← RULE
→ [3 Chụp + đặt tên/lưu ảnh theo cấu hình: 1']                 ← RULE
→ [4 Tester kiểm màn/trạng thái + đối chiếu thiết kế: 3']      ← CON NGƯỜI, ĐIỂM KIỂM
→ [5 Người ghép ảnh + ghi nhận vào mẫu báo cáo: 3']            ← CON NGƯỜI
→ [6 Người duyệt đủ/đúng rồi bàn giao: 2']                      ← CON NGƯỜI

Bước 2/3 thất bại hoặc ảnh sai → dừng trường hợp, ghi log, quay về chụp thủ công;
```

**Boundary:** chỉ thao tác build/môi trường, tài khoản và dữ liệu được phép; chỉ chuẩn bị trạng thái bằng thao tác đã duyệt. Không tạo giao dịch thật, xóa dữ liệu, sửa code/design, tự kết luận giao diện đạt hoặc tự gửi báo cáo. Nếu sau này thêm AI, AI cũng không được tự đổi đường đi khi thiếu căn cứ hoặc vượt quyền này.

**Phương án quay về:** dùng danh sách và cách chụp thủ công hiện tại; giữ ảnh đã kiểm, chụp lại ảnh không đạt; cập nhật ánh xạ/kịch bản sau khi xác nhận nguyên nhân. Trường hợp chưa mở được ghi “chưa hoàn tất”.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 6 | 6 | Giữ nguyên |
| Tổng thời gian thực làm/trường hợp | 30 phút, minh họa | 15 phút, mục tiêu minh họa | Giảm 50% |
| Thời gian mở đúng màn/trạng thái | 15 phút, minh họa | 3 phút, mục tiêu minh họa | Giảm 80%; target đánh giá tối thiểu là giảm 50% so baseline thực đo |
| Số bước thủ công | 6/6 | 4/6 | Bước 2–3 người vẫn kiểm và bàn giao |
| Bottleneck chính | Mở đúng màn/trạng thái | Chưa kết luận trước khi đo | Không mặc định chuyển sang bước khác |
| Rủi ro mới | Có thể sai/thiếu ảnh khi làm tay | Ánh xạ cũ, script hỏng, ảnh sai nhưng tên đúng | Tester kiểm từng ảnh, fallback khi lỗi |
| Setup/bảo trì | Chưa có số liệu riêng | Có chi phí tạo/kiểm ánh xạ và kịch bản | Ghi riêng và phân bổ vào thời gian các đợt |

**Lợi ích ròng một đợt** = thời gian cách cũ − (thời gian cách mới + setup phân bổ + bảo trì + xử lý lỗi).

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Dev/tester phụ trách lấy ảnh app để làm báo cáo đối chiếu thiết kế cho khách hàng. |
| **Quy trình** | Xác định màn/trạng thái → mở app → chụp ảnh → đối chiếu thiết kế → ghép báo cáo → kiểm và bàn giao. |
| **Bottleneck** | Mở đúng màn/trạng thái là điểm vướng đã xác nhận. |
| **Impact** | Một đợt có đội 6 người tham gia kéo dài 2 tuần. |
| **Success Metric** | Đo baseline trên 10 trường hợp cùng phạm vi; mô hình 30 phút/trường hợp chỉ minh họa. Target đề xuất: giảm ít nhất 50% thời gian thực làm, vẫn đủ ảnh đúng phạm vi. Bấm giờ theo bước, ghi chờ và số ảnh phải làm lại. |
| **Boundary** | Chỉ dùng môi trường/dữ liệu được phép; không giao dịch thật hoặc sửa code/design; người chịu trách nhiệm kiểm ảnh và duyệt trước khi gửi. |

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Phạm vi đã thu hẹp có **độ mơ hồ thấp, độ phức tạp trung bình**: màn/trạng thái đích định trước và ảnh đúng/sai kiểm được; có nhiều bước/điều kiện nhưng có thể mô tả thành kịch bản nếu app hỗ trợ. Cần kiểm giả định tái tạo trạng thái. Figma thể hiện giao diện đích, không tự chứng minh đường đi và dữ liệu trong app.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** | Checklist, hướng dẫn đường đi, dữ liệu test và mẫu ảnh/báo cáo | Ít màn, ít lặp hoặc chủ yếu thiếu hướng dẫn | Vẫn phải điều hướng lặp; hướng dẫn có thể cũ | Mốc so sánh và phương án quay về |
| **Rule** | Ánh xạ đã kiểm + kịch bản mở trạng thái + chụp/lưu ảnh cố định | Đường đi và dữ liệu tái tạo ổn định | Script/ánh xạ hỏng khi app đổi; setup/bảo trì | **Mức đề xuất hiện tại** |
| **Workflow** | AI đề xuất cặp frame–screen/đường đi có nguồn → người duyệt → kịch bản mở/chụp → tester kiểm | Có bằng chứng mapping thủ công vẫn là pain và Rule không đủ | Ghép sai frame, suy đoán trạng thái, tăng công kiểm | Chỉ xét lại sau so sánh No AI/Rule |
| **Agent** | AI tự khám phá giao diện, chọn thao tác để đến đích | Đường đi chưa biết trước, môi trường kiểm soát được và Workflow đã được chứng minh không đủ | Đi sai luồng, tác động dữ liệu, khó lặp lại | Chưa có căn cứ chọn |

**Mức chọn:** Rule là giả thuyết đơn giản nhất cho phép thử; chưa triển khai rộng.

**Vì sao không chỉ chọn mức đơn giản hơn:** checklist có thể giảm tìm thông tin nhưng vẫn giữ thao tác điều hướng/chụp lặp lại. Cần so Rule với checklist đã chuẩn hóa; nếu checklist đã đạt target hoặc Rule không có lợi ích ròng thì chọn No AI.

**Vì sao chưa chọn mức cao hơn:** chưa có bằng chứng phải dự đoán/tạo nội dung để mở các trạng thái cố định. Bắt đầu từ Figma không tự đồng nghĩa cần AI; nhiều bước không tự đồng nghĩa cần Agent.

### 6.3. AI Canvas rút gọn

**Không áp dụng cho mức Rule**, theo ngoại lệ trong worksheet CP6 và rubric C10. Đầu ra là đúng màn/trạng thái theo danh sách; nếu điều kiện được xác định thì có thể mã hóa, không có bước AI dự đoán/tạo nội dung.

Dữ liệu của phép thử Rule gồm build, cấu hình thiết bị, frame/version, ánh xạ đã kiểm và tài khoản/data test. Hành động là chạy đường đi/chụp; outcome là thời gian ròng và ảnh đúng/đủ; feedback là lỗi tester ghi để sửa ánh xạ/kịch bản. Nếu thử Workflow ở vòng sau phải điền AI Canvas riêng và chứng minh giá trị tăng thêm.

### 6.4. Hai câu hỏi của Google PAIR

Không áp dụng như câu trả lời về AI cho phương án đang chọn. Con người vẫn kiểm và bàn giao; chưa có phỏng vấn để kết luận người dùng muốn augment hay automate.

Với Rule, lỗi cần ưu tiên ngăn là **ảnh sai màn/trạng thái bị đánh dấu hoàn tất**. Tester đối chiếu ảnh với mục tiêu, không chỉ kiểm tên file. Mục chưa chắc phải giữ trạng thái “chưa hoàn tất” và xử lý thủ công.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Dev/tester lấy ảnh đối chiếu thiết kế cho một app trong môi trường test được phép; pilot một nền tảng và 10 màn-trạng thái-cấu hình. |
| **Quy trình** | Chọn mục tiêu từ ánh xạ đã kiểm → mở bằng kịch bản → chụp/lưu → tester kiểm trạng thái và đối chiếu → tổng hợp → người duyệt/bàn giao. |
| **Bottleneck** | Mở đúng màn/trạng thái; mô hình 15 phút ở bước này chưa bấm giờ. Cần tách điều hướng, dữ liệu, quyền và chờ. |
| **Impact** | Bằng chứng hiện có là một đợt kéo dài 2 tuần có 6 người tham gia, chưa suy ra giờ công. Đo thực làm, số lần mở/chụp lại, setup/bảo trì để lượng hóa. |
| **Success Metric** | Đo baseline thủ công trên 10 trường hợp; target giảm ít nhất 50% trung vị thời gian mở trạng thái và 50% tổng thời gian thực làm trên cùng phạm vi, kể cả setup/bảo trì phân bổ. 100% mục báo cáo hoàn tất có ảnh đúng màn/trạng thái/phiên bản theo người kiểm; không bỏ ca thất bại. Mô hình 30 → 15 phút chỉ minh họa target. |
| **Boundary** | Chỉ dùng tài khoản/data/môi trường được duyệt; không giao dịch thật, xóa dữ liệu, sửa code/design hoặc tự gửi báo cáo. Tester kiểm từng ảnh; lỗi/chưa chắc thì dừng và quay về thủ công. |
| **AI intervention point** | **Không có** trong phương án Rule; chưa có bằng chứng cần AI để giải bottleneck. Nếu nâng mức phải xác định điểm can thiệp và eval mới. |
| **Mức chọn** | **Rule**, so với baseline No AI đã chuẩn hóa. |
| **Rủi ro & người kiểm tra** | Dev kiểm kịch bản và khả năng tái tạo; tester kiểm từng ảnh; người phụ trách báo cáo duyệt trước bàn giao. Nhóm cần xác nhận người nhận vai trong TEAM.md. Rủi ro: ánh xạ cũ, thiếu data test, bảo trì cao, ảnh sai bị coi là đạt. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Actor/phạm vi | Dev/tester làm báo cáo nói chung | Một app, một nền tảng, 10 trường hợp có đầu vào được duyệt | Giảm biến số, làm phép thử nhỏ |
| Quy trình | Thao tác hiện tại | Điểm dùng Rule và điểm kiểm con người | Kiểm được ai làm gì, khi nào quay về |
| Success Metric | Thời gian và đủ ảnh | Thêm đúng trạng thái/version, không bỏ ca lỗi, setup/bảo trì | Tránh nhanh hơn nhờ bỏ việc hoặc chuyển chi phí sang chuẩn bị |
| Mức/rủi ro | Chưa chọn công nghệ | Rule; không có AI intervention; nêu vai kiểm | Chọn mức đơn giản trước, không chọn AI theo tên ý tưởng |

**Tiêu chí đánh giá giải pháp Rule — 5 tiêu chí:**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đúng màn, trạng thái, phiên bản | Mọi ảnh đánh dấu hoàn tất khớp mục tiêu theo tester kiểm | Có ảnh sai nhưng vẫn được đánh dấu đạt |
| 2 | Đủ phạm vi và truy nguyên | Cả 10 mục có trạng thái đạt/chưa đạt; ảnh truy được frame, build, cấu hình | Thiếu mục, ghép nhầm hoặc bỏ ca lỗi khỏi kết quả |
| 3 | Lợi ích thời gian | Đạt target 50% so baseline cùng phạm vi sau chi phí phân bổ | Không đạt hoặc bỏ setup/điểm kiểm khỏi phép tính |
| 4 | Hỏng có kiểm soát | Lỗi được ghi, không tác động ngoài phạm vi, chuyển thủ công được | Chạy tiếp sai trạng thái hoặc thực hiện thao tác ngoài quyền |
| 5 | Lặp lại và bảo trì được | Người khác chạy theo hướng dẫn được; nhận ra thay đổi; ghi thời gian bảo trì | Phụ thuộc thao tác không ghi lại, khó biết vì sao ảnh sai hoặc không tính bảo trì |

Đây là tiêu chí và kế hoạch kiểm; chưa có bộ đầu ra đã chạy để chấm hoặc đề nghị bonus eval.

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và dùng không? | **Trung bình** | Có trải nghiệm thật và bottleneck cá nhân; thiếu người ngoài nhóm, tần suất và giờ công. |
| **Usability** | Có vận hành và kiểm kết quả được không? | **Trung bình** | Đã thiết kế điểm kiểm/fallback; chưa quan sát người khác dùng ánh xạ/kịch bản. |
| **Feasibility** | Có dữ liệu, quyền và cách tái tạo trạng thái không? | **Cao** | Chưa xác nhận build, nền tảng, đường đi, data test, quyền và khả năng mở ổn định 10 trạng thái. Công cụ công khai chưa chứng minh chạy được trên app này. |
| **Viability** | Có hợp chi phí và quy định vận hành không? | **Trung bình** | Chưa biết setup/bảo trì, quyền dùng ảnh/design và người duy trì lâu dài. |

### 8.2. Kết luận

**Quyết định đề xuất: Not Yet cho triển khai; tiếp tục discovery với candidate #1 làm hướng chính.**

Rủi ro Feasibility còn Cao và chưa hoàn tất kiểm chứng ngoài nhóm. Not Yet xác định điều kiện cần vượt qua trước Go, không đổi candidate đã chọn.

**Cần kiểm chứng trước:**

1. Xác nhận quyền build/design/data/tài khoản; chỉ định người phụ trách và duyệt báo cáo.
2. Phỏng vấn 2–3 dev/tester ngoài nhóm, ghi cả trường hợp không có pain.
3. Chốt 10 trường hợp, mở thủ công được và bấm giờ theo bước; tách chờ và thực làm.
4. Thử checklist chuẩn hóa; chỉ viết/chạy kịch bản nếu thao tác lặp vẫn tốn thời gian và đường đi tái tạo được.

**Pilot nhỏ nhất sau khi đủ điều kiện Go:** tối đa 2 tuần; một app/nền tảng, 10 trường hợp; so checklist với Rule trên cùng cấu hình, ghi setup/bảo trì và chấm 5 tiêu chí. Tester kiểm mọi ảnh; không cần xây sản phẩm hay Agent cho phép thử.

**Điều kiện chuyển Go:** không còn rủi ro Cao; có quyền/đầu vào; có xác nhận pain từ người dùng phù hợp; có baseline và người chịu trách nhiệm pilot. Chỉ mở rộng sau khi đạt target thời gian ròng và chất lượng.

**Ngưỡng dừng / quay về:**

- Không có quyền dùng build/design/data → dừng trên hệ thống đó; dùng dữ liệu mẫu được phép hoặc No-Go cho phạm vi đó.
- Sau tối đa 2 tuần chưa mở ổn định ít nhất 9/10 trường hợp bằng kịch bản → dừng mở rộng Rule, tìm nguyên nhân và quay về checklist/thủ công. Nếu đạt 9/10, trường hợp còn lại vẫn phải xử lý thủ công và tính vào đủ 10 trường hợp khi đánh giá thời gian, không loại khỏi phép đo.
- Có một ảnh sai trạng thái bị đánh dấu hoàn tất hoặc một thao tác ngoài phạm vi → dừng lượt chạy, kiểm lại ảnh và sửa điểm kiểm trước khi thử tiếp.
- Không giảm ít nhất 50% thời gian ròng trên cùng phạm vi sau setup/bảo trì → chưa mở rộng; nếu checklist đủ thì chọn No AI.
- Kiểm chứng cho thấy pain ít lặp hoặc chủ yếu do chờ build → sửa problem/boundary trước khi tiếp tục.

**Nếu No-Go sau kiểm chứng:** giữ checklist, data test và mẫu báo cáo đã chuẩn hóa; ghi điều học được, dừng phần tự động hóa không tạo giá trị.

---

## 9. Hạn chế và hướng tiếp theo

- Chưa có Interview Snapshot, survey hoặc tín hiệu phản bác thực tế; bộ hỏi–đáp mô phỏng chỉ dùng luyện tập.
- Số phút theo bước là mô hình; cần đo giờ thực làm và tách khỏi hai tuần lịch của đợt báo cáo.
- Nhóm cần tự xác nhận điểm, ghi phản biện thực tế và phân công người nhận vai.
- Chưa biết app/nền tảng và điều kiện dữ liệu; không suy ra mọi trạng thái đều mở được bằng deep link hoặc kịch bản.
- Chưa chứng minh cần AI. Nếu Rule/checklist đủ thì giữ mức đó; chỉ mở vòng Workflow nếu còn pain được đo.
- #2 Jira và #9 Biên bản/hỏi đáp họp giữ cho vòng sau; sáu candidate khác cần thêm actor cụ thể và bằng chứng từ người đề xuất.

## 10. Tài liệu tham khảo

- [Figma REST API — File endpoints](https://developers.figma.com/docs/rest-api/file-endpoints/).
- [Maestro — openLink](https://docs.maestro.dev/reference/commands-available/openlink) và [takeScreenshot](https://docs.maestro.dev/reference/commands-available/takescreenshot).
- [Android Developers — Create deep links](https://developer.android.com/training/app-links/create-deeplinks).
- [Checkpoints](../../CHECKPOINTS.md), [worksheet](../../docs/01-worksheet.md), [rubric](../../RUBRIC.md).
