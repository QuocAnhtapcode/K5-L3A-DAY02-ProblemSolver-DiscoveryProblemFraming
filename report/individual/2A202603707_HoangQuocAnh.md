# Báo cáo cá nhân — Hoàng Quốc Anh — 2A202603707

> Báo cáo được biên soạn với hỗ trợ của AI từ trải nghiệm và thông tin nhóm do tôi cung cấp. Các số phút trong sơ đồ là ước lượng lập kế hoạch; dữ kiện tự thuật được ghi riêng. Phần phản biện mô phỏng và reflection dự thảo được phân biệt với hoạt động đã thực hiện.

## 1. Thông tin học viên

- Họ tên: Hoàng Quốc Anh
- MSSV: 2A202603707
- Email trường (không bắt buộc, repo có thể để public): 26ai.anhhq@vinuni.edu.vn
- Tên nhóm: Problem Solver
- Link repo nhóm: https://github.com/QuocAnhtapcode/K5-L3A-DAY02-ProblemSolver-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi khách hàng định kỳ yêu cầu báo cáo ảnh app thực tế để đối chiếu Figma, tôi muốn mở được đúng màn và trạng thái cần chụp, để thu thập đủ ảnh cho báo cáo mà không phải dò lại luồng thao tác nhiều lần. | Dev và tester | Một đội dev/tester 6 người mất 2 tuần để hoàn thiện một đợt báo cáo; tôi xác nhận vướng chính ở mở đúng màn/trạng thái. Hai tuần là thời gian lịch, chưa phải giờ công. |
| 2 | Tốn thời gian | Khi nhận ticket bug từ Jira của khách hàng trong một source code lớn, tôi muốn xác định luồng xử lý và vị trí code liên quan có căn cứ, để bắt đầu sửa đúng chỗ mà không phải điều tra lan man từ đầu. | Dev | Theo trải nghiệm của tôi, một ticket mới có thể mất cả ngày để tìm vị trí code cần sửa; chưa có log thời gian theo bước. |
| 3 | Pain từ người khác | Khi tester nhận tài liệu nghiệp vụ từ BA nhưng yêu cầu còn mơ hồ, tôi muốn các bên thống nhất được hành vi mong đợi và điều kiện kiểm thử, để tránh tranh luận và sửa lại khi thực hiện test. | Tester và BA | Tháng trước có bất đồng giữa đội BA và tester làm trễ tiến độ của khách; cần bổ sung số lượt trao đổi, số ngày trễ hoặc ticket minh chứng đã ẩn thông tin. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi tìm nhà thuê từ nhiều hội nhóm Facebook và nguồn khác nhau, tôi muốn so sánh được thông tin phù hợp với nhu cầu của mình, để chọn chỗ đáng đi xem và tránh đi lại không cần thiết. | Người thuê nhà | Tuần trước tôi dành cả tuần để tìm và đi xem phòng; chưa tách thời gian đọc tin, liên hệ và đi thực tế. |
| 5 | Tốn thời gian | Khi tự làm thủ tục đóng phạt vi phạm giao thông trực tuyến và hướng dẫn chưa rõ, tôi muốn biết cần chuẩn bị gì và phải thực hiện bước nào tiếp theo, để hoàn thành thủ tục mà không mất nhiều thời gian tìm hiểu. | Người tự thực hiện thủ tục, với trường hợp ban đầu là tôi | Tôi mất cả buổi sáng vì không rõ thủ tục; chưa quy đổi thành số phút bấm giờ. |
| 6 | Tốn thời gian | Khi nhóm bạn cùng chi tiền cho một chuyến đi, tôi muốn biết mỗi người đã trả bao nhiêu và còn phải thanh toán cho ai, để chia chi phí công bằng. | Người tổ chức chuyến đi, thành viên nhóm | Tháng trước tôi đi du lịch cùng nhóm bạn và mất nhiều thời gian chia tiền sau chuyến đi; cần bổ sung số người, số khoản và thời gian đối chiếu. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Tôi đã tham khảo danh sách gợi ý của AI; giữ cách diễn đạt cho vấn đề #5 và #6 vì có trải nghiệm tương ứng của chính mình. Tôi bổ sung trường hợp đóng phạt mất cả buổi sáng và chuyến du lịch tháng trước.
- Các gợi ý chưa gắn với trải nghiệm của tôi không đưa vào sáu vấn đề này. Tôi cũng sửa các mô tả ban đầu về công việc thành Job Story, tập trung vào tình huống, động cơ và kết quả.
- Vấn đề #3 và #6 còn thiếu số đo; kế hoạch bổ sung là đếm lượt trao đổi/thời gian trễ và bấm giờ việc đối chiếu chi phí, thay vì tự điền số.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Vấn đề #1 — Chuẩn bị báo cáo ảnh app thực tế để đối chiếu thiết kế Figma | Actor và đầu ra rõ; yêu cầu xuất hiện lặp lại; đã có một đợt đội 6 người mất 2 tuần để hoàn thành; tôi xác nhận vướng nhất ở mở đúng màn/trạng thái; có thể giới hạn thử nghiệm ở một nhóm màn hình | Hai tuần gồm bao nhiêu giờ thực làm, bao nhiêu màn/trạng thái/thiết bị? Mất bao nhiêu phút để mở đúng một màn/trạng thái, và bao nhiêu lần phải thực hiện lại? |
| 2 | Vấn đề #2 — Khoanh vùng code khi điều tra ticket bug từ Jira | Pain gắn với công việc dev; có thể đo thời gian từ lúc nhận ticket đến khi xác định vị trí liên quan kèm bằng chứng; có thể thử trên một module | Thời gian nằm ở tái hiện bug, tìm code, kiểm giả thuyết hay chờ khách bổ sung? Ticket có đủ dữ liệu và lỗi có tái hiện được không? |
| 3 | Vấn đề #5 — Không rõ bước tiếp theo khi tự làm thủ tục trực tuyến | Có trải nghiệm trực tiếp: tôi mất cả buổi sáng khi đóng phạt vi phạm giao thông vì không rõ thủ tục; có thể giới hạn vào chính thủ tục đã gặp | Vướng ở bước hoặc hướng dẫn cụ thể nào? “Cả buổi sáng” có bao nhiêu phút thực tìm hiểu và bao nhiêu phút chờ? Chưa có bằng chứng về lỗi từng ô biểu mẫu hoặc trải nghiệm của người lớn tuổi |

