# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Phú Thái
- MSSV: 2A202604001
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: SixSeven
- Link repo nhóm: https://github.com/phuthaitran/K5-L3B-DAY02-SixSeven-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi cài đặt máy tính hay máy in mới cho khách hàng, tôi muốn biết chính xác danh sách phần mềm, driver và cấu hình tương ứng theo từng khách hàng, để không bỏ sót bước và không phải hỏi lại đồng nghiệp. | IT Support | Số lần phải cài đặt bổ sung hoặc sửa lỗi |
| 2 | Lặp lại | Khi xử lý các lỗi máy in thường gặp, tôi muốn biết các bước kiểm tra tương ứng với từng dòng máy và môi trường mạng, để không phải lặp lại quá trình tìm nguyên nhân từ đầu. | IT Support | Thời gian xử lý mỗi sự cố máy in |
| 3 | Tốn thời gian | Khi cần xác định nguyên nhân một sự cố phức tạp, tôi muốn biết những bước kiểm tra đã được thực hiện và kết quả tương ứng, để không mất thời gian thử lại những phương án đã thất bại. | IT Support | Thời gian xác định nguyên nhân và số bước kiểm tra bị lặp lại |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi hỗ trợ một khách hàng mới hoặc một môi trường IT chưa quen thuộc, tôi muốn nắm được tổng quan hệ thống, thiết bị, phần mềm và các cấu hình đặc thù của khách hàng, để không phải đọc nhiều tài liệu rời rạc trước khi bắt đầu công việc. | IT Support | Thời gian chuẩn bị trước khi thực hiện công việc tại khách hàng. | 
| 5 | Pain từ người khác | Khi nhiều nhân viên cùng gửi yêu cầu hỗ trợ trong một khoảng thời gian, tôi muốn biết mức độ ảnh hưởng và mức độ ưu tiên của từng yêu cầu, để không bỏ sót những vấn đề ảnh hưởng đến hoạt động của khách hàng. | IT Support / Nhân viên khách hàng | Thời gian phản hồi và số yêu cầu quan trọng bị xử lý trễ. |
| 6 | Pain từ người khác | Khi khách hàng yêu cầu hỗ trợ một vấn đề đã từng được xử lý, tôi muốn biết khách hàng mong đợi kết quả như thế nào và tình trạng xử lý trước đây ra sao, để tránh xử lý không đúng yêu cầu hoặc gây ra sự không hài lòng. | Khách hàng/IT Support | Tỷ lệ yêu cầu xử lý lại |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Sau khi tự scan 5 ý đầu, tôi hỏi AI và giữ lại ý 6, đồng thời chỉnh sửa lại ý "muốn biết rõ các phương án xử lý các tình huống phổ biến nhất" vì nó quá rộng và mơ hồ

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Thiếu thông tin về quy trình và cấu hình đặc thù của từng khách hàng. | Xuất hiện thường xuyên, đặc biệt khi phục vụ nhiều khách hàng có môi trường khác nhau. | Thông tin nên được tổng hợp ở đâu và như thế nào? |
| 2 | Khi nhiều yêu cầu hỗ trợ đến trong cùng một khoảng thời gian | Có thể làm tăng thời gian xử lý các trường hợp ít nguy cấp, đặc biệt nếu khách hàng ở một văn phòng lớn | Ưu tiên theo tiêu chí hay sự cố nào? |
| 3 | Không biết trước tình trạng thiết bị và môi trường IT khi đi hỗ trợ. | Có thể làm tăng số lần di chuyển và kéo dài thời gian xử lý. | Khách hàng có biết rõ về các thiết bị công ty hay không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story |Lặp lại | Khi cài đặt máy tính hay máy in mới cho khách hàng, tôi muốn biết chính xác danh sách phần mềm, driver và cấu hình tương ứng theo từng khách hàng, để không bỏ sót bước và không phải hỏi lại đồng nghiệp.  |
| Actor | Intern/Fresher IT Support |
| Thời điểm / bối cảnh | Mỗi khi đến cài đặt máy tính cho khách hàng |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận yêu cầu khách hàng ; 2. Cài OS, các phần mềm thiết yếu (theo công ty yêu cầu) và driver ; 3. Bàn giao và lắp đặt máy tính mới ; 4. Thiết lập, kết nối mạng và cài driver máy in đang sử dụng|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4, thường mất khoảng 25-30 phút để tìm thông tin máy tính hoặc máy in đang dùng |
| Impact (nếu không giải thì sao) | Việc lắp đặt toàn bộ máy có thể kéo dài cả 1 buổi (3-4 tiếng) |
| Success metric (baseline → target) | Thời gian lắp đặt chỉ nên kéo dài xuống 20 phút/1 máy  |
| Phương án không dùng AI | Tạo ticket bao gồm sẵn quy trình làm việc và cấu hình trong công ty khách, tạo 1 script Powershell để tự động hoá quy trình |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
[Tiếp nhận yêu cầu khách hàng] -> [Cài OS, các phần mềm thiết yếu (theo công ty yêu cầu) và driver: 30'-40'] -> [Bàn giao và lắp đặt máy tính mới: 15'] -> [Thiết lập máy tính, kết nối mạng và máy in] <- BOTTLENECK
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhiều nhân viên cùng gửi yêu cầu hỗ trợ trong một khoảng thời gian, tôi muốn biết mức độ ảnh hưởng và mức độ ưu tiên của từng yêu cầu, để không bỏ sót những vấn đề ảnh hưởng đến hoạt động của khách hàng. |
| Actor | Intern/Fresher IT Support |
| Thời điểm / bối cảnh | Khi nhiều nhân viên gửi yêu cầu hỗ trợ trong cùng một khoảng thời gian |
| Quy trình hiện tại (3–7 bước) |1. Bắt đầu nhận hỗ trợ từ khách ; 2. Sắp xếp công việc ; 3. Xử lý theo mức độ ảnh hưởng và mức độ ưu tiên  |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, vì cần thời gian khoảng 1-2 phút để xác định thứ tự ưu tiên cho từng yêu cầu |
| Impact (nếu không giải thì sao) | mất thời gian làm việc ít quan trọng |
| Success metric (baseline → target) | Số việc làm ưu tiên cao được giải quyết đúng hạn |
| Phương án không dùng AI | tạo dashboard bao gồm mưc độ ưu tiên  |
| Giả thuyết về AI (nếu có) | AI phân loại mức độ ưu tiên của yêu cầu hỗ trợ  |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
[Nhận hỗ trợ của khách] -> [Sắp xếp công việc] <- BOTTLENECK -> [Xử lý theo mức độ ảnh hưởng]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi hỗ trợ một khách hàng mới hoặc một môi trường IT chưa quen thuộc, tôi muốn nắm được tổng quan hệ thống, thiết bị, phần mềm và các cấu hình đặc thù của khách hàng, để không phải đọc nhiều tài liệu rời rạc trước khi bắt đầu công việc. |
| Actor | Intern/Fresher IT Support |
| Thời điểm / bối cảnh | Hỗ trợ 1 khách hàng mới |
| Quy trình hiện tại (3–7 bước) | 1. Nhận nhiệm vụ hỗ trợ ; 2. Đến vị trí khách hàng ; 3. Thực hiện công việc cần hỗ trợ  |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, vì cần 5-10 phút để đọc các tài liệu thiết bị, và khoảng 10 phút để tìm hiểu các cấu hình của khách hàng |
| Impact (nếu không giải thì sao) | mất thời gian để xử lý vấn đề |
| Success metric (baseline → target) | Lượng thông tin có thể nắm được |
| Phương án không dùng AI | Tạo 1 bảng liệt kê các thiết bị và cấu hình, workflow máy in và scan của từng khách hàng |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI |

Quy trình nháp hiện tại:

```text
[Nhận nhiệm vụ cần hỗ trợ] -> [Đến vị trí khách hàng: 15'-60' tuỳ vào địa điểm] -> [Thực hiện công việc cần hỗ trợ] <- BOTTLENECK
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Vấn đề thường xảy ra trong quá trình làm IT Support
- Câu hỏi muốn nhóm phản biện: Với nhiều khách hàng có cấu hình và thiết bị khác nhau, làm sao để giải quyết cùng 1 vấn đề cho 2 khách khác nhau mà không cần phải tự tìm hiểu thêm

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Actor chưa cụ thể | Đồng ý | Sửa thành Intern/Fresher IT Support |
| Đang nhảy sang AI quá sớm | Đồng ý một phần | Bỏ đi phần nhờ AI tự động hoá quy trình cài đặt phần mềm |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch problem card của bản thân và thảo luận các problem của nhóm | Sau khi thảo luận, problem cards của tôi đã không được chọn |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Người học quên kiến thức có phải do người đấy lười ôn tập hay những lí do khác? | Đi tìm nguyên nhân cốt lõi trước khi đưa ra giải pháp phù hợp |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | Cùng nhóm gom 12 candidate thành 3 cluster: A (khó ghi nhớ kiến thức), B (thiếu phương pháp ôn tập), C (thiếu công cụ theo dõi tiến độ). Các candidate IT của tôi không thuộc cluster nào nên không đi tiếp | Cây OST có 1 outcome (ghi nhớ kiến thức lâu hơn) và 3 opportunity. Nhóm gạch bỏ 3 ý là solution đội lốt opportunity (AI tạo câu hỏi, nhắc lịch ôn, flashcard) |
| Chọn candidate problem | Tham gia thảo luận chấm điểm shortlist theo 7 tiêu chí | Chọn candidate B “Người học chưa biết cách và thời điểm ôn tập phù hợp” (31/35, cùng điểm với A nhưng hẹp hơn, dễ can thiệp hơn). Loại A vì quá rộng, loại C vì cần cách đánh giá ghi nhớ rõ ràng hơn |
| Kiểm chứng / research | Cùng nhóm phỏng vấn 3 học viên trong lớp và xem các công cụ có sẵn (Anki, Quizlet, RemNote, NotebookLM, Mochi, Notion) cùng 2 nghiên cứu về đường cong lãng quên và hiệu ứng tự kiểm tra | Những người được hỏi đều gặp tình trạng quên kiến thức, nên kết quả không gây bất ngờ. Research cho thấy khoảng trống là tạo câu hỏi tổng hợp từ ghi chú của người học và chấm câu trả lời dạng giải thích. Đây là chỗ duy nhất cần AI |
| Quy trình nhóm | Tham gia vẽ quy trình hiện tại (5 bước) và quy trình tương lai (6 bước) | Quy trình tương lai: người học chọn khái niệm → Rule (Anki/FSRS) xếp lịch → AI tạo câu hỏi → người học tự trả lời → AI chấm → người học xem lại. Thời gian dự kiến ~14 phút/lần ôn, nhớ lại khi làm lab dưới 5 phút |
| Problem Statement | Tham gia viết và sửa Problem Statement từ v0 sang v1 | v1 thu hẹp Actor thành học viên AI20K, thêm chỉ số “tỉ lệ ngày có ôn”, và tách rõ phần Rule quyết lịch với phần AI tạo câu hỏi và chấm |
| Mức can thiệp AI | Tham gia so sánh 4 mức No AI / Rule / Workflow / Agent | Chọn Workflow: Rule xếp lịch, AI chỉ tạo câu hỏi và chấm, người học luôn xem lại kết quả. Không chọn Agent vì các bước cố định và dễ phát sinh kiến thức ngoài tài liệu |
| Quyết định | Tham gia đánh giá 4 rủi ro (Value, Usability, Viability ở mức Trung bình; Feasibility ở mức Thấp) | Quyết định Go, phạm vi nhỏ: pilot 2 tuần với 3–5 học viên, không xây app, có ngưỡng dừng rõ ràng |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm problem theo vai trò IT Support | Liệt kê được các tình huống tôi đã từng gặp phải trong quá trình làm việc | Chưa có số liệu cụ thể | Sửa lại ý "muốn biết rõ các phương án xử lý các tình huống phổ biến nhất" |
| CP2 Problem Card | Đánh giá các problem card tự viết | Đánh giá được những điểm còn thiếu sót trong problem card của tôi | | Cụ thể hoá Actor và bỏ phần không cần thiết sử dụng AI |
| CP4 Research | | | | |
| CP5 Quy trình | Nhờ AI nhận xét Problem Statement v0 | Chỉ ra 3 điểm yếu: Actor quá rộng, baseline chỉ là ước lượng của một người, chưa rõ AI làm bước nào và Rule làm bước nào | Các nhận xét còn chung, chưa nói cách sửa cụ thể | Nhóm đồng ý cả 3 điểm: thu hẹp Actor, ghi rõ baseline là ước tính và sẽ đo lại trong pilot, bổ sung phân vai AI/Rule ở v1 |
| CP5–6 Problem Statement | Nhờ AI kiểm tra Problem Statement v1 và đề xuất tiêu chí đánh giá đầu ra | Gợi ý được các tiêu chí kiểm tra đầu ra của AI như bám nguồn, có câu tổng hợp, chấm đúng | Tiêu chí còn chung chung nếu không có ngưỡng “đạt/không đạt” | Nhóm đặt ngưỡng cụ thể, ví dụ chấm khớp người chấm ít nhất 8/10 câu, 3–5 câu làm xong trong 10 phút |
| CP6 Mức can thiệp / quyết định | Nhờ AI so sánh 4 mức No AI / Rule / Workflow / Agent | Giúp thấy Anki (Rule) đã đủ cho nhắc lịch, nên AI chỉ cần ở phần tạo câu hỏi và chấm | AI có xu hướng đề xuất giải pháp phức tạp hơn mức cần thiết | Nhóm chọn Workflow, không chọn Agent, và đặt ngưỡng dừng để quay về Rule hoặc No AI nếu AI không hiệu quả |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Thông qua top 3 problems của các bạn khác, tôi thấy họ có những vấn đề giống tôi, nhưng cũng có những vấn đề đặc thù do môi trường và công việc của họ

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Nhóm đã tuân thủ hướng dẫn của mentor, nên hầu như không bị "solution-first"

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Tôi không đổi ý sau khi bị phản biện

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Không bất ngờ, hầu như những người được hỏi cũng đều gặp chung tình trạng quên kiến thức sau một thời gian học

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó khăn nhất nằm ở phần phân loại, một số vấn đề có thể thuộc về nhiều hơn 1 nhóm.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, minh muốn có thể pitch được problem gần với vấn đề chung của nhóm hơn

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
