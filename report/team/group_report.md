# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Nhóm 6 — L3B
- Thành viên và phân công: xem [TEAM.md](../../TEAM.md). Khoa phụ trách CP5; An phụ trách CP4; Lam phụ trách CP6; Dương điều phối, tổng hợp nguồn, tích hợp báo cáo và làm slide.
- Candidate problem được chọn (1 câu): Sinh viên mất thời gian tìm lại đúng đoạn, hình hoặc bảng trong paper đã đọc để xác minh nhận định.
- Quyết định đề xuất: Not Yet — Chưa đủ bằng chứng để triển khai AI; ưu tiên thử No AI trước. Chờ nhóm xác nhận quyết định cuối.

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

Các thành viên đã thảo luận, đối chiếu các phương án rồi chọn shortlist và đề tài tìm lại bằng chứng trong paper. Bảng dưới tổng hợp candidate từ CP2 của bốn báo cáo cá nhân, dùng mã truy vết ở mục 2.2; chưa ghi lại câu hỏi phản biện cụ thể và người hỏi.

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Khoa | K1 — Khi chuẩn bị sprint, cần tìm và ghép thông tin dự án để hiểu bối cảnh công việc | Developer mới hoặc tham gia dự án có sẵn | Tìm, đọc và đối chiếu thông tin qua nhiều nguồn (bước 2–6 trong card) | |
| 2 | Khoa | K2 — Khi làm task trên hệ thống có sẵn, cần tìm kiến thức và quyết định kỹ thuật cũ để hiểu module | Developer làm việc với module chưa quen | Đọc code, tìm lịch sử và hỏi người từng phụ trách (bước 3–6) | |
| 3 | Khoa | K3 — Khi nhận backlog mới, cần hiểu yêu cầu và acceptance criteria để bắt đầu đúng phạm vi | Developer nhận task từ PO, PM hoặc Tech Lead | Làm rõ yêu cầu qua nhiều vòng trao đổi (bước 3–6) | |
| 4 | Dương | D1 — Khi review PR lớn, cần hiểu thay đổi và rủi ro để nhận xét có căn cứ | Developer được giao review PR | Giả thuyết: lần theo mã liên quan để hiểu tác động (bước 4) | |
| 5 | Dương | D2 — Khi điền nhiều biểu mẫu, cần xác định thông tin khách hàng để hoàn tất hồ sơ không bỏ sót | Nhân viên nhập thông tin khách hàng | Giả thuyết: nhập lại các trường trùng (bước 4) | |
| 6 | Dương | D3 — Khi nhận tiền điện, nước và dịch vụ, cần đối chiếu hợp đồng để kiểm khoản phải trả | Người thuê nhà | Giả thuyết: đối chiếu từng khoản với điều khoản và dữ liệu tính tiền (bước 4) | |
| 7 | Lam | L1 — Khi dùng lại nhận định trong paper đã đọc, cần tìm đúng bằng chứng để giải thích có căn cứ | Sinh viên mới tham gia nhóm nghiên cứu, bối cảnh giả định | Dò bằng chứng trong PDF (bước 3), chưa đo thực tế | |
| 8 | Lam | L2 — Khi có nhiều paper liên quan, cần xác định bài sát câu hỏi nghiên cứu để chọn bài đọc sâu | Sinh viên chọn paper, bối cảnh giả định | Đọc tiêu đề và abstract (bước 2), chưa đo thực tế | |
| 9 | Lam | L3 — Khi so điểm số giữa paper, cần kiểm điều kiện đánh giá để tránh kết luận thiếu căn cứ | Sinh viên lập bảng so sánh, bối cảnh giả định | Đối chiếu mô hình, dữ liệu và thiết lập (bước 4), chưa đo thực tế | |
| 10 | An | A1 — Khi rà soát biến thể tín hiệu, cần nhận biết khác biệt để chọn bước thử tiếp có căn cứ | Người nghiên cứu tín hiệu định lượng | Đối chiếu nhiều thay đổi và chỉ số (bước 3), thời gian phân rã là ước lượng | |
| 11 | An | A2 — Khi tiếp tục việc sau họp, cần rõ quyết định, người phụ trách và hạn để không bỏ sót cam kết | Người tổng hợp biên bản, bối cảnh giả định | Xác nhận người phụ trách và deadline (bước 3) | |
| 12 | An | A3 — Khi tra đề nghị mua vật tư, cần biết người đang xử lý và thông tin thiếu để bổ sung đúng chỗ | Nhân viên gửi đề nghị mua, bối cảnh giả định | Xác định người giữ hồ sơ và thông tin thiếu (bước 3) | |