### Problem Card #1 — Báo cáo ảnh app thực tế để đối chiếu Figma

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách hàng yêu cầu báo cáo hình ảnh của app đang chạy để đối chiếu với thiết kế Figma, tôi muốn thu thập đủ ảnh đúng màn và trạng thái, đối chiếu được với đúng bản thiết kế, để gửi báo cáo chính xác mà không phải chụp hoặc ghép lại nhiều lần. |
| Actor | Dev và tester phụ trách chuẩn bị báo cáo cho khách hàng; trường hợp đã ghi nhận có đội 6 người tham gia. |
| Thời điểm / bối cảnh | Mỗi đợt khách hàng yêu cầu báo cáo. Cần xác định trước phiên bản app, bản thiết kế, danh sách màn, trạng thái và cấu hình thiết bị thuộc phạm vi. Chưa có số liệu về tần suất yêu cầu. |
| Quy trình hiện tại (3–7 bước) | 6 bước: (1) Xác định màn/trạng thái và thiết kế cần đối chiếu; (2) Đưa app về đúng màn/trạng thái; (3) Chụp và lưu ảnh có định danh; (4) Đối chiếu ảnh app với Figma; (5) Ghép ảnh và ghi nhận khác biệt vào báo cáo; (6) Kiểm tra độ đầy đủ, phiên bản và bàn giao báo cáo. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2 — mở đúng màn/trạng thái đã được tôi xác nhận là điểm vướng chính.** Cần làm rõ phải điều hướng, chuẩn bị dữ liệu hoặc đáp ứng điều kiện gì để tới được trạng thái đó. Ước lượng minh họa 15 phút/màn-trạng thái. |
| Impact (nếu không giải thì sao) | Hiện tại một đợt báo cáo mất 2 tuần với đội dev/tester 6 người tham gia. Rủi ro cần kiểm chứng: ảnh thiếu/sai trạng thái, ghép nhầm thiết kế, phải làm lại và giảm thời gian dành cho phát triển hoặc kiểm thử. |
| Success metric (baseline → target) | Baseline cần đo: phút thực làm trên mỗi màn-trạng thái-cấu hình thiết bị, số ảnh thiếu/sai và số vòng sửa trong một đợt báo cáo. Mục tiêu đề xuất: giảm ít nhất 50% thời gian thực làm trên cùng đơn vị và phạm vi; 100% mục trong danh sách đã thống nhất có ảnh đúng phiên bản/trạng thái, số ảnh phải chụp lại không tăng. Cách đo: bấm giờ từng bước trên 10 trường hợp trước/sau, cùng người kiểm và tiêu chí; ghi riêng thời gian chờ. |
| Phương án không dùng AI | Chuẩn hóa danh sách màn/trạng thái, dữ liệu kiểm thử, cách đặt tên ảnh và mẫu báo cáo; phân công theo màn để tránh trùng việc. Nếu luồng thao tác ổn định, thử script kiểm thử giao diện chụp ảnh theo kịch bản và ghép báo cáo theo quy tắc; tester vẫn kiểm ảnh và kết luận khác biệt. |
| Giả thuyết về AI (nếu có) | Nếu việc ghép frame Figma với màn/trạng thái trong app vẫn mơ hồ sau khi đã chuẩn hóa danh mục, thử hỗ trợ đề xuất các mục phù hợp từ danh mục đã duyệt, kèm căn cứ. Tester xác nhận trước khi mở màn; script chạy kịch bản cố định. Không suy ra đường dẫn hoặc quyền truy cập chỉ từ ảnh thiết kế. Việc tự đánh giá khác biệt giao diện là hướng sau, ngoài phạm vi chính của lần này. |
| Cảm nhận nhanh | **Rule, cần kiểm chứng.** Hướng chính là bảng liên kết frame → màn/trạng thái → điều kiện dữ liệu và kịch bản mở/chụp. Chỉ cân nhắc Workflow nếu đo cho thấy bước ghép frame vào danh mục còn cần xử lý ngữ nghĩa mà Rule chưa đủ. |

