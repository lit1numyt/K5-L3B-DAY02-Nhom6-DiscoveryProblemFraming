# CP4 — Kiểm chứng và research giải pháp đã có

Phụ trách: Nguyễn Hữu An.

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
