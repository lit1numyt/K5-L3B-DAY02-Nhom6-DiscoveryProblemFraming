# CP6 — Mức can thiệp, Problem Statement v1 và quyết định

Phụ trách: Nguyễn Đức Khương Lam.

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Phân loại ban đầu là **mơ hồ thấp, phức tạp thấp** khi chỉ tìm lại một bằng chứng trong paper đã đọc và có PDF gốc. Đầu vào và thứ tự bước khá rõ; phần cần cân nhắc nằm ở việc bằng chứng có thật sự hỗ trợ nhận định trong đúng ngữ cảnh hay không.

**Điểm cần làm rõ:** quy trình có 5 bước nối tiếp, trong khi worksheet dùng số bước và mức phối hợp để xét độ phức tạp. Nhóm cần rà lại cách xếp ô trước khi chốt phân loại.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** | Ghi chú có cấu trúc: nhận định, paper, trang/hình/bảng, annotation/liên kết và ngữ cảnh; dùng Zotero mở lại nguồn | Người học tìm lại và xác minh được bằng chứng với tổng công phù hợp | Công chuẩn bị, thiếu/sai liên kết, hiểu sai ngữ cảnh | Ưu tiên thử trước; chưa triển khai |
| **Rule** | Keyword search hoặc BM25 trong paper đã chọn | No AI còn nghẽn và tìm kiếm theo quy tắc đủ đáp ứng | Nhận định diễn đạt lại không khớp từ khóa; kết quả liên quan nhưng chưa đủ căn cứ | Chỉ thử khi cần; nếu đủ thì dừng ở mức này |
| **Workflow** | Retrieval → AI gợi ý đoạn cùng vị trí nguồn → người học mở PDF xác minh → lưu kết quả | No AI/Rule chưa đủ và thử nghiệm cho thấy lợi ích về tổng thời gian, chất lượng | Trích dẫn sai, gợi ý không hỗ trợ nhận định, tăng công kiểm | Tùy chọn, chưa triển khai |
| **Agent** | AI tự chọn công cụ/nguồn và bước tìm tiếp theo | Chỉ cân nhắc nếu có bằng chứng cần quyền tự quyết vượt Workflow | Khó kiểm nguồn, mở rộng phạm vi và tăng chi phí | Chưa có cơ sở để chọn |

**Mức chọn để thử trước: No AI First.** Ghi chú có nguồn và liên kết Zotero xử lý trực tiếp giả thuyết thiếu vị trí. Người học vẫn kiểm ngữ cảnh và quay về tìm thủ công khi liên kết lỗi. Cách này cũng tốn công chuẩn bị, nên chưa kết luận hiệu quả trước khi đo.

**Vì sao không chọn mức đơn giản hơn / cao hơn:** sửa cách ghi chú và dùng công cụ sẵn có là điểm bắt đầu đơn giản nhất. Chỉ nâng mức khi cách trước chưa đủ; không thêm AI nếu No AI/Rule đã giải quyết được tác vụ. Các bước hiện đã rõ, chưa có lý do giao quyền tự quyết cho Agent.

### 6.3. AI Canvas rút gọn

Không áp dụng cho phương án No AI đang ưu tiên thử, theo hướng dẫn worksheet/rubric. Nhánh Workflow chưa được chọn hay triển khai; nếu chuyển mức, nhóm cần hoàn thiện Canvas theo dữ liệu và tác vụ thật.

### 6.4. Hai câu hỏi Google PAIR

Không bắt buộc với mức No AI. Nếu thử Workflow, cần làm rõ người dùng muốn được hỗ trợ hay giao việc và so sánh lỗi nhận nhầm bằng chứng với lỗi bỏ sót. Người học giữ quyền chấp nhận bằng chứng, không giao quyền đó cho AI.

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