Quy trình nháp hiện tại — **đơn vị: 1 màn × 1 trạng thái × 1 cấu hình thiết bị**. Thời gian là ước lượng minh họa, chưa gồm chi phí thiết lập chung và các vòng làm lại của cả đợt.

```text
HIỆN TẠI — KỊCH BẢN ƯỚC LƯỢNG 30 PHÚT / TRƯỜNG HỢP

[1 Xác định màn/trạng thái + bản Figma: 5']
→ [2 Đưa app về đúng màn/trạng thái: 15'] ← BOTTLENECK
→ [3 Chụp + lưu ảnh có định danh: 1']
→ [4 Đối chiếu ảnh app với Figma: 3']
→ [5 Ghép ảnh + ghi khác biệt vào báo cáo: 4']
→ [6 Kiểm tra đủ/đúng + bàn giao: 2']
```

### Problem Card #2 — Khoanh vùng code khi điều tra bug từ Jira

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận ticket bug từ Jira của khách hàng trong một source code lớn, tôi muốn lần được từ triệu chứng lỗi đến luồng xử lý và vị trí code liên quan có bằng chứng, để bắt đầu sửa đúng chỗ mà không phải đọc mò nhiều phần của hệ thống. |
| Actor | Dev được giao điều tra và sửa ticket bug, đặc biệt khi chưa quen module phát sinh lỗi. |
| Thời điểm / bối cảnh | Khi nhận một ticket mới. Phạm vi card là từ lúc bắt đầu điều tra đến khi khoanh vùng được vị trí có căn cứ, chưa gồm sửa code, kiểm thử bản sửa và triển khai. Cần ghi rõ phiên bản source, môi trường và chất lượng thông tin trong ticket. |
| Quy trình hiện tại (3–7 bước) | 5 bước: (1) Đọc ticket, làm rõ điều kiện và hành vi kỳ vọng/thực tế; (2) Tái hiện lỗi và lấy log/stack trace nếu có; (3) Lần luồng xử lý, tìm module/file/hàm liên quan; (4) Kiểm tra giả thuyết bằng debugger, log hoặc kiểm thử và quay lại bước 3 nếu sai; (5) Ghi vị trí đã khoanh vùng, bằng chứng và hướng sửa dự kiến. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 — lần từ triệu chứng đến module/file/hàm trong source lớn. Đây là giả thuyết bám vào mô tả “có thể tốn cả ngày để tìm ra file cần sửa”; ước lượng minh họa 240 phút/ticket. |
| Impact (nếu không giải thì sao) | Việc tìm vị trí cần sửa có thể mất cả ngày. Rủi ro cần kiểm chứng: điều tra lặp lại giữa các dev, sửa nhầm vị trí, kéo dài thời gian xử lý ticket. |
| Success metric (baseline → target) | Baseline cần đo: trung vị phút khoanh vùng ở bước 3 và tổng phút điều tra cho ít nhất 5 ticket có mức khó tương đương. Mục tiêu đề xuất: giảm ít nhất 50% trung vị thời gian khoanh vùng; tỷ lệ giả thuyết bị bác bỏ hoặc phải quay lại điều tra không tăng. Cách đo: ghi giờ theo bước, số vòng kiểm giả thuyết và bằng chứng xác nhận; tách thời gian chờ khách bổ sung khỏi thời gian dev thực làm. |
| Phương án không dùng AI | Chuẩn hóa ticket với bước tái hiện, phiên bản, môi trường và log; bổ sung sơ đồ module, người phụ trách từng phần; dùng tìm kiếm code, debugger và kiểm thử tái hiện. Giới hạn thử nghiệm ở một module để kiểm tra các cách này đã đủ giảm thời gian chưa. |
| Giả thuyết về AI (nếu có) | Trong một luồng điều tra định sẵn, hỗ trợ đọc ticket/log và đề xuất danh sách vị trí code cần kiểm tra kèm đường dẫn, hàm và căn cứ từ source đúng phiên bản. Dev xác nhận bằng tái hiện/debug/kiểm thử; gợi ý vị trí không được coi là kết luận nguyên nhân, không tự sửa hoặc triển khai. Chỉ thử khi có quyền sử dụng source và dữ liệu liên quan. |
| Cảm nhận nhanh | **Workflow, cần kiểm chứng.** Các bước điều tra vẫn được xác định trước và dev kiểm từng giả thuyết; chưa có bằng chứng cần Agent tự quyết toàn bộ. Cần so sánh với ticket đầy đủ + tài liệu module + tìm kiếm code trước khi chọn mức này. |

