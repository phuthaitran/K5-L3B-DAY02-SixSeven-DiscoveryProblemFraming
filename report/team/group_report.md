# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 |Minh |Khi chuẩn bị cho các buổi dạy thêm hằng tuần, tôi muốn xây dựng giáo án đầy đủ, có cấu trúc và phù hợp với nội dung cần dạy.  |Giáo viên dạy thêm, gia sư | Phải tìm kiếm, đọc, chọn lọc và biên soạn nội dung từ nhiều nguồn khác nhau. Thời gian thực tế cần được ghi nhận qua từng buổi soạn bài. |trong sách giáo khoa có đầy đủ nhưng do giáo viên soạn ko chuẩn bị theo thì thực tế trong sách chỉ đủ kiến thức cơ bản và không thể chỉ dạy mỗi kiến thức cơ bản cho học sinh vì sẽ ảnh hưởng tới kết quả thi và học tập của học sinh.(Bảo Minh) |
| 2 |Minh |Khi học một kiến thức mới hoặc tham gia một buổi học, tôi muốn có thể ghi nhớ và truy xuất lại kiến thức đã học sau một khoảng thời gian để sử dụng chúng trong những tình huống tiếp theo. |Học sinh, sinh viên, người tự học, nhân viên tham gia đào tạo. |Kiến thức không được ôn tập hoặc truy xuất thường xuyên, dẫn đến khó nhớ lại. Cần đo thời gian đọc lại và số lần phải học lại. |Vậy có phải do người đấy lười ôn tập hay những lí do khác.(Thái) |
| 3 |Minh |Khi nhóm bắt đầu một công việc hoặc dự án mới có liên quan đến những công việc trước đây, tôi muốn truy xuất và áp dụng các bài học kinh nghiệm cũ để tránh lặp lại sai lầm và nâng cao hiệu quả thực hiện. |Nhân viên, thành viên nhóm dự án, trưởng nhóm |Kinh nghiệm cũ khó được nhớ lại hoặc tìm kiếm. Thời gian tìm kiếm thực tế cần được đo bằng cách theo dõi một số nhiệm vụ. |Nếu kinh nghiệm cũ khó được nhớ lại hoặc tìm kiếm, làm thế nào để xác định vấn đề thực sự nằm ở việc nhân viên không ghi chép, hệ thống lưu trữ chưa hiệu quả hay quy trình tìm kiếm còn phức tạp?(Duyệt)  |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A. Khó ghi nhớ kiến thức  |Học xong nhưng một thời gian sau quên kiến thức; đọc lại bài nhưng chỉ nhớ mang máng; khó nhớ lại khái niệm khi cần sử dụng. |Kiến thức không được ghi nhớ lâu dài hoặc khó truy xuất khi cần. |
| B. Thiếu phương pháp ôn tập |Không biết nên ôn lại kiến thức nào; không có lịch ôn tập; thường chỉ đọc lại bài trước kỳ thi. |Việc ôn tập thiếu hệ thống và chưa đúng thời điểm. |
| C. Thiếu công cụ theo dõi tiến độ |Không biết mình đã nhớ hay quên phần nào; khó tìm lại kiến thức cũ; không biết cần luyện tập thêm nội dung nào. |Người học thiếu cơ chế theo dõi và đánh giá khả năng ghi nhớ. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giúp người học ghi nhớ kiến thức lâu hơn và có thể
truy xuất, vận dụng kiến thức khi cần.
│
├── Opportunity A: Người học khó nhớ lại kiến thức đã học sau một
│   khoảng thời gian.
├── Opportunity B: Người học chưa biết cách và thời điểm ôn tập
│   phù hợp để hạn chế quên kiến thức.
└── Opportunity C: Người học khó xác định nội dung nào đã nhớ,
    nội dung nào cần ôn tập thêm.
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- Ứng dụng AI tự động tạo câu hỏi và bài tập ôn tập.

- Tính năng nhắc nhở người học ôn tập theo lịch.

- Sử dụng flashcard để ghi nhớ kiến thức.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
|Người học khó nhớ lại kiến thức sau một khoảng thời gian |5 |4 |3 |4 |5 |5 |5 |31 |
|Người học chưa biết cách và thời điểm ôn tập phù hợp |5 |4 |3 |4 |5|5 |5 |31 |
|Người học khó xác định nội dung nào đã nhớ và nội dung nào cần ôn thêm |5 |4 |3 |4 |4 |5 |5 |30 |

