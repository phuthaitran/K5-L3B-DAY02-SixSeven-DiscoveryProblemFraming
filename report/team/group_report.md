# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: SixSeven
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Người học chưa biết cách và thời điểm ôn tập phù hợp, nên học xong 1–2 tuần cần dùng lại thì đã quên, mỗi lần mất khoảng 20 phút đọc lại slide mà vài ngày sau lại quên tiếp.
- Quyết định cuối: **Go, phạm vi nhỏ** (pilot 2 tuần, không xây app)

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 |Minh |Khi chuẩn bị cho các buổi dạy thêm hằng tuần, tôi muốn xây dựng giáo án đầy đủ, có cấu trúc và phù hợp với nội dung cần dạy.  |Giáo viên dạy thêm, gia sư | Phải tìm kiếm, đọc, chọn lọc và biên soạn nội dung từ nhiều nguồn khác nhau. Thời gian thực tế cần được ghi nhận qua từng buổi soạn bài. |trong sách giáo khoa có đầy đủ nhưng do giáo viên soạn ko chuẩn bị theo thì thực tế trong sách chỉ đủ kiến thức cơ bản và không thể chỉ dạy mỗi kiến thức cơ bản cho học sinh vì sẽ ảnh hưởng tới kết quả thi và học tập của học sinh.(Bảo Minh) |
| 2 |Minh |Khi học một kiến thức mới hoặc tham gia một buổi học, tôi muốn có thể ghi nhớ và truy xuất lại kiến thức đã học sau một khoảng thời gian để sử dụng chúng trong những tình huống tiếp theo. |Học sinh, sinh viên, người tự học, nhân viên tham gia đào tạo. |Kiến thức không được ôn tập hoặc truy xuất thường xuyên, dẫn đến khó nhớ lại. Cần đo thời gian đọc lại và số lần phải học lại. |Vậy có phải do người đấy lười ôn tập hay những lí do khác.(Thái) |
| 3 |Minh |Khi nhóm bắt đầu một công việc hoặc dự án mới có liên quan đến những công việc trước đây, tôi muốn truy xuất và áp dụng các bài học kinh nghiệm cũ để tránh lặp lại sai lầm và nâng cao hiệu quả thực hiện. |Nhân viên, thành viên nhóm dự án, trưởng nhóm |Kinh nghiệm cũ khó được nhớ lại hoặc tìm kiếm. Thời gian tìm kiếm thực tế cần được đo bằng cách theo dõi một số nhiệm vụ. |Nếu kinh nghiệm cũ khó được nhớ lại hoặc tìm kiếm, làm thế nào để xác định vấn đề thực sự nằm ở việc nhân viên không ghi chép, hệ thống lưu trữ chưa hiệu quả hay quy trình tìm kiếm còn phức tạp?(Duyệt)  |
| 4 | Đào Lê Bảo Minh | Khi làm lab mới cần kiến thức 1–2 tuần trước, muốn nhớ lại nhanh và biết mình còn hiểu tới đâu | Học viên AI20K | Đọc lại slide 10–30 phút chỉ tạo cảm giác quen; không có bước ôn giãn cách | "NotebookLM đã tổng hợp tài liệu, quên thì hỏi lại là nó trích xuất nhanh, vậy sao vẫn là problem?" (Duyệt) · "Quên là do không ôn thường xuyên, phương pháp học chưa hợp hay do lượng kiến thức quá lớn?" (Hoàng Minh) |
| 5 | Đào Lê Bảo Minh | Khi cần tìm lại link, hướng dẫn lab hay thông báo cũ, muốn tìm ra ngay | Học viên AI20K, nhận tin từ 5 nguồn | Search không ra phải kéo lại tin nhắn, ~15 phút/lần | |
| 6 | Đào Lê Bảo Minh | Khi số điện có ngày tăng đột biến, muốn biết nguyên nhân để chỉnh thói quen | Người thuê trọ | Chỉ đoán nguyên nhân rồi bỏ qua | |
| 7 | Duyệt | Khi phải theo dõi thông báo từ 10+ kênh, muốn thấy ngay tin quan trọng để không lỡ deadline | Học viên | Lọc tin quan trọng ~10 phút/ngày, lỡ 2–3 thông báo/tuần | "Vấn đề bạn gặp có giống vấn đề của Minh không?" (thành viên nhóm) |
| 8 | Duyệt | Khi học nhiều kiến thức mới, muốn nhớ lại được nội dung đã học | Học viên | Tìm/lướt lại ghi chú ~15 phút/lần, hơn 30 phút/ngày | |
| 9 | Duyệt | Khi nhiều việc học, làm, cá nhân cùng lúc, muốn biết nên làm việc nào trước | Học viên vừa học vừa làm | Quyết định thứ tự ~7 phút/ngày, tuần trước trễ 2–3 việc | |
| 10 | Thái | Khi cài đặt máy cho khách, muốn biết sẵn cấu hình và quy trình đặc thù của khách đó | Intern/Fresher IT Support | Tìm thông tin máy tính, máy in đang dùng ~25–30 phút | |
| 11 | Thái | Khi nhiều yêu cầu hỗ trợ đến cùng lúc, muốn biết xử lý cái nào trước | Intern/Fresher IT Support | Xếp ưu tiên các yêu cầu | |
| 12 | Thái | Khi đi hỗ trợ, muốn biết trước tình trạng thiết bị của khách | Intern/Fresher IT Support | Phải di chuyển nhiều lần mới đủ thông tin | |

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
Duyệt hỏi nếu NotebookLM đã trích xuất kiến thức cũ rất nhanh thì vì sao vẫn là problem. Nhóm không bỏ candidate mà đưa NotebookLM vào bảng research (mục 3.3) để kiểm tra nó làm được tới đâu: tra cứu nhanh nhưng không nhắc ôn, nên không giải được chuyện "ôn lúc nào, ôn thế nào".

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
| NotebookLM | https://notebooklm.google/ | Tra cứu, hỏi lại kiến thức từ tài liệu đã tải lên | Trả lời nhanh, có trích nguồn từ chính tài liệu | Không nhắc ôn; hỏi lại để tra cứu khác với tự nhớ ra | Giải được bước "tìm lại", chưa giải được "giữ được kiến thức" |
| Mochi | https://mochi.cards/ | Viết thẻ ôn bằng markdown, ôn giãn cách | Gọn, viết thẻ nhanh hơn Anki | Vẫn là thẻ hỏi–đáp, người học tự viết thẻ | Cùng khoảng trống với Anki: thiếu câu tổng hợp và chấm bài |
| Notion | https://www.notion.com/ | Lưu và tổ chức ghi chú | Gom ghi chú một chỗ, dễ tìm | Không nhắc ôn, không kiểm tra người học | Giải được bước "lưu và tìm lại", không giải được "ôn lúc nào" |
| Murre & Dros (2015), lặp lại đường cong lãng quên Ebbinghaus | https://doi.org/10.1371/journal.pone.0120644 | Cơ sở của vấn đề | Xác nhận phần lớn kiến thức rơi rụng ngay trong ngày đầu | Đo trên âm tiết vô nghĩa, không phải kiến thức thật | Quên là mặc định, phải có ôn chủ động |
| Roediger & Karpicke (2006), hiệu ứng tự kiểm tra | https://doi.org/10.1111/j.1467-9280.2006.01693.x | Cơ sở cho cách ôn | Sau 1 tuần, nhóm tự kiểm tra nhớ tốt hơn hẳn nhóm chỉ đọc lại | Thí nghiệm với văn bản ngắn | Ôn phải là **tự trả lời câu hỏi**, không phải đọc lại |