Quy trình nháp hiện tại — **đơn vị: 1 ticket điều tra**. Đây là kịch bản ước lượng tổng 420 phút để chuẩn bị đo, thời gian vòng lặp bước 3–4 tính vào hai bước đó.

```text
HIỆN TẠI — KỊCH BẢN ƯỚC LƯỢNG 420 PHÚT / TICKET

[1 Đọc ticket + làm rõ thông tin: 30']
→ [2 Tái hiện + thu log/stack trace: 45']
→ [3 Lần luồng + tìm module/file/hàm: 240'] ← BOTTLENECK
→ [4 Kiểm giả thuyết bằng debug/log/test: 90']
   Nếu chưa có căn cứ: quay lại bước 3
→ [5 Ghi vị trí + bằng chứng + hướng sửa dự kiến: 15']
```

### Problem Card #3 — Hiểu bước tiếp theo khi làm thủ tục trực tuyến (vấn đề #5)

| Trường | Nội dung |
|---|---|
| Job Story | Khi tự làm thủ tục đóng phạt vi phạm giao thông trực tuyến và gặp hướng dẫn chưa rõ, tôi muốn biết mình đang ở bước nào, cần chuẩn bị hoặc bổ sung gì và tiếp theo phải làm gì, để hoàn thành thủ tục đúng cách mà không phải thử lại nhiều lần hoặc nhờ người khác giải thích. |
| Actor | Người tự làm thủ tục đóng phạt trực tuyến, với bằng chứng ban đầu là trải nghiệm của chính tôi. |
| Thời điểm / bối cảnh | Khi thực hiện thủ tục trên hệ thống trực tuyến và không hiểu cách đi tiếp. Bản nháp thu hẹp vào một điểm vướng của thủ tục đóng phạt; cần bổ sung tên hệ thống, bước cụ thể và nguyên văn hướng dẫn/thông báo đã gặp. Chưa xác nhận có lỗi ở từng ô biểu mẫu. |
| Quy trình hiện tại (3–7 bước) | Bản nháp 5 bước cần xác nhận từ trải nghiệm thật: (1) Mở thủ tục và đọc yêu cầu ban đầu; (2) Chuẩn bị/nhập thông tin hệ thống yêu cầu; (3) Đọc hướng dẫn tại điểm vướng và xác định việc cần làm tiếp; (4) Tra cứu hoặc hỏi hỗ trợ, bổ sung/chỉnh lại thông tin nếu cần; (5) Tiếp tục thao tác và kiểm tra trạng thái kết quả. Đây không phải hướng dẫn thao tác của một cổng dịch vụ cụ thể. |
| Bottleneck (bước nào, mất bao nhiêu phút) |  Bước 3 — hiểu yêu cầu và xác định bước tiếp theo từ hướng dẫn chưa rõ. Tôi đã mất cả buổi sáng vì không rõ thủ tục. Phân bổ minh họa 90 phút cho bước 3. |
| Impact (nếu không giải thì sao) | Dữ kiện từ trải nghiệm của tôi: mất **cả buổi sáng** khi làm thủ tục đóng phạt vi phạm giao thông vì không rõ thủ tục. |
| Success metric (baseline → target) | Baseline theo trải nghiệm: cả buổi sáng để làm thủ tục vì không rõ quy trình; cần ghi lại mốc bắt đầu/kết thúc, tách phút thực tìm hiểu khỏi phút chờ. Mục tiêu đề xuất: giảm ít nhất 50% thời gian chủ động tìm hiểu quy trình trên cùng tình huống; người dùng xác định đúng yêu cầu/bước tiếp theo theo nội dung chính thức, số thao tác sai không tăng. Cách đo: ghi thời gian từng bước của phiên thực tế, sau đó thử cùng tình huống với ít nhất 3 người có trải nghiệm phù hợp. |
| Phương án không dùng AI | Viết lại hướng dẫn theo từng bước, nêu rõ thông tin cần chuẩn bị, vị trí đang thực hiện và điều kiện để đi tiếp; nếu có lỗi biểu mẫu, chỉ rõ trường lỗi và cách sửa, giữ lại dữ liệu đã nhập. Nếu không có quyền sửa hệ thống, thử một hướng dẫn/checklist ngắn dựa trên nội dung chính thức cho đúng điểm vướng. |
| Giả thuyết về AI (nếu có) | Chỉ cân nhắc giải thích hướng dẫn bằng ngôn ngữ dễ hiểu khi câu hỏi đa dạng và đã có nguồn chính thức làm căn cứ. Không tự suy diễn quy định, kết luận nghĩa vụ, nộp hồ sơ hoặc thực hiện thanh toán; khi nguồn không đủ thì chuyển người dùng sang kênh hỗ trợ của hệ thống. |
| Cảm nhận nhanh | **No AI trước; Rule nếu cần hướng dẫn theo trạng thái hoặc kiểm tra dữ liệu.** Chưa có bằng chứng cho thấy hướng dẫn rõ ràng và kiểm tra cố định là không đủ; chưa cần chọn Workflow hoặc Agent. |