**Candidate được chọn:**
Người học chưa biết cách và thời điểm ôn tập phù hợp 
**Vì sao chọn:**
Đây là vấn đề gần gũi với trải nghiệm học tập của các thành viên trong nhóm.
Có thể xác định quy trình hiện tại: học bài → ghi chép → ôn tập không thường xuyên → quên kiến thức → phải học lại.
**Vì sao loại các candidate còn lại:**
Candidate A: Đây là vấn đề cốt lõi nhưng khá rộng, khó xác định một nguyên nhân cụ thể để can thiệp trong phạm vi lab.
Candidate C: Có liên quan chặt chẽ đến Candidate B nhưng cần xây dựng cách đánh giá khả năng ghi nhớ và theo dõi tiến độ tương đối rõ ràng.
**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 |Nhiều người học thường quên kiến thức sau một khoảng thời gian nếu không ôn tập lại. |Value |5 |3 |Có |
| 2 |Người học gặp khó khăn trong việc xác định khi nào cần ôn tập lại kiến thức. |Value |5 |2 |Có |
| 3 |Người học sẵn sàng sử dụng một ứng dụng hỗ trợ quản lý và nhắc nhở ôn tập. |Viability |4 |2 |Có |
| 4 |Người học có thể dễ dàng tải tài liệu hoặc nhập nội dung bài học lên ứng dụng. |Usability |3 |3 |Có |
| 5 |AI có thể tạo câu hỏi và bài tập ôn tập chính xác, bám sát nội dung tài liệu. |Feasibility	 |5 |2 |Có |
| 6 |Có thể xây dựng cơ chế đề xuất thời điểm ôn tập dựa trên kết quả làm bài của người học. |Feasibility |4 |2 |Có |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:
1. Người học thường quên kiến thức sau khi học nếu không ôn tập lại.
2. Người học không biết nên ôn tập nội dung nào và vào thời điểm nào.
3. Người học sẵn sàng sử dụng công cụ hỗ trợ ôn tập.
4. Câu hỏi do AI tạo ra có thể giúp người học tự kiểm tra mức độ ghi nhớ.
### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review
Phỏng vấn
Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) |Học viên trong lớp |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
|Phỏng vấn người học |3 |Người học kể lại tình huống thường xuyên quên bài hoặc không biết ôn phần nào |Người học có lịch ôn tập rõ ràng và ít gặp vấn đề này |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**
Người học gặp khó khăn trong việc xác định nội dung cần ôn tập và thời điểm ôn tập phù hợp, dẫn đến việc ôn tập thiếu hệ thống và khó ghi nhớ kiến thức lâu dài.
### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
|Anki |https://apps.ankiweb.net |Ôn tập kiến thức bằng flashcard theo lịch |Có cơ chế lên lịch ôn tập, hỗ trợ người học ghi nhớ lâu dài |Người học thường phải tự tạo thẻ; có thể mất thời gian chuẩn bị nội dung |Nên có cơ chế ôn tập theo lịch và theo dõi kết quả |
|Quizlet |https://quizlet.com |Tạo flashcard, đề kiểm tra và câu hỏi từ tài liệu |Có thể dùng AI chuyển ghi chú thành câu hỏi và bài kiểm tra |Câu hỏi AI tạo ra vẫn cần được người học kiểm tra lại; một số tính năng có giới hạn theo gói |Có thể tham khảo cách chuyển tài liệu thành bài tập luyện tập |
|Remnote |https://help.remnote.com/en |Ghi chú, tạo flashcard và ôn tập theo lịch |Kết hợp ghi chú với spaced repetition; có hỗ trợ tạo flashcard bằng AI |Có thể gây khó khăn cho người mới nếu phải thiết lập và quản lý nhiều nội dung |Nên kết hợp lưu trữ kiến thức và ôn tập trong cùng một quy trình |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
Người học tiếp nhận bài học
          |
          v
Ghi chép / lưu tài liệu
          |
          v
Tự đọc lại và ôn tập
          |
          v
Không nhớ rõ kiến thức
          |
          v
Tìm lại tài liệu / học lại
          |
          v
Tiếp tục ôn tập khi có nhu cầu
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1.Tiếp nhận kiến thức |Người học |Bài giảng, sách, tài liệu |Kiến thức mới |Theo lịch học |Tiếp nhận nội dung |
| 2.Ghi chép và lưu trữ |Người học |Kiến thức vừa học |Vở ghi, file tài liệu |Sau buổi học |Tùy thói quen mỗi người |
| 3. Ôn tập |Người học |Vở ghi, tài liệu cũ |Kiến thức được củng cố |Không cố định |Có thể chỉ ôn trước kỳ thi |
| 4. Kiểm tra khả năng ghi nhớ |Người học |Kiến thức đã học |Nhận biết phần nhớ và chưa nhớ |Khi làm bài hoặc tự kiểm tra |Chưa có cơ chế theo dõi liên tục |
| 5. Tìm lại và học lại |Người học |Nội dung đã quên |Kiến thức được xem lại |Khi cần sử dụng |Có thể mất thời gian tìm kiếm |

**Bottleneck chính:**
Người học chưa có phương pháp xác định nội dung cần ôn và thời điểm ôn tập phù hợp. Việc ôn tập phụ thuộc nhiều vào trí nhớ và thói quen cá nhân, khiến một số kiến thức chỉ được xem lại khi đã quên hoặc khi sắp kiểm tra.
### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