### 2.2. Cluster

**[CHỜ NHÓM XÁC NHẬN]** Phân nhóm sơ bộ có hỗ trợ AI, từ CP1–CP2 của bốn báo cáo trên main tại commit 71f0e47. Pitch, phản biện trực tiếp và lựa chọn cuối do các thành viên thực hiện.

**Các candidate trong top 3 của từng thành viên**

Mã dưới đây dùng để truy vết card gốc. Cột ưu tiên pitch ghi lựa chọn trong báo cáo cá nhân, chưa phải kết quả pitch của nhóm.

| Mã | Thành viên / nguồn | Candidate CP2 và mã CP1 | Ưu tiên pitch |
|---|---|---|---|
| K1 | [Khoa — 2A202604000](../individual/2A202604000_DongHuuNguyenKhoa.md) | Card #1: Tìm kiếm và tổng hợp thông tin dự án; CP1 #1, #5 | Có |
| K2 | [Khoa — 2A202604000](../individual/2A202604000_DongHuuNguyenKhoa.md) | Card #2: Truy xuất kiến thức kỹ thuật và quyết định cũ; CP1 #4, #9 | — |
| K3 | [Khoa — 2A202604000](../individual/2A202604000_DongHuuNguyenKhoa.md) | Card #3: Hiểu backlog và làm rõ yêu cầu; CP1 #2, #7 | — |
| D1 | [Dương — 2A202604016](../individual/2A202604016_ChuNguyenTungDuong.md) | Card #1: Đọc Pull Request lớn; CP1 #6 | Có |
| D2 | [Dương — 2A202604016](../individual/2A202604016_ChuNguyenTungDuong.md) | Card #2: Nhập lại thông tin khách hàng; CP1 #12 | — |
| D3 | [Dương — 2A202604016](../individual/2A202604016_ChuNguyenTungDuong.md) | Card #3: Đối chiếu chi phí thuê nhà; CP1 #19 | — |
| L1 | [Lam — 2A202604020](../individual/2A202604020_NguyenDucKhuongLam.md) | Card #1: Tìm lại bằng chứng trong paper đã đọc; CP1 #1 | Có |
| L2 | [Lam — 2A202604020](../individual/2A202604020_NguyenDucKhuongLam.md) | Card #2: Sàng lọc paper sát câu hỏi nghiên cứu; CP1 #3 | — |
| L3 | [Lam — 2A202604020](../individual/2A202604020_NguyenDucKhuongLam.md) | Card #3: Đối chiếu điều kiện đánh giá giữa các paper; CP1 #7 | — |
| A1 | [An — 2A202604024](../individual/2A202604024_NguyenHuuAn.md) | Card #1: So sánh các biến thể tín hiệu định lượng; CP1 #2 | Có |
| A2 | [An — 2A202604024](../individual/2A202604024_NguyenHuuAn.md) | Card #2: Xác định quyết định, người phụ trách và deadline sau cuộc họp; CP1 #9 | — |
| A3 | [An — 2A202604024](../individual/2A202604024_NguyenHuuAn.md) | Card #3: Xác định trạng thái và thông tin thiếu của đề nghị mua vật tư; CP1 #8 | — |

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Tìm và hiểu thông tin theo ngữ cảnh | K1, K2, D1, L1, L2 | Phải tìm, đọc và nối thông tin liên quan trước khi sử dụng: bối cảnh dự án, mã nguồn hoặc tài liệu nghiên cứu. Tìm lại nguồn đã biết và sàng lọc nguồn mới là các bước khác nhau, cần giữ riêng khi phân tích từng card. |
| B — Đối chiếu kết quả nghiên cứu | L3, A1 | Nhiều chỉ số và điều kiện thử nghiệm cần được đối chiếu trước khi diễn giải khác biệt; chỉ nhìn kết quả có thể dẫn đến so sánh thiếu căn cứ. |
| C — Làm rõ thông tin và trách nhiệm trong phối hợp | K3, A2, A3 | Thông tin để tiếp tục công việc còn thiếu hoặc mơ hồ; phải tìm đầu mối và xác nhận lại yêu cầu, trách nhiệm hoặc trạng thái xử lý. |
| D — Nhập lặp dữ liệu khách hàng | D2 | Cùng thông tin phải điền qua nhiều biểu mẫu, sau đó kiểm tra sự nhất quán. |
| E — Đối chiếu khoản thu với hợp đồng thuê | D3 | Người thuê phải kiểm các khoản thu bằng điều khoản và chứng từ liên quan. |