### 7.1. Problem Statement v1

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên đang đọc và tổng hợp paper nghiên cứu; phạm vi thử là paper đã đọc và có PDF gốc được phép sử dụng. |
| **Quy trình** | Ghi chú → xác định paper → dò PDF → đọc ngữ cảnh → lưu vị trí nguồn. Phương án thử trước: structured notes/Zotero → mở liên kết → sinh viên kiểm ngữ cảnh → lưu bằng chứng đúng vị trí. |
| **Bottleneck** | Giả thuyết: tìm đúng đoạn, hình hoặc bảng khi ghi chú thiếu vị trí nguồn. Cần đo từng bước, tách khó định vị khỏi khó hiểu ngữ cảnh. |
| **Impact** | Có thể tốn thời gian đọc lại và dùng kết quả sai phạm vi; chưa có baseline, tần suất hoặc mức ảnh hưởng thực nghiệm. |
| **Success Metric** (baseline → target, cách đo) | Baseline: chưa có số đo thực nghiệm. Pilot dự kiến: 10 yêu cầu từ 3 paper được phép sử dụng, có cả yêu cầu không có đáp án. Target đề xuất: giảm ít nhất 30% tổng thời gian của No AI so với cách tìm hiện tại, tính cả chuẩn bị, tìm kiếm và xác minh, không giảm chất lượng. Đo retrieval time, evidence hit rate, citation accuracy và context correctness theo mục 7.3–7.4; báo cả tử số/mẫu số, ngoại lệ và lượt thất bại. |
| **Boundary** | Người học mở PDF gốc để kiểm nguồn, bằng chứng và ngữ cảnh trước khi chấp nhận. AI không tự tạo trích dẫn, bịa nguồn/số trang hoặc tự xác nhận độ đúng. Thiếu căn cứ thì ghi chưa tìm thấy và kiểm thủ công; không dùng nhận định chưa xác minh. |
| **AI intervention point** | Không có trong phương án No AI. Nhánh Workflow chỉ là tùy chọn khi mức đơn giản chưa đủ. |
| **Mức chọn** | No AI First để kiểm chứng; chưa triển khai AI. |
| **Rủi ro & người kiểm tra** | Liên kết sai, hiểu sai ngữ cảnh, công chuẩn bị lớn, PDF scan/hình/bảng khó truy xuất. Người học kiểm mỗi kết quả với PDF; người thực hiện pilot và người đối chiếu đáp án cần được nhóm phân công trước khi chạy. |

### 7.2. Thay đổi so với v0 và lý do

| Trường | v0 trong CP5 | v1 | Vì sao đổi |
|---|---|---|---|
| Actor / phạm vi | Sinh viên dùng lại nhận định từ paper đã đọc | Làm rõ có PDF gốc và quyền sử dụng; pilot ban đầu ưu tiên PDF tìm được văn bản | Có nguồn để đối chiếu, tránh mặc định đã xử lý tốt scan/hình/bảng |
| Success Metric | Target giảm ít nhất 30%, kiểm tốc độ và độ đúng | Làm rõ 10 yêu cầu/3 paper, có yêu cầu không có đáp án; định nghĩa các thước đo và tính công chuẩn bị | So sánh được tổng công và chất lượng, không bỏ lượt khó/không tìm thấy |
| Boundary | Người học kiểm PDF; AI nếu thử chỉ gợi ý | Ghi rõ chưa tìm thấy khi thiếu căn cứ, không để AI tự tạo vị trí nguồn; có ngưỡng dừng | Tránh coi nguồn tồn tại là đủ chứng minh nhận định |
| Mức can thiệp / người kiểm tra | Ưu tiên Zotero, AI có thể thử sau | No AI First; Workflow tùy chọn, không Agent; nhóm cần phân công người kiểm | Chỉ tăng mức khi có lợi ích đã đo và giữ quyền xác nhận ở con người |

### 7.3. Tiêu chí đánh giá

Dùng 5 tiêu chí dưới đây để đánh giá No AI và so sánh với mức cao hơn nếu thử tiếp. Ngưỡng chất lượng sẽ được chốt trước pilot.