**Kết luận research:** bước "nhắc ôn đúng lúc" đã có Anki làm bằng thuật toán (Rule). Bước "tra cứu lại" đã có NotebookLM. Khoảng trống còn lại là **tạo câu hỏi tổng hợp từ đúng ghi chú của người học và chấm câu trả lời dạng giải thích**. Đây là chỗ duy nhất cần AI.

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

```text
TƯƠNG LAI — ôn ~14 phút/lần; khi làm lab chỉ cần tra lại ghi chú

[1 Sau buổi học: chọn 3–5 khái niệm chính, lưu ghi chú: 5']   ← CON NGƯỜI
→ [2 Xếp lịch ôn giãn cách: 0']                                ← RULE (Anki / FSRS)
→ [3 Đến ngày ôn: tạo 3–5 câu hỏi tổng hợp từ đúng ghi chú: 1'] ← AI
→ [4 Tự trả lời, không xem tài liệu: 5']                        ← CON NGƯỜI
→ [5 Chấm, chỉ ra ý còn thiếu, kèm trích đoạn ghi chú: 1']      ← AI
→ [6 Xem lại kết quả chấm, sửa nếu AI chấm sai: 2']             ← CON NGƯỜI (HITL)
→ kết quả đưa lại vào lịch ôn                                   ← RULE

BOUNDARY: AI chỉ dùng ghi chú/slide người học đưa vào, không tự thêm kiến thức ngoài;
          AI không tự quyết lịch ôn (Rule quyết) và không tự sửa, xóa ghi chú;
          kết quả chấm chỉ được ghi nhận sau khi người học xem lại.
PHƯƠNG ÁN QUAY VỀ: câu hỏi lạc đề hoặc chấm sai → bỏ câu đó, ôn bằng thẻ Anki tự tạo
          hoặc bộ 10 câu tự kiểm tra viết sẵn sau buổi học.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 (học lại nhiều lần) | 6 | Thêm bước nhưng mỗi bước ngắn và có chủ đích |
| Tổng thời gian | ~20 phút/lần nhớ lại × ~3 lần/tuần | ~14 phút/lần ôn; nhớ lại khi làm lab dưới 5 phút | Thời gian chuyển từ "học lại khi đã quên" sang "ôn trước khi quên" |
| Số bước thủ công | 5/5 | 3/6 | Người học vẫn tự trả lời và tự xem lại chấm |
| Bottleneck chính | Đọc lại slide | Tự trả lời câu hỏi | Chấp nhận được, vì đây chính là bước luyện nhớ |
| Rủi ro mới phát sinh | — | AI hỏi ngoài ghi chú, chấm sai; người học bỏ ôn | Xử lý bằng boundary, bước 6 và ngưỡng dừng |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Người học và người đi làm phải tiếp nhận nhiều kiến thức mới: học viên, nhân viên sau đào tạo hoặc họp rút kinh nghiệm |
| **Quy trình** | Học hoặc họp → ghi chú → khi cần dùng lại thì tìm và đọc lại tài liệu → quay lại làm việc |
| **Bottleneck** | Đọc lại 10–30 phút mỗi lần chỉ tạo cảm giác quen; không có bước ôn giãn cách nên lại quên |
| **Impact** | ~20 phút/lần × ~3 lần/tuần ≈ 60 phút/tuần/người (ước tính); sau 10 ngày chỉ nhớ ~3/10 khái niệm; ở tổ chức thì lặp lại lỗi cũ |
| **Success Metric** (baseline → target, cách đo) | Thời gian nhớ lại một khái niệm: ~20 phút → dưới 5 phút. Bộ 10 câu tự kiểm tra (viết ngay sau buổi học, làm lại sau 10 ngày, không xem tài liệu): ~3/10 → ≥7/10. Đo bằng tự ghi giờ và làm bộ câu hỏi trong 2 tuần |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI không tạo nội dung ngoài tài liệu người học đưa vào, không tự kết luận người học "đã nhớ". Người học xem lại kết quả chấm trước khi ghi nhận |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- Actor gộp cả học viên lẫn tổ chức nên quá rộng, khó dùng chung một metric. → **Đồng ý**, thu hẹp ở v1.
- Baseline ~20 phút và ~3/10 là ước lượng của một người. → **Đồng ý**, ghi rõ là ước tính và đo lại trong pilot.
- Chưa nói rõ AI làm bước nào, Rule làm bước nào. → **Đồng ý**, bổ sung ở v1.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **độ mơ hồ trung bình–cao, độ phức tạp thấp**.

Vì sao: câu hỏi tổng hợp và cách chấm bài giải thích không có một đáp án duy nhất (mơ hồ). Nhưng các bước thì cố định và không rẽ nhánh: lưu ghi chú → xếp lịch → tạo câu hỏi → trả lời → chấm → xem lại (ít phức tạp). Ô này hợp với Workflow, có AI ở một vài bước.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Sau mỗi buổi tự viết 10 câu tự kiểm tra, đặt nhắc lịch trên điện thoại để làm lại | Người học đủ kỷ luật tự viết câu hỏi | Tốn công viết câu hỏi nên dễ bỏ | Dùng làm phương án quay về |
| **Rule** | Anki + FSRS xếp lịch ôn giãn cách với thẻ tự tạo | Kiến thức dạng định nghĩa, hỏi–đáp ngắn | Không luyện được câu giải thích, tổng hợp | **Dùng cho bước xếp lịch** |
| **Workflow** | Rule xếp lịch → AI tạo câu hỏi tổng hợp từ ghi chú → người học trả lời → AI chấm → người học xem lại | Các bước cố định, AI chỉ làm phần ngôn ngữ | Câu hỏi lạc đề, chấm sai | **Chọn** |
| **Agent** | AI tự quyết học gì, tự tìm tài liệu, tự lên lịch và tự đánh giá | Khi bước tiếp theo không đoán trước được | Tự thêm kiến thức ngoài, khó kiểm soát, người học dựa dẫm | Không chọn |

**Mức chọn:** Workflow.

**Vì sao không chọn mức đơn giản hơn:** Anki (Rule) đã làm tốt phần nhắc ôn đúng lúc, nhưng chỉ có thẻ hỏi–đáp ngắn và người học phải tự tạo thẻ. Kiến thức kỹ thuật như trong khóa AI20K cần câu giải thích, so sánh, áp dụng, và cần được chấm. Phần này No AI và Rule không làm được. Ngược lại, các bước đều cố định nên không cần tới Agent.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | 3–5 câu hỏi tổng hợp từ ghi chú của một buổi học; kết quả chấm từng câu kèm ý còn thiếu |
| **Judgment** — con người cân nhắc, quyết định gì? | Người học chọn khái niệm nào cần nhớ, tự trả lời, và quyết định kết quả chấm có đúng không |
| **Action** — hành động cuối cùng là gì, ai làm? | Người học ôn lại phần còn thiếu; Rule cập nhật lịch ôn tiếp theo |
| **Outcome** — đo kết quả bằng gì? | Thời gian nhớ lại khi làm lab; điểm bộ 10 câu sau 10 ngày; tỉ lệ ngày có ôn |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Ghi chú hoặc slide của buổi học (có sẵn), câu trả lời của người học |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Những câu người học đánh dấu "AI chấm sai"; câu hỏi bị bỏ vì lạc đề |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: **augment**. Problem Card #1 của Đào Lê Bảo Minh ghi rõ người học muốn "biết mình còn hiểu tới đâu", tức là muốn được hỏi và được chấm, không muốn AI học thay. Việc tự trả lời là phần không thể giao cho AI.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: **báo nhầm là "đã nhớ"** tệ hơn, vì người học tưởng đã nắm và bỏ ôn, đến lúc làm lab mới lộ ra. Thiết kế xử lý bằng cách: khi không chắc thì AI chấm "chưa đạt" và luôn kèm trích đoạn ghi chú làm căn cứ, người học xem lại trước khi ghi nhận.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Học viên AI20K học nhiều chủ đề mới mỗi tuần, chưa có thói quen ôn định kỳ |
| **Quy trình** | Học → ghi chú → khi làm lab cần kiến thức 1–2 tuần trước thì tìm và đọc lại slide → làm tiếp |
| **Bottleneck** | Đọc lại slide 10–30 phút chỉ thấy quen; không có bước ôn giãn cách |
| **Impact** | ~20 phút/lần × ~3 lần/tuần (ước tính); sau 10 ngày chỉ nhớ ~3/10 khái niệm |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian nhớ lại: ~20 phút → dưới 5 phút; (2) bộ 10 câu sau 10 ngày: ~3/10 → ≥7/10; (3) ôn ít nhất 70% số ngày có lịch. Đo bằng tự ghi giờ và nhật ký ôn trong 2 tuần pilot với 3–5 học viên |
| **Boundary** | AI chỉ dùng ghi chú/slide người học đưa vào; không tự thêm kiến thức ngoài; không tự quyết lịch ôn; kết quả chấm chỉ ghi nhận sau khi người học xem lại |
| **AI intervention point** | Bước 3 (tạo câu hỏi tổng hợp) và bước 5 (chấm câu trả lời) trong quy trình tương lai |
| **Mức chọn** | Workflow |
| **Rủi ro & người kiểm tra** | Câu hỏi ngoài ghi chú, chấm sai, người học bỏ ôn → người học tự xem lại kết quả chấm; mỗi tuần đối chiếu với bộ 10 câu tự viết |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Actor | Người học và người đi làm, cả tổ chức | Học viên AI20K | Phản biện: actor quá rộng; học viên là nhóm kiểm chứng được ngay, tổ chức để hướng tiếp theo |
| Success Metric | Thời gian nhớ lại + bộ 10 câu | Thêm tỉ lệ ngày có ôn, ghi rõ cách đo trong pilot | Ôn giãn cách chỉ có tác dụng khi người học duy trì được |
| Boundary | Chung chung, chưa tách AI và Rule | Ghi rõ Rule quyết lịch, AI chỉ tạo câu hỏi và chấm | Sau khi so sánh 4 mức, mới thấy rõ phần nào cần AI |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Bám nguồn | Mọi câu hỏi truy được về một đoạn cụ thể trong ghi chú | Có câu hỏi về nội dung không có trong ghi chú |
| 2 | Có câu tổng hợp | Ít nhất 1/3 số câu yêu cầu giải thích, so sánh hoặc áp dụng | Toàn câu hỏi định nghĩa, học thuộc |
| 3 | Chấm đúng | Kết quả chấm khớp với người chấm (bạn cùng lớp) ở ít nhất 8/10 câu | Lệch quá 2/10 câu |
| 4 | Chỉ ra chỗ hổng | Phản hồi nêu đúng ý còn thiếu, kèm trích đoạn ghi chú | Chỉ ghi "sai" hoặc nhận xét chung chung |
| 5 | Vừa sức | 3–5 câu, làm xong trong 10 phút | Quá dài, người học bỏ dở |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Trung bình | Nhóm 8 và cả 5 nhóm trong cụm đều xác nhận có quên, nhưng mới là ý kiến; chưa chứng minh được Anki + NotebookLM là không đủ |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Trung bình | Đọc và sửa kết quả chấm thì dễ, nhưng phải tự trả lời và duy trì ôn đều, dễ bỏ |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Thấp | Anki/FSRS, NotebookLM và các mô hình ngôn ngữ đều có sẵn; dữ liệu là ghi chú của chính người học |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Trung bình | Chi phí nhỏ, nhưng cần hỏi quy định về việc đưa slide khóa học vào công cụ AI |

### 8.2. Kết luận

**Quyết định:** Go, phạm vi nhỏ

**Lý do:** không có rủi ro nào ở mức Cao. Feasibility thấp vì mọi công cụ đều có sẵn. Hai rủi ro Trung bình (Value, Usability) kiểm được ngay trong một pilot rẻ, không cần xây gì, nên chạy thử là cách nhanh nhất để có số liệu thật thay cho ước lượng.

**Nếu Go — pilot nhỏ nhất (2 tuần, 3–5 học viên AI20K):**

- Không xây app. Anki xếp lịch ôn giãn cách (Rule).
- Đến ngày ôn, học viên dán ghi chú của buổi đó vào một prompt chuẩn để AI tạo 3–5 câu hỏi tổng hợp; học viên tự trả lời, AI chấm và chỉ ra ý còn thiếu; học viên xem lại kết quả chấm.
- Mỗi người ghi: thời gian nhớ lại mỗi lần làm lab, điểm bộ 10 câu sau 10 ngày, số ngày có ôn, số câu AI chấm sai.
- Trước khi chạy: hỏi coach về quy định đưa slide khóa học vào công cụ AI (giả định #6).

**Nếu Not Yet — cần kiểm chứng gì trước:** —

**Nếu No-Go — nên làm gì thay AI:** —

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

- Nếu sau 2 tuần thời gian nhớ lại không xuống dưới 10 phút, hoặc bộ 10 câu không lên được ít nhất 5/10 → dừng, quay về Anki + bộ câu hỏi tự viết (Rule / No AI).
- Nếu AI chấm lệch với người chấm quá 2/10 câu → bỏ bước AI chấm, chỉ giữ AI tạo câu hỏi.
- Nếu học viên bỏ ôn quá 50% số ngày có lịch → dừng, xem lại vấn đề duy trì thói quen trước.

---

## 9. Hạn chế và hướng tiếp theo

- Các con số baseline (~20 phút, ~3/10) là ước tính của một người, chưa bấm giờ thật.
- Kiểm chứng ngoài nhóm mới dừng ở mức hỏi nhóm 8 và sự đồng tình sau pitch, chưa có phỏng vấn sâu theo The Mom Test. Pilot 2 tuần sẽ bù phần số liệu hành vi.
- Hướng tiếp theo: vấn đề tổ chức lặp lại lỗi cũ sau họp rút kinh nghiệm (candidate #3) là hướng tiềm năng cho vòng sau.

## 10. Tài liệu tham khảo

- Murre, J. M. J., & Dros, J. (2015). Replication and Analysis of Ebbinghaus' Forgetting Curve. *PLOS ONE*. https://doi.org/10.1371/journal.pone.0120644
- Roediger, H. L., & Karpicke, J. D. (2006). Test-Enhanced Learning. *Psychological Science*. https://doi.org/10.1111/j.1467-9280.2006.01693.x
- Anki: https://apps.ankiweb.net/ · FSRS: https://github.com/open-spaced-repetition/fsrs4anki
- NotebookLM: https://notebooklm.google/ · Quizlet: https://quizlet.com/ · RemNote: https://www.remnote.com/ · Mochi: https://mochi.cards/ · Notion: https://www.notion.com/
- Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md)