A và C gom theo pattern, chưa đồng nghĩa các card là cùng một problem. D và E tạm đứng riêng vì chưa có card khác đủ gần về pain và quy trình. Nhóm cần xác nhận ranh giới cluster, nhất là việc tìm lại thông tin so với sàng lọc thông tin mới ở A.

**Dữ liệu còn thiếu:** Dương chưa có số đo; Khoa chưa có baseline thực đo và các target còn là giả thuyết. Báo cáo của Lam dùng bối cảnh và số liệu giả định. An tự báo cáo tổng thời gian ở Card #1, còn thời gian phân rã và bối cảnh Card #2–#3 là ước lượng hoặc giả định. Chưa dùng các số này làm baseline chung hay bằng chứng đồng thuận của nhóm.

### 2.3. Opportunity Solution Tree rút gọn

Phạm vi: tìm lại bằng chứng trong paper đã đọc, theo candidate L1 của Lam và [shortlist](shortlist.md).

~~~text
OUTCOME: Giảm thời gian tìm lại bằng chứng từ paper,
         đồng thời giữ đúng ngữ cảnh và truy xuất được nguồn.
├── Opportunity 1: Ghi chú thiếu vị trí cụ thể của bằng chứng
│                 như số trang, hình, bảng hoặc đoạn văn.
├── Opportunity 2: Mất thời gian dò lại PDF để tìm đúng
│                 đoạn, hình hoặc bảng cần dùng.
├── Opportunity 3: Khó xác nhận ngữ cảnh của bằng chứng
│                 để diễn giải nhận định đúng phạm vi.
└── Opportunity 4: Vị trí nguồn được ghi không nhất quán
                  giữa các paper, gây khó khi tìm lại.
~~~