| # | Tiêu chí | Cách đo / đạt khi | Không đạt / cần ghi nhận |
|---:|---|---|---|
| 1 | Retrieval time | Bấm giờ từ yêu cầu đến khi tìm được bằng chứng; báo trung vị thời gian mỗi yêu cầu, ghi riêng công xác minh | Chưa tìm được vẫn ghi thời gian và trạng thái; không bỏ khỏi log hoặc gán thời gian bằng 0 |
| 2 | Evidence hit rate | Số yêu cầu có đáp án tìm được bằng chứng hợp lệ / tổng yêu cầu có đáp án | Chỉ trùng từ khóa nhưng không hỗ trợ nhận định, hoặc bỏ sót bằng chứng; chất lượng không được giảm so với baseline |
| 3 | Citation accuracy | Số vị trí nguồn đúng / tổng trích dẫn đã lưu; đối chiếu paper và trang/đoạn/hình/bảng | Nhầm paper, vị trí, phiên bản hoặc nguồn không tồn tại |
| 4 | Context correctness | Số nhận định dùng đúng điều kiện và giới hạn / tổng nhận định đã lưu | Đúng trang nhưng diễn giải vượt bằng chứng hoặc bỏ điều kiện áp dụng |
| 5 | Tổng thời gian | Mục tiêu đề xuất giảm ít nhất 30% so với baseline, gồm công chuẩn bị + tìm kiếm + xác minh | Nhanh ở bước tìm nhưng tổng công không đạt mục tiêu, hoặc chất lượng giảm |

Với yêu cầu không có đáp án, chấm riêng việc nhận ra thiếu căn cứ và số gợi ý sai; không đưa vào mẫu số evidence hit rate của yêu cầu có đáp án. Báo tử số/mẫu số cho các tỷ lệ; mẫu số bằng 0 thì ghi không áp dụng. Một kết quả chỉ được chấp nhận sau khi người học kiểm cả nguồn, bằng chứng và ngữ cảnh.

### 7.4. Kế hoạch đo — chưa có kết quả thực nghiệm

1. Chuẩn bị **10 yêu cầu từ 3 paper** được phép sử dụng, có cả yêu cầu không có đáp án. Tạo đáp án tham chiếu gồm đoạn/hình/bảng, vị trí và giới hạn áp dụng; người đọc kiểm PDF trước.
2. Đo baseline bằng cách tìm thủ công hiện tại. Đo No AI với ghi chú có cấu trúc/Zotero; tính công chuẩn bị cho tập paper và thời gian xử lý toàn bộ yêu cầu, kể cả xác minh và fallback.
3. Đổi thứ tự phương án giữa người thử hoặc dùng tác vụ tương đương để giảm ảnh hưởng nhớ đáp án. Ghi log từng yêu cầu, lỗi bỏ sót/nhận nhầm và kết quả kiểm ngữ cảnh.
4. Gọi B là tổng thời gian baseline đã đo, T là tổng thời gian No AI gồm chuẩn bị. Mục tiêu đề xuất là T ≤ 0,70 × B (B > 0), đồng thời không giảm chất lượng. Chưa có giá trị B hoặc T thực nghiệm.
5. Nếu No AI/Rule chưa đủ mới cân nhắc Workflow và so với phương án đơn giản tốt nhất. Mười yêu cầu chỉ giúp phát hiện lỗi ban đầu, chưa đủ suy rộng hiệu quả hoặc độ tin cậy cho nhiều người dùng.

| Nội dung | Trạng thái hiện tại |
|---|---|
| Baseline, thời gian từng bước, công chuẩn bị | [CẦN ĐO] — chưa có baseline thực nghiệm |
| Bộ yêu cầu, đáp án tham chiếu và log thử | Chưa có bộ thử/log đính kèm; cần nhóm chuẩn bị trước pilot |
| Target giảm ít nhất 30% | Mục tiêu thử nghiệm đề xuất, không phải kết quả |
| Thời điểm, người thực hiện, người kiểm và ngưỡng chất lượng | [CẦN NHÓM XÁC NHẬN] trước khi chạy |

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