Quy trình nháp hiện tại — **đơn vị: 1 phiên làm thủ tục gặp hướng dẫn chưa rõ**. Thời gian thực tế theo tôi kể là **cả buổi sáng**. Tổng 180 phút dưới đây chỉ là kịch bản phân bổ minh họa để chuẩn bị đo từng bước, không phải quy đổi chính xác từ lời kể; chưa gồm thời gian chờ hệ thống hoặc người hỗ trợ.

```text
HIỆN TẠI — KỊCH BẢN ƯỚC LƯỢNG 180 PHÚT / PHIÊN

[1 Mở thủ tục + đọc yêu cầu ban đầu: 10']
→ [2 Chuẩn bị/nhập thông tin được yêu cầu: 25']
→ [3 Hiểu hướng dẫn + xác định bước tiếp theo: 90'] ← BOTTLENECK
→ [4 Tra cứu/hỏi hỗ trợ + bổ sung nếu cần: 45']
→ [5 Tiếp tục thao tác + kiểm tra trạng thái kết quả: 10']
```

### Card muốn pitch nhất

- Card số: **Card #1**
- Vì sao: Có bối cảnh công việc cụ thể và một đợt báo cáo đã xảy ra; có thể giới hạn vào 10 màn-trạng thái để đo; đầu ra đủ/đúng ảnh kiểm tra được; có phương án Rule để so sánh trước khi cân nhắc AI.
- Câu hỏi muốn nhóm phản biện: “Vướng nhất ở mở đúng màn/trạng thái là do thao tác điều hướng, dữ liệu hay điều kiện truy cập? Nếu chuẩn hóa dữ liệu kiểm thử và script điều hướng/chụp ảnh đã đủ thì phần nào còn cần AI? Hai tuần hoàn thành báo cáo có bao nhiêu thời gian thực làm và bao nhiêu thời gian chờ?”

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: “6 người, 2 tuần” chưa chứng minh số giờ công và ban đầu chưa xác định bước nghẽn. | Tôi xác nhận vướng ở mở đúng màn/trạng thái; chưa có thời gian bấm giờ. | Đã chọn bước 2 làm bottleneck theo xác nhận của tôi; tách thời gian lịch khỏi thời gian thực làm và quy định đơn vị đo theo màn-trạng thái-thiết bị. |
| Card #2: Source lớn chưa đủ để kết luận cần AI; tìm được file chưa đồng nghĩa tìm đúng nguyên nhân. | Chờ tôi xác nhận qua các ticket đã xử lý. | Bản nháp đã thêm phương án ticket chuẩn/tài liệu module/tìm kiếm code; yêu cầu bằng chứng debug hoặc kiểm thử; tách điều tra khỏi sửa và triển khai. |
| Card #3: Job Story ban đầu trong scan nói lỗi biểu mẫu nhưng bằng chứng mới cho thấy quy trình chưa rõ; actor “người lớn tuổi” chưa có dữ liệu. | Tôi xác nhận mất cả buổi sáng vì không rõ thủ tục; cần bổ sung bước cụ thể. | Đã sửa cả Scan và Card để bám vào trải nghiệm tự đóng phạt và thời gian “cả buổi sáng”; không khẳng định người lớn tuổi hoặc lỗi từng ô đã được kiểm chứng. |
| Cả 3 card chưa có thời gian đo theo từng bước. | Cần tôi bấm giờ và thay số trước khi dùng làm baseline. | Mọi sơ đồ đều ghi rõ là kịch bản ước lượng; success metric tách baseline cần đo, target đề xuất và cách đo. |