Các opportunity trên lấy từ shortlist và [Card #1 của Lam](../individual/2A202604020_NguyenDucKhuongLam.md); cần được kiểm chứng bằng trường hợp thực tế. Hướng đo là thời gian tìm được bằng chứng, độ đúng của vị trí nguồn và ngữ cảnh. Baseline và target chưa chốt bằng số đo thực tế.

**Các ý là solution, không đặt ở tầng Opportunity:**

- AI chatbot đọc paper.
- RAG-based paper assistant.
- Tự động tóm tắt PDF.
- Ghi chú có cấu trúc, Zotero annotation và liên kết đến trang PDF.

### 2.4. Chấm điểm shortlist (1–5)

Nguồn: [shortlist.md](shortlist.md). Điểm được giữ nguyên từ bảng shortlist.

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| L1 — Tìm lại bằng chứng từ paper | 5 | 5 | 4 | 5 | 5 | 5 | 4 | **33** |
| A1 — So sánh biến thể tín hiệu | 5 | 5 | 4 | 4 | 4 | 5 | 3 | **30** |
| K1 — Tổng hợp thông tin trước Sprint Planning | 5 | 4 | 2 | 3 | 3 | 4 | 4 | **25** |

Mốc 10 phút/lần, trong đó 6 phút dò PDF, là số liệu giả định trong báo cáo của Lam, chưa phải baseline đã đo. Điểm ở cột “Pain có bằng chứng” là đánh giá được ghi trong shortlist, chưa thay thế việc kiểm chứng thực tế.

**Candidate được chọn:** L1 — Tìm lại bằng chứng từ paper.

**Job Story:** Khi cần dùng lại một nhận định từ paper đã đọc, tôi muốn tìm đúng đoạn, hình hoặc bảng chứa bằng chứng, để giải thích có căn cứ mà không phải đọc lại cả bài.

**Vì sao chọn:**

- Phạm vi gọn trong một tác vụ: tìm đúng bằng chứng trong paper đã đọc.
- Có thể đo thời gian tìm và kiểm tra trực tiếp vị trí nguồn, ngữ cảnh trong PDF.
- Có phương án không dùng AI để đối chiếu: ghi số trang/hình/bảng, annotation và liên kết PDF trong Zotero.
- Không cần tích hợp nhiều nguồn dữ liệu dự án. Candidate đạt 33 điểm, cao nhất trong shortlist.

**Vì sao loại các candidate còn lại:**

- **A1 — So sánh biến thể tín hiệu:** domain quant research đặc thù; cần kiểm tra điều kiện thử nghiệm và phân biệt mô tả chênh lệch với kết luận nhân quả.
- **K1 — Tổng hợp thông tin trước Sprint Planning:** phạm vi rộng, liên quan nhiều nguồn và quyền truy cập; chưa có baseline thực nghiệm để xác định bước nghẽn chính.

**Xử lý bất đồng (nếu có):** Chưa có ghi nhận trong tài liệu nguồn.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

Nhóm đã trao đổi trực tiếp với 2 sinh viên cùng lớp, ngoài Nhóm 6, đồng thời tham khảo kinh nghiệm của các thành viên. Phần kiểm chứng hiện gồm lời kể trải nghiệm và research công cụ; chưa có số đo thời gian hoặc kết quả pilot. Tình huống ban đầu lấy từ [Card #1 của Lam](../individual/2A202604020_NguyenDucKhuongLam.md).

### 3.1. Assumption Map

Thang điểm: 1 = thấp, 5 = cao. Điểm dưới đây là đánh giá sơ bộ để ưu tiên kiểm chứng, không phải số đo từ người dùng.

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Sinh viên cần tìm lại bằng chứng khi tổng hợp paper hoặc giải thích nhận định với nhóm/mentor. | Value | 5 | 2 | Có — hỏi về các lần tìm đã xảy ra và tần suất thực tế. |
| 2 | Ghi chú thiếu vị trí nguồn khiến dò đúng đoạn, hình hoặc bảng trong PDF trở thành bước nghẽn. | Value | 5 | 2 | Có — quan sát ghi chú và đo từng bước; phân biệt khó định vị với khó hiểu ngữ cảnh. |
| 3 | Ghi chú có cấu trúc và liên kết Zotero đủ giúp tìm lại bằng chứng, không cần thêm AI. | Usability | 5 | 1 | Có — thử No AI trước, đo cả tốc độ lẫn chất lượng và ngoại lệ. |
| 4 | Zotero hỗ trợ liên kết annotation/ghi chú về trang PDF cần kiểm tra. | Feasibility | 4 | 4 | Tài liệu công cụ mô tả tính năng; cần thử với PDF và ghi chú trong phạm vi pilot. |
| 5 | Thời gian tiết kiệm khi tìm lại lớn hơn công chuẩn bị ghi chú và kiểm chứng. | Viability | 4 | 1 | Có — tính cả chuẩn bị, tìm kiếm và xác minh; mục tiêu giảm ít nhất 30% mới là đề xuất. |

**Ưu tiên kiểm chứng:** #2 và #3. Nếu điểm nghẽn nằm ở hiểu ngữ cảnh thay vì định vị nguồn, chỉ liên kết trang có thể chưa đủ.

### 3.2. Kiểm chứng: interview/survey/evidence

Tổng hợp trao đổi trực tiếp với 2 sinh viên cùng lớp, ngoài Nhóm 6:

| Nội dung | Ghi nhận |
|---|---|
| Người được hỏi | 2 sinh viên cùng lớp, ngoài Nhóm 6. |
| Cách thu thập | Trao đổi trực tiếp về trải nghiệm dùng công cụ khi đọc paper và trích dẫn. |
| Thời điểm | Chưa ghi ngày trao đổi trong bản tổng hợp. |
| Cách làm được kể lại | Các bạn thường dùng NotebookLM. |
| Khó khăn được nêu | Lo công cụ có thể bịa hoặc đưa trích dẫn không đúng khi cố tìm dẫn chứng. |
| Giới hạn ghi nhận | Bản tổng hợp chưa có ví dụ lỗi, ghi nhận từng người hoặc log thao tác; chưa đo thời gian. Hiện ghi nhận mối lo về trích dẫn sai, chưa xác định một lỗi cụ thể. |

| Nguồn | Tín hiệu hiện có | Điều cần làm rõ |
|---|---|---|
| Trao đổi với 2 sinh viên ngoài nhóm | Người được hỏi thường dùng NotebookLM nhưng chưa yên tâm khi lấy trích dẫn. | Xin một lần tìm dẫn chứng gần nhất, yêu cầu đã hỏi, đầu ra và cách người học kiểm nguồn; tìm cả trường hợp công cụ hoặc cách thủ công đã đủ dùng. |
| Kinh nghiệm của thành viên Nhóm 6 | Được dùng để nêu tình huống và đối chiếu cách làm. | Chưa có ghi chép riêng trong báo cáo; không tính thành viên nhóm vào 2 người được phỏng vấn ngoài nhóm. |
| Problem Card #1 | Nêu giả thuyết ghi chú thiếu vị trí nguồn khiến sinh viên phải dò lại PDF. | Chưa xác nhận dò PDF là bước lâu nhất; các mốc thời gian trong card vẫn là giả định. |
| Research Zotero, Elicit và RAG | Có các cách hỗ trợ lưu nguồn, tìm thông tin và gợi ý bằng chứng. | Khả năng công cụ không thay thế phép đo trên tác vụ thực tế; cần thử xem ghi chú có nguồn/Zotero đã đủ chưa. |

**Ảnh hưởng đến bản đề xuất:** ghi nhận phỏng vấn cho thấy cần kiểm độ tin cậy của dẫn chứng, bên cạnh thời gian tìm. Vì vậy, quy trình giữ bước mở PDF gốc và đánh giá riêng vị trí nguồn với ngữ cảnh. Chưa đủ thông tin để kết luận nguyên nhân chính là ghi chú thiếu vị trí hay công cụ gợi ý sai.

**Câu hỏi cho lượt trao đổi tiếp theo:**

1. Lần gần nhất cần tìm lại bằng chứng là khi nào? Có thể mở yêu cầu đã hỏi, ghi chú và PDF để kể lại từng bước không?
2. Đã gặp một trích dẫn sai cụ thể hay đang lo nguy cơ sai? Khi đó đã kiểm và xử lý thế nào?
3. Bước nào tốn công nhất: tìm paper, định vị đoạn/hình/bảng hay đọc lại ngữ cảnh? Có thể quan sát và bấm giờ một lượt không?
4. Có lần nào ghi chú, Zotero hoặc tìm từ khóa đã đủ đáp ứng không? Điều gì khác với lần gặp khó?

### 3.3. Research giải pháp đã có

Nhóm tham khảo các công cụ và pattern dưới đây để xác định phần đã có thể giải quyết bằng công cụ sẵn có. Hiệu quả với tác vụ của nhóm sẽ được đo trong pilot.

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Zotero — annotation, ghi chú và liên kết nguồn | [PDF Reader and Note Editor](https://www.zotero.org/support/pdf_reader), [Notes](https://www.zotero.org/support/notes) | Gắn ghi chú với paper và mở lại trang/annotation khi cần bằng chứng. | Giữ đường dẫn về PDF, không cần AI. | Ghi chú cũ thiếu vị trí phải bổ sung; mở đúng trang chưa bảo đảm hiểu đúng ngữ cảnh. | Thử nhận định + trang/hình/bảng + annotation/liên kết + ngữ cảnh trước khi thêm AI. |
| Elicit — làm việc với paper tải lên | [Which workflow should I use?](https://support.elicit.com/en/articles/14757543-getting-started-with-elicit-which-workflow-should-i-use) | Hỏi về paper tải lên và trích thông tin theo mô tả của công cụ. | Có công cụ sẵn để tham khảo cách hỗ trợ người đọc. | Chưa kiểm hiệu quả với paper của nhóm; người học vẫn phải kiểm nguồn và ngữ cảnh. | Không mặc định công cụ có AI sẽ tốt hơn ghi chú có nguồn/Zotero. |
| RAG — truy xuất kết hợp sinh câu trả lời | [Lewis và cộng sự (2020)](https://arxiv.org/abs/2005.11401) | Gợi ý pattern retrieval trước, sinh/gợi ý nội dung sau nếu cần thử Workflow. | Tách bước tìm ứng viên khỏi bước sinh nội dung. | Bài nghiên cứu không chứng minh độ đúng trích dẫn hay khả năng tìm hình/bảng trong PDF của nhóm. | Chỉ là nhánh tùy chọn; nguồn/vị trí phải lấy từ tài liệu và được người học xác minh. |

**Phương án quay về không dùng AI:** tìm từ/cụm từ trong PDF bằng tính năng sẵn có, theo [Adobe — Searching PDFs](https://helpx.adobe.com/acrobat/using/searching-pdfs.html). Nhận định diễn đạt lại có thể không khớp từ khóa; tìm thấy vẫn phải đọc ngữ cảnh rồi lưu vị trí nguồn.

---

## 4. Quy trình trước/sau (CP5)

Quy trình dưới đây là mô tả ban đầu từ Problem Card. Cần đối chiếu với một lượt tìm dẫn chứng thực tế; báo cáo hiện chưa có số đo từng bước.

### 4.1. Quy trình hiện tại

```text
HIỆN TẠI — GIẢ THUYẾT, 5 bước chính

[1 Ghi chú] → [2 Xác định paper] → [3 Dò PDF] → [4 Đọc ngữ cảnh]
                                      ↑                 ↓
                          BOTTLENECK GIẢ THUYẾT   [5 Lưu vị trí nguồn]

Thời gian từng bước: [CẦN ĐO]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Sinh viên | Nhận định cần kiểm chứng, ghi chú đã có | Ghi chú liên quan được mở | [CẦN ĐO] | Có thể thiếu vị trí nguồn. |
| 2 | Sinh viên | Ghi chú, tên bài hoặc citation | Paper/PDF cần đối chiếu | [CẦN ĐO] | Phạm vi là paper đã đọc. |
| 3 | Sinh viên | Nhận định và PDF | Đoạn, hình hoặc bảng có thể chứa bằng chứng | [CẦN ĐO] | Bottleneck giả thuyết; chưa chứng minh là bước lâu nhất. |
| 4 | Sinh viên | Bằng chứng ứng viên và phần xung quanh | Xác nhận hoặc bác bỏ nhận định theo ngữ cảnh | [CẦN ĐO] | Giữ đúng điều kiện và giới hạn của kết quả. |
| 5 | Sinh viên | Kết quả đã đối chiếu PDF | Bằng chứng và vị trí nguồn được lưu | [CẦN ĐO] | Chưa đủ căn cứ thì ghi chưa xác minh, không dùng làm bằng chứng. |

**Bottleneck chính cần kiểm chứng:** bước 3 — tìm đúng đoạn, hình hoặc bảng khi ghi chú không lưu vị trí nguồn. Khó định vị và khó hiểu ngữ cảnh cần được đo riêng.

### 4.2. Quy trình tương lai

**No AI đề xuất:** ghi chú có cấu trúc và Zotero; người học thao tác và giữ quyền xác nhận bằng chứng. Công tạo ghi chú/liên kết khi đọc cũng phải được đo, dù diễn ra trước lượt tìm lại.

```text
NO AI ĐỀ XUẤT — CHƯA TRIỂN KHAI, 5 bước chính

[1 Nhận định cần kiểm chứng]
               ↓
[2 Structured notes / Zotero]
               ↓
[3 Mở liên kết nguồn] ── thiếu / sai ──> [Tìm thủ công trong PDF]
               │                                    │
               └──────────────────┬─────────────────┘
                                  ↓
                  [4 Sinh viên kiểm tra ngữ cảnh] ← HITL
                                  ↓
                  [5 Lưu bằng chứng đúng vị trí]

Không đủ căn cứ: ghi chưa tìm thấy/chưa xác minh, không chấp nhận nhận định.
Thời gian từng bước và công chuẩn bị: [CẦN ĐO]
```

**Boundary:** người học mở PDF gốc để kiểm nguồn, nội dung và ngữ cảnh trước khi lưu. AI không được tự tạo trích dẫn, bịa nguồn/số trang hoặc tự xác nhận bằng chứng đúng. Liên kết thiếu/sai thì tìm thủ công và vẫn qua bước kiểm tra.

**OPTIONAL — CHƯA TRIỂN KHAI:** chỉ cân nhắc khi No AI và tìm kiếm theo quy tắc chưa đủ.

```text
[Nhận định + paper] → [Retrieval] → [AI gợi ý đoạn và vị trí nguồn]
                                                    ↓
                       [Người học mở PDF gốc để xác minh] → [Lưu kết quả]
```

Vị trí nguồn phải đến từ PDF/metadata truy xuất, không để mô hình tạo số trang. Nếu không tìm đủ căn cứ, báo chưa tìm thấy và quay về kiểm thủ công. Rule (keyword search/BM25) có thể được thử trước Workflow; Agent chưa có cơ sở để chọn.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---|---|---|
| Số bước chính | 5 | 5 | Theo hai pipeline trên slide; nhánh ngoại lệ và công chuẩn bị được ghi riêng. |
| Tổng thời gian | Chưa có baseline thực nghiệm [CẦN ĐO] | Mục tiêu đề xuất giảm ít nhất 30% | Tính cả chuẩn bị, tìm kiếm và kiểm chứng cho cùng bộ tác vụ. |
| Số bước thủ công | 5/5 bước do người học thao tác | 5/5 bước do người học thao tác, có Zotero hỗ trợ | Chưa triển khai script/AI tự động; không suy hiệu quả chỉ từ số bước. |
| Bottleneck | Giả thuyết: dò PDF để tìm đúng bằng chứng | Kỳ vọng giảm dò lại nhờ liên kết nguồn | Chưa biết công kiểm ngữ cảnh và tạo ghi chú có triệt tiêu lợi ích không. |
| Rủi ro mới phát sinh | Ghi chú thiếu vị trí nguồn, phải dò lại | Liên kết sai/hỏng, công chuẩn bị tăng, hiểu sai ngữ cảnh | Luôn kiểm PDF, có fallback thủ công và tính cả ngoại lệ. |
| Chất lượng | [CẦN ĐO] | Không giảm so với baseline | Đánh giá riêng evidence hit rate, citation accuracy và context correctness. |

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên đang đọc và tổng hợp paper nghiên cứu, cần dùng lại nhận định từ paper đã đọc. |
| **Quy trình** | Ghi chú → xác định paper → dò PDF → đọc ngữ cảnh → lưu vị trí nguồn. |
| **Bottleneck** | Giả thuyết: ghi chú thiếu vị trí khiến người học phải dò lại đúng đoạn, hình hoặc bảng; cần quan sát để xác nhận bước nghẽn. |
| **Impact** | Có thể tốn thời gian đọc lại và diễn giải sai điều kiện/giới hạn của kết quả; chưa đo mức độ hay tần suất. |
| **Success Metric** (baseline → target, cách đo) | Baseline: chưa có số đo thực nghiệm. Target đề xuất: giảm ít nhất 30% tổng thời gian, không giảm độ đúng của nguồn và ngữ cảnh. Đo cách tìm hiện tại và No AI trên bộ tác vụ có đối chiếu PDF, tính cả chuẩn bị và xác minh. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | Ưu tiên ghi chú có cấu trúc/Zotero. Người học kiểm PDF trước khi dùng bằng chứng; thiếu/sai liên kết thì tìm thủ công. Nếu thử AI sau này, chỉ gợi ý đoạn và vị trí từ nguồn thật, không tự tạo citation hoặc xác nhận độ đúng. |

**Phản biện AI đã ghi nhận:** đo tốc độ chưa đủ; tìm đúng vị trí nhưng sai ngữ cảnh vẫn không đạt. Cần tính cả công tạo ghi chú, lượt thất bại và quay về thủ công để tránh chuyển công sức sang bước khác.

**Điều chỉnh sau phản biện:** tách thời gian tìm khỏi tổng công chuẩn bị và kiểm chứng; kiểm riêng độ đúng của nguồn và ngữ cảnh. Cách đo được trình bày ở mục 7.

---

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