Đánh giá rủi ro khi cân nhắc triển khai AI:

| Rủi ro | Câu hỏi | Mức độ | Lý do / bằng chứng hiện có |
|---|---|---|---|
| **Value** | Pain có thật và đủ đáng giải quyết không? | Cao | Đã trao đổi với 2 sinh viên nhưng chưa có log tác vụ, tần suất hay baseline để đánh giá mức độ pain; chưa biết ghi chú/Zotero đã đủ chưa. |
| **Usability** | Người học có dùng và kiểm kết quả được không? | Trung bình | Công tạo ghi chú và kiểm lại có thể lớn; người học phải hiểu và giữ đúng ngữ cảnh. |
| **Feasibility** | Có truy xuất được bằng chứng trong phạm vi dữ liệu không? | Trung bình | PDF scan, hình và bảng có thể khó tìm; chưa có thử nghiệm. Pilot ban đầu ưu tiên PDF tìm được văn bản, trường hợp khó kiểm thủ công hoặc ghi ngoài phạm vi. |
| **Viability** | Quyền dùng tài liệu, chi phí và vận hành có phù hợp không? | Trung bình | Cần kiểm quyền sử dụng paper và tổng chi phí/công chuẩn bị; chưa có số đo để kết luận. |

### 8.2. Kết luận

**Đề xuất: Not Yet — Chưa đủ bằng chứng để triển khai AI.** Bước trước mắt là hoàn thiện kiểm chứng và thử No AI. Quyết định cuối sẽ được nhóm chốt sau khi xem kết quả.

**Lý do:** trao đổi trải nghiệm với 2 bạn cùng lớp chưa cho biết mức độ tốn thời gian hay vị trí nghẽn thực tế. Chưa có baseline và phép so sánh cho thấy No AI/Rule không đủ; vì vậy chưa có căn cứ để triển khai AI.

**Bước tiếp theo:** bổ sung trường hợp cụ thể từ người đã trao đổi → quan sát và đo baseline → thử No AI → so sánh kết quả. Pilot dự kiến gồm **10 yêu cầu từ 3 paper**, có yêu cầu không có đáp án; cách đo ở mục 7.4. Nếu còn bottleneck, thử Rule; nếu Rule đủ thì dừng ở đó, nếu chưa đủ mới cân nhắc Workflow để so sánh. Lịch, người thực hiện và người kiểm nguồn sẽ được phân công trước pilot.

**Ngưỡng dừng / điều kiện không nâng cấp:**

- Nếu có một trích dẫn sai được chấp nhận, dừng dùng đầu ra AI và xem lại bước kiểm nguồn/ngữ cảnh trước khi thử tiếp.
- Sau bộ pilot dự kiến, nếu tổng thời gian và chất lượng không tốt hơn phương án đơn giản, không nâng cấp lên AI; quay về No AI/Rule hoặc tìm thủ công, sửa quy trình rồi đo lại. Target giảm ít nhất 30% là mục tiêu thử No AI so với baseline, chưa phải kết quả đạt được.
- Chỉ đánh giá pilot khi đủ log tác vụ, thời gian chuẩn bị và kết quả kiểm chất lượng; nếu thiếu, tiếp tục giữ Not Yet.

**Khi nào cân nhắc Go:** có pain thực tế và baseline đã đo, No AI/Rule chưa đủ, Workflow đem lại lợi ích về tổng công mà không giảm chất lượng, có người kiểm PDF và ngưỡng dừng. Nếu đạt, chỉ cân nhắc pilot AI nhỏ sau khi nhóm xác nhận; chưa phải Go triển khai rộng.

---

## 9. Hạn chế và hướng tiếp theo