**Thông tin cần bổ sung:** thời gian đo từng bước, số màn/trạng thái/thiết bị của đợt báo cáo, một ticket bug cụ thể và điểm vướng chính xác của thủ tục trực tuyến. Nhóm đã chọn card #1 làm hướng chính; phần hỏi–đáp luyện tập nằm trong báo cáo nhóm.

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Chuẩn bị pitch Problem Card | Tôi chuẩn bị 3 card về báo cáo ảnh app/Figma, điều tra bug Jira và thủ tục trực tuyến; chọn card #1 để đề xuất. | Hai card của tôi vào shortlist của nhóm; nhóm chọn vấn đề mở đúng màn/trạng thái app làm hướng chính. |
| Phản biện bài của bạn khác | Câu hỏi chuẩn bị cho phương án biên bản họp của Vinh: “Nếu đã có bản ghi và chức năng tìm kiếm, bước nào vẫn khiến người dùng mất thời gian? Làm sao kiểm câu trả lời có đúng với cuộc họp?” | Đưa vào bộ phản biện mô phỏng. |
| Nhận phản biện | AI hỏi: “Nếu bảng liên kết màn và script cố định đã đủ thì còn cần AI ở đâu?” | Tôi cung cấp thông tin thực tế rằng bước vướng nhất là mở đúng màn/trạng thái; bản đề xuất tập trung vào bước này và có phương án Rule để so sánh. |
| Gom cluster / cây OST | Tôi cung cấp danh sách 9 candidate và thông tin người đề xuất để AI tổ chức bản nháp cluster/OST. | Báo cáo nhóm phân biệt pain của người dùng với tên giải pháp bắt đầu bằng “AI hỗ trợ”. |
| Chọn candidate problem | Tôi xác nhận shortlist gồm app/Figma, Jira và biên bản họp; chốt app/Figma là hướng chính của nhóm. | Bảng chấm điểm đề xuất dùng cùng 7 tiêu chí cho cả ba phương án; app/Figma đứng đầu vì phạm vi rõ, có trải nghiệm và dễ kiểm đầu ra. |
| Kiểm chứng / research | Tôi cung cấp trải nghiệm đội 6 người mất 2 tuần, xác định bottleneck mở màn và xác nhận nhóm chưa phỏng vấn người ngoài; nhờ AI mở tài liệu Figma, Maestro và Android Developers. | Có nguồn chính thức cho các khả năng kỹ thuật cơ bản. |
| Quy trình nhóm | Tôi xác định bước mở đúng màn/trạng thái là bottleneck và giữ kịch bản hiện tại 30 phút/trường hợp, bước mở màn 15 phút. | Bản nháp quy trình tương lai hướng tới 15 phút/trường hợp; các con số là mục tiêu/ước lượng để kiểm bằng đo trước–sau. |
| Problem Statement | Tôi cung cấp actor, bối cảnh và bottleneck để AI biên soạn v0/v1. | v1 giới hạn một app, một nền tảng và 10 màn-trạng thái; bổ sung cách đo, người kiểm và ranh giới thao tác. |
| Mức can thiệp AI | Tôi yêu cầu làm rõ giải pháp chính; bản đề xuất so sánh cả No AI, Rule, Workflow và Agent. | Mức đề xuất hiện tại là Rule; AI chỉ là phương án tiếp theo nếu có bằng chứng Rule chưa đủ. Đây là đề xuất cần nhóm xác nhận khi hoàn tất. |
| Quyết định | Tôi chốt bài toán chính; nhờ AI lập phần đánh giá 4 rủi ro và điều kiện thử nghiệm. | Bản báo cáo đề xuất Not Yet cho triển khai: cần xác minh quyền sử dụng app/dữ liệu, khả năng mở màn và kiểm chứng ngoài nhóm trước khi chạy pilot. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tham khảo 20 gợi ý, sau đó đưa 6 vấn đề có trải nghiệm của mình để chỉnh cách diễn đạt. | Gợi ý cấu trúc Job Story và cách thu thập dấu hiệu thật. | Ví dụ chung chưa phản ánh đầy đủ trường hợp đóng phạt của tôi; một số vấn đề của tôi còn thiếu số đo. | Tôi bổ sung trải nghiệm đóng phạt mất cả buổi sáng, giữ các vấn đề gắn với học tập/đời sống/công việc đã gặp. |
| CP2 Problem Card | Nhờ AI triển khai bản nháp chi tiết cho các vấn đề #1, #2, #5 tôi đã scan và phản biện các giả định. | Tổ chức Job Story, actor, quy trình, metric, phương án không dùng AI; chỉ ra chỗ bằng chứng chưa khớp với mô tả. | AI chưa biết đủ quy trình; bản nháp đầu minh họa vấn đề #5 bằng 30 phút, không sát trải nghiệm mất cả buổi sáng. Mọi số phút theo bước vẫn là ước lượng. | Tôi xác nhận vấn đề #1 vướng ở mở đúng màn/trạng thái và vấn đề #5 mất cả buổi sáng vì không rõ thủ tục; AI đã cập nhật card theo phản hồi. Tôi còn cần kiểm lại các bước và thay ước lượng bằng số đo. |
| CP3 Hội tụ nhóm | Cung cấp 9 candidate, shortlist 3 và lựa chọn cuối để AI tổ chức bản nháp, đề xuất điểm cùng bộ hỏi–đáp mô phỏng. | Tách pain khỏi giải pháp, giải thích các tiêu chí so sánh. | Bảng điểm và câu trả lời mô phỏng không phải dữ liệu chấm độc lập hoặc phản biện trực tiếp của thành viên. | Tôi xác nhận lựa chọn app/Figma; phần nhật ký pitch thực tế chưa có. |
| CP4 Research | Nhờ AI tìm và mở tài liệu chính thức Figma REST API, Maestro và Android deep links. | Làm rõ phần công cụ có sẵn và khoảng trống ghép thiết kế với trạng thái app. | Tài liệu công cụ chưa chứng minh áp dụng được cho app của nhóm; chưa biết nền tảng và quyền truy cập cụ thể. | Tôi cần tự mở nguồn và kiểm khả năng áp dụng; report ghi nghiên cứu tài liệu riêng với dữ liệu người dùng. |
| CP4 Phản biện mô phỏng | Nhờ AI tự đặt câu hỏi và trả lời để chuẩn bị thảo luận khi nhóm chưa phỏng vấn ai. | Có bộ câu hỏi kiểm giả định, phản chứng và điều kiện dừng. | Câu trả lời do AI tạo không thay thế người dùng thật. | Tôi xác nhận nhóm chưa có phỏng vấn; không tính mô phỏng vào số người kiểm chứng. |
| CP5 Quy trình | Nhờ AI diễn đạt quy trình trước/sau từ bottleneck đã cung cấp. | Tách phần Rule, người kiểm, điều kiện dữ liệu và cách quay về thao tác thủ công. | Ước lượng thời gian chưa phải số đo; chưa biết đủ trạng thái đặc biệt của app. | Tôi xác nhận bước mở màn là điểm nghẽn; giữ các số theo bước ở mức kịch bản để đo lại. |
| CP5–6 Problem Statement | Nhờ AI biên soạn v0/v1 và phản biện độ rõ của metric, phạm vi, boundary. | Liên kết actor → bottleneck → metric → tiêu chí nghiệm thu. | Không thể suy giờ công từ 6 người/2 tuần; không thể cam kết giảm thời gian khi chưa chạy thử. | Tôi đã cung cấp thông tin thực tế và lựa chọn bài toán; cần xác nhận các mục tiêu đề xuất trước khi nộp. |
| CP6 Mức can thiệp / quyết định | Nhờ AI so sánh 4 mức, đánh giá rủi ro và đề xuất quyết định. | Chỉ ra có thể bắt đầu bằng Rule và cần kiểm feasibility trước pilot. | Đánh giá dựa trên thông tin còn hạn chế; chưa phải kết luận được tất cả thành viên xác nhận. | Tôi giữ hướng chính app/Figma; phần triển khai được ghi Not Yet trong bản đề xuất, kèm điều kiện để chuyển Go. |
| CP7 Reflection | Nhờ AI biên soạn bản nháp từ các thông tin và phản hồi tôi đã cung cấp trong trao đổi. | Tổ chức các ý về giới hạn bằng chứng, lựa chọn bài toán và cách sửa bản nháp. | AI không biết trải nghiệm thảo luận thực tế của tôi ngoài những gì tôi cung cấp. | Tôi cần đọc, tự xác nhận và chỉnh lại các nhận định cá nhân trước khi sử dụng như reflection chính thức. |

---

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Từ danh sách chín phương án của nhóm, tôi thấy các thành viên quan tâm đến nhiều bối cảnh khác nhau: thuế hộ kinh doanh, học tập, tìm việc, tồn kho, tuyển dụng và cuộc họp. Tôi chưa có nhật ký phần trình bày trực tiếp nên phần này dựa trên danh sách đã tổng hợp. Điểm tôi rút ra là một tên giải pháp hấp dẫn chưa đủ để so sánh; cần làm rõ ai gặp vấn đề, đang làm theo quy trình nào và mất thời gian ở bước nào. Với app/Figma, tôi đã xác định được điểm vướng là mở đúng màn và trạng thái, thay vì nói chung rằng làm báo cáo lâu.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Nhiều phương án trong danh sách ban đầu bắt đầu bằng “AI hỗ trợ”, nên bản báo cáo có nguy cơ đi thẳng vào công cụ. Cách xử lý trong bản đề xuất là chuyển chúng thành Job Story và tách outcome khỏi tên tính năng. Bài toán của tôi được diễn đạt thành giảm thời gian mở đúng màn/trạng thái để thu thập ảnh, còn mức dùng AI được xét sau. Tôi chưa có bằng chứng rằng chỉ một bảng liên kết và kịch bản cố định là không đủ; vì vậy cần có phương án No AI/Rule để đối chiếu.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Ví dụ có thật trong quá trình làm bản nháp là tôi đã sửa thông tin cho AI: vấn đề báo cáo ảnh app vướng nhất ở mở đúng màn/trạng thái; còn thủ tục đóng phạt khiến tôi mất cả buổi sáng vì không rõ quy trình. Những chi tiết này làm nội dung card cụ thể hơn và tránh dùng thời gian minh họa như dữ kiện đã đo. Tôi chưa cung cấp một tình huống đổi ý sau phản biện trực tiếp từ thành viên khác, nên không ghi thêm tình huống đó. Điểm thay đổi của bản nháp là tập trung vào bottleneck đã xác định và tách trải nghiệm thật khỏi giả định.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Nhóm chưa phỏng vấn hoặc survey người ngoài nhóm. Vì thế tôi chưa thể nói vấn đề của mình đã được xác nhận rộng hơn. Phần nghiên cứu tài liệu giúp phân biệt hai việc: lấy được frame/ảnh từ Figma và điều hướng được app không tự tạo ra một liên kết chính xác giữa hai bên. Khoảng trống vẫn là màn nào, trạng thái nào, dữ liệu nào và điều kiện truy cập nào tương ứng với frame. Đây là giả định kỹ thuật cần kiểm trên app thật; bộ hỏi–đáp mô phỏng chỉ giúp chuẩn bị câu hỏi.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là chuyển nhận xét “đội sáu người mất hai tuần” thành một metric có thể kiểm tra. Hai tuần là thời gian hoàn thành một đợt, còn chưa biết mỗi người làm bao lâu hay có bao nhiêu thời gian chờ. Tôi cần chọn đơn vị là một màn-trạng thái trên một cấu hình thiết bị, đo riêng thời gian mở màn và thời gian cả quy trình. Target giảm thời gian cũng phải đi cùng chất lượng: ảnh phải đúng trạng thái và đúng bản thiết kế. Nhanh hơn nhưng chụp nhầm màn thì không đạt mục tiêu.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Tôi sẽ ghi thời gian ngay từ đầu và lưu các trường hợp khó mở màn thay vì chỉ nhớ tổng thời gian cả đợt. Tôi cũng sẽ hỏi hai đến ba dev/tester ngoài nhóm về lần làm báo cáo gần nhất, cách họ xử lý hiện tại và trường hợp cách cũ đã đủ tốt. Trong lựa chọn giải pháp, tôi sẽ hỏi kỹ chi phí tạo, cập nhật bảng liên kết và kịch bản mỗi khi app hoặc Figma đổi. Nếu chi phí chuẩn bị và bảo trì lớn hơn phần thời gian tiết kiệm, nhóm cần thu hẹp phạm vi hoặc dừng hướng thử nghiệm đó.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Vấn đề nhóm chọn là dev/tester mất thời gian mở đúng màn và trạng thái app để chụp ảnh đối chiếu Figma. Quy trình đi từ xác định frame và trạng thái, mở app, chụp ảnh, đối chiếu, ghép báo cáo đến kiểm tra và bàn giao. Bước mở đúng màn/trạng thái là bottleneck được tôi xác nhận, còn số phút cần đo thực tế. Metric chính là thời gian bước mở màn và tổng thời gian trên cùng bộ 10 trường hợp, đồng thời ảnh phải đúng phiên bản và trạng thái. Boundary là chỉ dùng môi trường, tài khoản và dữ liệu được phép; con người kiểm ảnh và duyệt báo cáo, hệ thống không tự thực hiện nghiệp vụ thật hoặc gửi báo cáo. Mức đề xuất ban đầu là Rule với bảng liên kết frame và kịch bản định sẵn; Workflow chỉ được xét khi có bằng chứng cần hỗ trợ xử lý ngữ nghĩa. Quyết định đề xuất hiện tại là Not Yet cho triển khai, vì còn phải xác minh khả năng mở màn, quyền dữ liệu và nhu cầu từ người ngoài nhóm.

---

## 7. Tài liệu tham khảo

- [Worksheet của lab](../../docs/01-worksheet.md) và [bài làm mẫu](../../docs/02-deliverable-example.md): cấu trúc Scan, Problem Card và chuỗi lập luận.
- [Rubric](../../RUBRIC.md) và [báo cáo nhóm](../team/group_report.md): tiêu chí chấm và hướng app/Figma được lựa chọn.
- [Figma REST API — File endpoints](https://developers.figma.com/docs/rest-api/file-endpoints/): tài liệu lấy dữ liệu node và render ảnh thiết kế.
- [Maestro — openLink](https://docs.maestro.dev/reference/commands-available/openlink) và [takeScreenshot](https://docs.maestro.dev/reference/commands-available/takescreenshot): tài liệu mở URL/deep link và chụp ảnh.
- [Android Developers — Create deep links](https://developer.android.com/training/app-links/create-deeplinks): điều kiện định tuyến vào app trên Android, nếu đây là nền tảng được chọn.