### 9.1. Việc còn thiếu

| Nội dung | Hiện có | Cần bổ sung |
|---|---|---|
| Phản biện trực tiếp | Nhóm đã thảo luận chọn đề tài. | Câu hỏi thực sự đã đặt/nhận và người hỏi ở mục 2.1. |
| Ghi chép phỏng vấn | Trao đổi trực tiếp với 2 sinh viên ngoài nhóm; ghi nhận việc dùng NotebookLM và lo ngại trích dẫn sai. | Ngày trao đổi, ghi nhận từng người, một tác vụ cụ thể và ví dụ đầu ra; tìm cả trường hợp cách hiện tại đã đủ dùng. |
| Kinh nghiệm nội bộ | Thành viên nhóm dùng trải nghiệm bản thân để nêu và đối chiếu tình huống. | Ghi lại trường hợp cụ thể; giữ riêng với nguồn phỏng vấn ngoài nhóm. |
| Quy trình và baseline | Có sơ đồ, actor/input/output, bước kiểm nguồn và fallback. | Quan sát thao tác thật, đo từng bước và công chuẩn bị. |
| Bộ eval | Kế hoạch 10 yêu cầu/3 paper, target giảm ít nhất 30%, các thước đo tốc độ và chất lượng. | Yêu cầu/đáp án có nguồn, trường hợp không có đáp án, log thử và ngưỡng chất lượng. |
| Ma trận độ phức tạp | Phân loại ban đầu là mơ hồ thấp, phức tạp thấp. | Rà lại cách áp dụng tiêu chí của worksheet cho quy trình 5 bước. |
| Quyết định và pilot | Đề xuất Not Yet đối với triển khai AI, thử No AI trước. | Chốt quyết định, lịch, người thử và người kiểm PDF sau khi hoàn thiện dữ liệu. |

### 9.2. Nguồn và sử dụng AI

Nguồn nội dung gồm các báo cáo cá nhân, shortlist, tài liệu công cụ, ghi nhận trao đổi với 2 sinh viên ngoài nhóm và kinh nghiệm của thành viên nhóm. Phần thuyết trình dùng `nhom6-paper-evidence-6min-v3.pptx` cùng `nhom6_kich_ban_thuyet_trinh_6_phut.pdf`; hai file này hiện được cung cấp riêng ngoài repo.

AI hỗ trợ tổng hợp tài liệu, soạn bản nháp slide/báo cáo, dựng sơ đồ và phản biện metric, boundary. Chi tiết sử dụng AI của Dương nằm trong báo cáo cá nhân, mục 5.

---

## 10. Tài liệu tham khảo

- [Card L1 — CP1–CP2 của Lam](../individual/2A202604020_NguyenDucKhuongLam.md), [shortlist](shortlist.md), [CP3 trong báo cáo nhóm](group_report.md#2-hội-tụ-nhóm-cp3).
- [CP4](CP4.md), [CP5](CP5.md), [CP6](CP6.md); [CP4 trước khi đồng bộ](https://github.com/lit1numyt/K5-L3B-DAY02-Nhom6-DiscoveryProblemFraming/blob/169d1927dce2f72cae879ac35dc90e8575901c3f/report/team/CP4.md).
- [Worksheet](../../docs/01-worksheet.md), [checklist](../../CHECKPOINTS.md), [rubric](../../RUBRIC.md), [quy định](../../RULES.md).
- [Zotero PDF Reader](https://www.zotero.org/support/pdf_reader), [Zotero Notes](https://www.zotero.org/support/notes).
- [Elicit — Which workflow should I use?](https://support.elicit.com/en/articles/14757543-getting-started-with-elicit-which-workflow-should-i-use).
- [Lewis và cộng sự (2020) — Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401).
- [Adobe — Searching PDFs](https://helpx.adobe.com/acrobat/using/searching-pdfs.html).
- Slide v3 và PDF kịch bản: tên file ghi tại mục 9.2.
