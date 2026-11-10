Báo cáo cá nhân — 2A202604000\_DongHuuNguyenKhoa

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Đồng Hữu Nguyên Khoa
- MSSV: 2A202604000
- Email trường (không bắt buộc, repo có thể để public): <26ai.khoadhn@vinuni.edu.vn>
- Tên nhóm: Nhóm 6
- Link repo nhóm: <https://github.com/lit1numyt/K5-L3B-DAY02-Nhom6-DiscoveryProblemFraming.git>

---

## 2. Scan problem (CP1)

Đã scan 10 vấn đề mà Developer và các thành viên kỹ thuật gặp phải trong quá trình chuẩn bị cho sprint, vượt mức tối thiểu 5 vấn đề.

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| #  | Lăng kính                           | Job Story                                                                                                                                                                     | Ai chịu ảnh hưởng?           | Dấu hiệu thực tế cần xác minh                                                                      |
| -- | ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------- | -------------------------------------------------------------------------------------------------- |
| 1  | Thiếu thông tin                     | Khi chuẩn bị cho sprint mới, tôi muốn tìm được toàn bộ tài liệu và thông tin liên quan đến dự án tại một nơi để không phải hỏi nhiều người hoặc tìm kiếm trên nhiều nền tảng. | Developer, PM, Scrum Master  | Thông tin dự án phân tán trên Jira, Slack, Google Drive, Notion và các nền tảng khác.              |
| 2  | Tốn thời gian                       | Khi nhận backlog mới, tôi muốn nhanh chóng hiểu mục tiêu và yêu cầu của từng task để có thể bắt đầu công việc.                                                                | Developer, Tech Lead         | Developer phải đọc nhiều task và tài liệu liên quan trước khi hiểu đầy đủ công việc cần thực hiện. |
| 3  | Công việc lặp lại                   | Khi bắt đầu sprint mới, tôi muốn xem lại kết quả sprint trước và các task chưa hoàn thành mà không phải tự tổng hợp lại toàn bộ tiến độ.                                      | Developer, PM                | Phải kiểm tra lại Jira, sprint report và meeting notes để xác định tiến độ trước đó.               |
| 4  | Thiếu thông tin kỹ thuật            | Khi làm việc với một hệ thống hoặc module đã tồn tại, tôi muốn tìm được tài liệu kỹ thuật, API và kiến trúc liên quan mà không phải phụ thuộc hoàn toàn vào đồng nghiệp.      | Developer, Tech Lead         | Developer thường phải hỏi Tech Lead hoặc người từng phát triển module để hiểu hệ thống.            |
| 5  | Cần đọc và tổng hợp nhiều thông tin | Khi tiếp nhận một task, tôi muốn tổng hợp yêu cầu, acceptance criteria và tài liệu liên quan để hiểu đầy đủ phạm vi công việc.                                                | Developer, BA, PM            | Cần đối chiếu nhiều tài liệu, task và thảo luận trước khi có đủ thông tin để thực hiện.            |
| 6  | Phụ thuộc người khác                | Trước khi bắt đầu sprint, tôi muốn có đầy đủ quyền truy cập repository, database và môi trường development để không bị trì hoãn bởi các vấn đề thiết lập.                     | Developer, DevOps, Tech Lead | Developer phải chờ cấp quyền hoặc nhờ người khác cấu hình môi trường.                              |
| 7  | Thiếu rõ ràng                       | Khi nhận một task chưa có acceptance criteria rõ ràng, tôi muốn xác định chính xác yêu cầu và kết quả mong đợi để tránh hiểu sai khi triển khai.                              | Developer, PO, PM            | Phải trao đổi nhiều lần để xác nhận yêu cầu và phạm vi công việc.                                  |
| 8  | Khó xác định thứ tự ưu tiên         | Khi có nhiều task trong sprint, tôi muốn hiểu mức độ ưu tiên và các dependency giữa chúng để lựa chọn thứ tự thực hiện phù hợp.                                               | Developer, Tech Lead, PM     | Một số task bị blocked do dependency chưa hoàn thành hoặc chưa được xác định rõ.                   |
| 9  | Khó tìm lại thông tin               | Khi cần hiểu lý do của một quyết định kỹ thuật trước đây, tôi muốn tìm lại được bối cảnh và nội dung thảo luận để tránh phải điều tra hoặc tranh luận lại từ đầu.             | Developer, Tech Lead, team   | Phải tìm kiếm trong Slack, meeting notes, GitHub hoặc hỏi người đưa ra quyết định.                 |
| 10 | Thiếu đồng bộ                       | Trước buổi sprint planning, tôi muốn nắm được tình trạng công việc và khả năng tham gia của các thành viên để chuẩn bị kế hoạch phù hợp.                                      | Developer, Scrum Master, PM  | Phải hỏi riêng từng thành viên về tiến độ, workload và khả năng tham gia.                          |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

### Các vấn đề có thể chia thành các nhóm như sau

- **Nhóm A – Tìm kiếm và tổng hợp thông tin:** #1, #4, #5, #9. Các vấn đề liên quan đến việc tìm kiếm, truy xuất và tổng hợp thông tin dự án hoặc kiến thức kỹ thuật từ nhiều nguồn khác nhau.
- **Nhóm B – Hiểu task và làm rõ yêu cầu:** #2, #7. Các vấn đề liên quan đến việc hiểu backlog, xác định phạm vi công việc và làm rõ những yêu cầu còn thiếu hoặc chưa rõ ràng.
- **Nhóm khác:** #3, #6, #8, #10. Các vấn đề liên quan đến theo dõi tiến độ, thiết lập môi trường, quản lý dependency và đồng bộ team.

Hai nhóm A và B có tiềm năng được cải thiện đáng kể thông qua việc tự động hóa tìm kiếm, tổng hợp và phân tích thông tin.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem                                                | Vì sao chọn                                                                                                                     | Điều còn chưa chắc                                                                                              |
| ---- | ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| 1    | Tìm kiếm và tổng hợp thông tin dự án (#1, #5)          | Ảnh hưởng đến nhiều developer; thông tin phân tán trên nhiều nền tảng khiến việc tìm kiếm và tổng hợp tốn thời gian.            | Nguồn thông tin nào gây tốn thời gian nhất? Có thể tích hợp API và truy cập các nguồn dữ liệu này không?        |
| 2    | Truy xuất kiến thức kỹ thuật và quyết định cũ (#4, #9) | Developer thường phụ thuộc vào Tech Lead hoặc senior developer để hiểu hệ thống, kiến trúc và các quyết định kỹ thuật trước đó. | Tài liệu hiện tại có đầy đủ không? Có thể truy xuất chính xác thông tin từ codebase và lịch sử thảo luận không? |
| 3    | Hiểu backlog và làm rõ yêu cầu (#2, #7)                | Task chưa rõ ràng có thể dẫn đến nhiều vòng trao đổi, trì hoãn triển khai và phát sinh rework.                                  | Vấn đề này xảy ra thường xuyên đến mức nào? Nguyên nhân chủ yếu đến từ mô tả task hay quy trình refinement?     |

### 3.2. Problem Card #1 – Tìm kiếm và tổng hợp thông tin dự án

| Thành phần                  | Nội dung                                                                                                                                                                                                                                              |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Job Story**               | Khi chuẩn bị cho một sprint mới, tôi muốn tìm kiếm và tổng hợp toàn bộ thông tin liên quan đến dự án tại một nơi để hiểu được bối cảnh công việc mà không phải liên tục chuyển đổi giữa các nền tảng hoặc hỏi nhiều người.                            |
| **Actor**                   | Software Developer, đặc biệt là thành viên mới hoặc developer tham gia vào một dự án đã tồn tại.                                                                                                                                                      |
| **Thời điểm / bối cảnh**    | Trước Sprint Planning, khi developer cần thu thập tài liệu dự án, meeting notes, sprint reports, backlog và thông tin liên quan đến các task.                                                                                                         |
| **Quy trình hiện tại**      | 1. Xác định thông tin cần tìm. 2. Tìm tài liệu trên Drive / Notion. 3. Đọc meeting notes. 4. Kiểm tra Jira và sprint history. 5. Tìm kiếm các thảo luận trên Slack. 6. Hỏi đồng nghiệp nếu vẫn thiếu thông tin. 7. Tự tổng hợp thành ghi chú cá nhân. |
| **Bottleneck**              | Các bước 2–6. Thông tin phân tán trên nhiều nền tảng, yêu cầu developer phải tìm kiếm, đọc, đối chiếu và kết nối thủ công. Việc chuyển đổi liên tục giữa các nền tảng cũng làm gián đoạn luồng công việc.                                             |
| **Impact**                  | Tốn thời gian tìm kiếm thông tin, phải thực hiện lại các thao tác thu thập dữ liệu, tăng số lần gián đoạn để hỏi đồng nghiệp và làm chậm quá trình chuẩn bị sprint. Cần phỏng vấn để xác định mức độ ảnh hưởng thực tế.                               |
| **Success Metric**          | Mục tiêu giả thuyết: giảm ít nhất 50% thời gian thu thập thông tin dự án, đồng thời đảm bảo tính chính xác và khả năng truy xuất nguồn của thông tin.                                                                                                 |
| **Phương án không dùng AI** | Chuẩn hóa cấu trúc tài liệu, sử dụng shared folders, xây dựng project templates và dashboard tập trung. Các giải pháp này giúp cải thiện khả năng truy cập nhưng developer vẫn phải tự đọc và tổng hợp thông tin.                                     |
| **Giả thuyết về AI**        | Xây dựng một AI assistant có khả năng truy xuất thông tin từ các nguồn dữ liệu dự án được cấp quyền, tự động tổng hợp và phân loại thông tin thành báo cáo có cấu trúc, kèm theo nguồn tham chiếu để developer kiểm tra.                              |
| **Cảm nhận nhanh**          | Workflow / Knowledge Assistant.                                                                                                                                                                                                                       |

#### Workflow hiện tại

```text
HIỆN TẠI — Thông tin phân tán trên nhiều nền tảng

[1. Xác định thông tin cần tìm]
                |
                v
[2. Tìm tài liệu trên Drive / Notion]
                |
                v
[3. Đọc meeting notes]
                |
                v
[4. Kiểm tra Jira và sprint history]
                |
                v
[5. Tìm kiếm thảo luận trong Slack]
                |
                v
[6. Hỏi đồng nghiệp nếu thiếu thông tin]
                |
                v
[7. Tự tổng hợp thành ghi chú cá nhân]

BOTTLENECK:
Tìm kiếm lặp lại, chuyển đổi ngữ cảnh và
tổng hợp thông tin thủ công.
```

#### Workflow giả thuyết với AI

```text
ĐỀ XUẤT — AI hỗ trợ tìm kiếm và tổng hợp thông tin

[Developer cung cấp yêu cầu / bối cảnh]
                |
                v
[AI truy xuất dữ liệu từ các nguồn được cấp quyền]
                |
                v
[AI phân loại và tổng hợp thông tin]
                |
                v
[Tạo báo cáo có cấu trúc kèm nguồn tham chiếu]
                |
                v
[Developer kiểm tra và xác nhận]
                |
                v
[Sẵn sàng cho Sprint Planning]
```

---

### 3.3. Problem Card #2 – Truy xuất kiến thức kỹ thuật và quyết định cũ

| Thành phần                  | Nội dung                                                                                                                                                                                                                                                                                                                          |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Job Story**               | Khi chuẩn bị thực hiện một task trên hệ thống đã tồn tại, tôi muốn nhanh chóng hiểu kiến trúc, tài liệu kỹ thuật và các quyết định kỹ thuật trước đây để không phải điều tra lại từ đầu hoặc phụ thuộc quá nhiều vào senior developer.                                                                                            |
| **Actor**                   | Software Developer, đặc biệt là thành viên mới hoặc developer phải làm việc với module chưa quen thuộc.                                                                                                                                                                                                                           |
| **Thời điểm / bối cảnh**    | Trước khi thực hiện một task kỹ thuật, chỉnh sửa module hiện có hoặc tích hợp với một API / component chưa quen thuộc.                                                                                                                                                                                                            |
| **Quy trình hiện tại**      | 1. Xác định module hoặc vấn đề cần tìm hiểu. 2. Tìm kiếm tài liệu kiến trúc. 3. Đọc README và kiểm tra source code. 4. Tìm kiếm lịch sử thảo luận trên Slack / meeting notes. 5. Xác định người từng phát triển module. 6. Hỏi Tech Lead hoặc senior developer. 7. Tự tổng hợp lại bối cảnh và lý do của các quyết định kỹ thuật. |
| **Bottleneck**              | Các bước 3–6. Kiến thức kỹ thuật bị phân tán giữa source code, tài liệu, lịch sử thảo luận và kinh nghiệm cá nhân. Đặc biệt, lý do đằng sau các quyết định kỹ thuật thường khó tìm lại.                                                                                                                                           |
| **Impact**                  | Developer phải điều tra lại những vấn đề đã được giải quyết trước đó, làm gián đoạn công việc của senior developer, kéo dài thời gian onboarding và có nguy cơ đưa ra quyết định kỹ thuật không phù hợp với kiến trúc hiện tại.                                                                                                   |
| **Success Metric**          | Mục tiêu giả thuyết: giảm thời gian tìm câu trả lời cho các câu hỏi kỹ thuật liên quan đến dự án xuống dưới 2 phút trung bình mỗi câu hỏi, đồng thời cung cấp nguồn tham chiếu có thể kiểm chứng.                                                                                                                                 |
| **Phương án không dùng AI** | Xây dựng architecture diagrams, ADRs (Architecture Decision Records), README, API documentation và chuẩn hóa meeting notes kỹ thuật.                                                                                                                                                                                              |
| **Giả thuyết về AI**        | Xây dựng RAG-based Technical Knowledge Assistant có khả năng truy xuất tài liệu kỹ thuật, code references và lịch sử thảo luận được cấp quyền, sau đó cung cấp giải thích theo ngữ cảnh kèm đường dẫn đến nguồn thông tin.                                                                                                        |
| **Cảm nhận nhanh**          | RAG / Technical Knowledge Assistant.                                                                                                                                                                                                                                                                                              |

#### Workflow hiện tại

```text
HIỆN TẠI — Developer phải tự tìm hiểu kiến thức kỹ thuật

[Không quen thuộc với module / component]
                |
                v
[Tìm kiếm tài liệu kiến trúc]
                |
                v
[Đọc README và kiểm tra source code]
                |
                v
[Tìm lịch sử thảo luận / quyết định]
                |
                v
[Xác định developer từng phụ trách]
                |
                v
[Hỏi Tech Lead / senior developer]
                |
                v
[Tự tổng hợp lại kiến thức và bối cảnh]

BOTTLENECK:
Kiến thức phân tán, khó truy xuất và phụ thuộc
vào kinh nghiệm của một số thành viên.
```

#### Workflow giả thuyết với AI

```text
ĐỀ XUẤT — AI hỗ trợ truy xuất kiến thức kỹ thuật

[Developer đặt câu hỏi về module / component]
                |
                v
[AI truy xuất tài liệu kỹ thuật]
                |
                v
[AI truy xuất code references và quyết định cũ]
                |
                v
[AI tổng hợp giải thích theo ngữ cảnh]
                |
                v
[Cung cấp nguồn tham chiếu]
                |
                v
[Developer kiểm tra và xác nhận]
```

---

### 3.4. Problem Card #3 – Hiểu backlog và làm rõ yêu cầu

| Thành phần                  | Nội dung                                                                                                                                                                                                                                                                                 |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Job Story**               | Khi nhận một task mới trong Product Backlog, tôi muốn hiểu rõ yêu cầu, kết quả mong đợi, phạm vi kỹ thuật và acceptance criteria để có thể bắt đầu triển khai mà không phải trao đổi nhiều lần hoặc hiểu sai yêu cầu.                                                                    |
| **Actor**                   | Software Developer / Junior Developer nhận task từ PO, PM hoặc Tech Lead.                                                                                                                                                                                                                |
| **Thời điểm / bối cảnh**    | Trước Sprint Planning và trong giai đoạn đầu của sprint, khi developer đọc và đánh giá các user stories hoặc technical tasks mới.                                                                                                                                                        |
| **Quy trình hiện tại**      | 1. Mở task trên Jira. 2. Đọc mô tả và tài liệu đính kèm. 3. Xác định các yêu cầu còn thiếu hoặc chưa rõ. 4. Tìm kiếm các task và thảo luận liên quan. 5. Liên hệ PM / PO / Tech Lead để hỏi thêm. 6. Trao đổi và xác nhận kỳ vọng. 7. Cập nhật ghi chú hoặc giả định triển khai cá nhân. |
| **Bottleneck**              | Các bước 3–6. Mô tả task thiếu bối cảnh, acceptance criteria hoặc constraints khiến developer phải thực hiện nhiều vòng trao đổi để hiểu đúng yêu cầu.                                                                                                                                   |
| **Impact**                  | Trì hoãn thời điểm bắt đầu triển khai, làm gián đoạn công việc của PM / PO / Tech Lead, tạo ra cách hiểu không đồng nhất giữa các thành viên và tăng nguy cơ phải thực hiện lại công việc.                                                                                               |
| **Success Metric**          | Mục tiêu giả thuyết: giảm ít nhất 50% thời gian làm rõ yêu cầu và số lần trao đổi bổ sung, đồng thời duy trì hoặc cải thiện mức độ đầy đủ của acceptance criteria.                                                                                                                       |
| **Phương án không dùng AI** | Chuẩn hóa user story templates, yêu cầu acceptance criteria rõ ràng, áp dụng Definition of Ready và tổ chức backlog refinement thường xuyên.                                                                                                                                             |
| **Giả thuyết về AI**        | Xây dựng AI Requirements Assistant có khả năng phân tích backlog và tài liệu dự án, phát hiện các yêu cầu mơ hồ hoặc còn thiếu, đề xuất câu hỏi cần làm rõ và gợi ý acceptance criteria để PM / PO xem xét và xác nhận.                                                                  |
| **Cảm nhận nhanh**          | Workflow / AI Requirements Assistant.                                                                                                                                                                                                                                                    |

#### Workflow hiện tại

```text
HIỆN TẠI — Task chưa rõ ràng, cần nhiều vòng trao đổi

[Nhận task trên Jira]
                |
                v
[Đọc mô tả và tài liệu đính kèm]
                |
                v
[Xác định yêu cầu còn thiếu / chưa rõ]
                |
                v
[Tìm kiếm task và thảo luận liên quan]
                |
                v
[Liên hệ PM / PO / Tech Lead]
                |
                v
[Trao đổi và chờ xác nhận]
                |
                v
[Cập nhật ghi chú / giả định triển khai]
                |
                v
[Bắt đầu thực hiện task]

BOTTLENECK:
Yêu cầu chưa rõ ràng dẫn đến nhiều vòng
trao đổi và nguy cơ hiểu sai task.
```

#### Workflow giả thuyết với AI

```text
ĐỀ XUẤT — AI hỗ trợ phân tích và làm rõ yêu cầu

[Developer nhận task trên Jira]
                |
                v
[AI phân tích task và tài liệu liên quan]
                |
                v
[Phát hiện yêu cầu mơ hồ / còn thiếu]
                |
                v
[AI đề xuất câu hỏi và acceptance criteria]
                |
                v
[PM / PO xem xét và xác nhận]
                |
                v
[Developer nhận task đã được làm rõ]
                |
                v
[Bắt đầu triển khai]
```

---

### Card muốn pitch nhất

### Card muốn pitch nhất

- **Card số:** #1 – Tìm kiếm và tổng hợp thông tin dự án.
- **Vì sao:** Đây là vấn đề có thể ảnh hưởng đến nhiều developer, đặc biệt là thành viên mới hoặc những người tham gia vào dự án đã tồn tại. Thông tin thường nằm rải rác trên nhiều nền tảng như Jira, Slack, Google Drive và Notion, khiến developer phải liên tục tìm kiếm, đọc, đối chiếu và tự tổng hợp trước khi có thể hiểu đầy đủ bối cảnh công việc. Tôi cho rằng đây là cơ hội để cải thiện quy trình chuẩn bị sprint, giảm thời gian tìm kiếm thông tin và hạn chế sự phụ thuộc vào đồng nghiệp. Tuy nhiên, cần xác minh mức độ ảnh hưởng thực tế trước khi quyết định có nên ứng dụng AI hay không.
- **Câu hỏi muốn nhóm phản biện:**
  1. Vấn đề thông tin phân tán có thực sự gây ảnh hưởng đáng kể đến developer hay chỉ là bất tiện nhỏ trong quy trình làm việc?
  2. Có nên gộp việc tìm kiếm thông tin dự án và truy xuất kiến thức kỹ thuật vào cùng một Problem Card, hay đây là hai nhu cầu khác nhau?
  3. Liệu chuẩn hóa documentation và xây dựng dashboard tập trung đã đủ giải quyết vấn đề, hay AI thực sự mang lại giá trị bổ sung?
  4. Phạm vi MVP nên giới hạn ở những nguồn dữ liệu nào để vừa khả thi về mặt kỹ thuật vừa tạo ra giá trị thực tế?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra                                                                         | Đồng ý?                                                                                                   | Đã sửa gì                                                                                                                           |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| Problem Card có phạm vi quá rộng, bao gồm nhiều nguồn dữ liệu và loại thông tin khác nhau. | Đồng ý. Phạm vi ban đầu có thể khiến việc triển khai và kiểm chứng trở nên phức tạp.                      | Định hướng giới hạn MVP ở Jira, meeting notes và tài liệu dự án; chỉ mở rộng sang các nguồn khác khi xác định được nhu cầu thực tế. |
| Chưa xác định được nguồn thông tin nào khiến developer tốn nhiều thời gian nhất.           | Đồng ý. Hiện chưa có dữ liệu phỏng vấn hoặc quan sát để xác định bottleneck chính.                        | Bổ sung việc phỏng vấn và quan sát developer để xác định nguồn thông tin thường được tìm kiếm, tần suất sử dụng và thời gian xử lý. |
| Giả định rằng có thể tích hợp tất cả nguồn dữ liệu vào một hệ thống AI.                    | Đồng ý. Khả năng tích hợp còn phụ thuộc vào API, quyền truy cập, định dạng dữ liệu và chính sách bảo mật. | Chưa mặc định tích hợp toàn bộ nền tảng; cần đánh giá khả năng truy cập và tích hợp từng nguồn trước khi xác định MVP.              |
| Success Metric giảm 50% thời gian chưa có baseline thực tế.                                | Đồng ý. Đây mới là mục tiêu giả thuyết, chưa phải kết quả đo lường.                                       | Giữ mức 50% như mục tiêu ban đầu và bổ sung bước đo thời gian thu thập thông tin theo quy trình hiện tại để làm baseline.           |
| Có thể giải quyết vấn đề bằng cách chuẩn hóa tài liệu mà không cần AI.                     | Đồng ý. Đây là phương án thay thế cần được đánh giá.                                                      | Bổ sung chuẩn hóa documentation, shared folders và dashboard tập trung làm phương án không sử dụng AI để so sánh hiệu quả.          |
| AI có thể tổng hợp sai hoặc bỏ sót thông tin quan trọng.                                   | Đồng ý. Điều này có thể khiến developer sử dụng thông tin không chính xác.                                | Yêu cầu AI cung cấp nguồn tham chiếu cho các thông tin được tổng hợp và để developer kiểm tra, xác nhận trước khi sử dụng.          |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động                  | Tôi đã làm gì?                                                                                                                                                                                                                        | Kết quả / ảnh hưởng tới bài nhóm                                                                                                                                                                                  |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Pitch Problem Card         | Mình đã trình bày Problem Card #1 của mình, giải thích vấn đề và hướng giải quyết dự kiến.                                                                                                                                            | Nhóm đã debate các Problem Card và cuối cùng quyết định chọn Problem Card của bạn Lam.                                                                                                                            |
| Phản biện bài của bạn khác | Mình đã đặt câu hỏi về solution của các bạn. Cụ thể, với solution của bạn An, mình cho rằng vấn đề có thể được giải quyết bằng deterministic algorithm hoặc scripting thay vì chấp nhận tính không xác định và sai số của mô hình ML. | Giúp nhóm nhận diện nguy cơ solution-first, tránh đưa AI vào một quy trình khi phương pháp đơn giản hơn có thể giải quyết được vấn đề.                                                                            |
| Nhận phản biện             | Mình nhận được phản biện rằng AI hỗ trợ digest paper với khối lượng lớn có nguy cơ hallucination, đặc biệt là trích dẫn giả hoặc thông tin không đúng ngữ cảnh.                                                                       | Làm rõ hướng tiếp cận: công cụ nên đóng vai trò semantic search/retrieval engine thay vì tự viết lại nội dung paper. Cần sử dụng chunking, truy xuất nguồn và kiểm tra ngữ cảnh để hạn chế kết quả ngoài phạm vi. |
| Gom cluster / cây OST      | Trình bày Problem Card của mình để các thành viên hiểu vấn đề, từ đó có thêm cơ sở so sánh và gom các problem có liên quan.                                                                                                           | Đóng góp thêm góc nhìn khi nhóm phân loại và đánh giá các problem trước khi chọn candidate.                                                                                                                       |
| Chọn candidate problem     | Vote cho Problem Card của bạn Lam sau khi nghe pitch và thảo luận các phương án.                                                                                                                                                      | Nhóm thống nhất chọn bài của bạn Lam làm problem chính.                                                                                                                                                           |
| Kiểm chứng / research      | Đọc blog post của researchers/RA và báo cáo, tài liệu của những tool có solution gần với bài toán. So sánh hướng tiếp cận có AI và không sử dụng AI.                                                                                  | Nhận thấy các phương pháp No-AI có những công cụ cụ thể và dễ kiểm soát hơn. Đây là cơ sở để ưu tiên thử structured notes/Zotero trước khi cân nhắc AI.                                                           |
| Quy trình nhóm             | Phụ trách xây dựng quy trình Before/After ở CP5, phân rã quy trình thành 5 bước, xác định actor, input, output và bottleneck giả thuyết.                                                                                              | Nhóm có mô hình quy trình cụ thể để thảo luận. Đồng thời xác định cần đo thời gian từng bước và tính cả công chuẩn bị, tìm kiếm, xác minh thay vì chỉ đo tốc độ retrieval.                                        |
| Problem Statement          | Tham gia xây dựng và phản biện Problem Statement v0, làm rõ actor, workflow, bottleneck, impact, success metric và boundary.                                                                                                          | Problem Statement được cụ thể hóa hơn: phân biệt thời gian tìm kiếm với tổng thời gian, đánh giá cả citation accuracy và context correctness, không chỉ tốc độ.                                                   |
| Mức can thiệp AI           | Đề xuất và ủng hộ hướng No-AI-first. Nếu No AI chưa đủ mới cân nhắc Rule, sau đó mới đến Workflow; chưa có cơ sở để sử dụng Agent.                                                                                                    | Giữ phạm vi giải pháp đơn giản, dễ kiểm chứng và có quyền xác nhận cuối cùng thuộc về người học.                                                                                                                  |
| Quyết định                 | Ủng hộ quyết định Not Yet đối với việc triển khai AI vì chưa có baseline và bằng chứng cho thấy các phương pháp đơn giản hơn không đáp ứng được nhu cầu.                                                                              | Ưu tiên quan sát, đo baseline và thử nghiệm No AI trước. Chưa đưa ra kết luận triển khai AI khi chưa có dữ liệu thực nghiệm.                                                                                      |

---

## 5. Dùng AI

| Checkpoint                     | Tôi dùng AI để làm gì?                                                                                          | AI hữu ích ở đâu?                                                                                              | AI sai hoặc hời hợt ở đâu?                                                                                                        | Tôi sửa gì bằng nhận định của mình?                                                                                                        |
| ------------------------------ | --------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| CP1 Scan                       | Hỗ trợ tổng hợp thông tin ban đầu, phân tích các vấn đề và tìm những hướng có thể phát triển thành problem.     | Giúp mở rộng góc nhìn và hệ thống hóa các quan sát ban đầu.                                                    | AI bị phình scope rất nhanh, bị ưu tiên AI solution hoặc recommend code/app solution cho những vấn đề không được đề cập.          | Ưu tiên những vấn đề có tình huống cụ thể và có thể quan sát, kiểm chứng thay vì chọn chỉ vì nghe có vẻ phù hợp với AI.                    |
| CP2 Problem Card               | Hỗ trợ diễn đạt và cấu trúc hóa Problem Card, xác định actor, pain point và solution dự kiến.                   | Giúp trình bày vấn đề rõ ràng và có cấu trúc hơn.                                                              | Dễ chuyển từ pain point sang solution quá sớm, mặc định rằng vấn đề cần được giải quyết bằng AI.                                  | Tách biệt problem và solution, xem xét liệu scripting, deterministic algorithm hoặc thay đổi thói quen có thể giải quyết vấn đề hay không. |
| CP4 Research                   | Hỗ trợ digest và tổng hợp tài liệu, tìm hiểu các hướng tiếp cận và công cụ có solution tương tự.                | Tiết kiệm thời gian đọc sơ bộ và giúp xác định những hướng research cần tìm hiểu sâu hơn.                      | Có nguy cơ hallucination, trích dẫn không tồn tại hoặc diễn giải kết quả ngoài ngữ cảnh của paper.                                | Đối chiếu với blog post, báo cáo và nguồn gốc; không coi nội dung AI tổng hợp là bằng chứng nếu chưa kiểm tra tài liệu gốc.                |
| CP5 Quy trình                  | Hỗ trợ phân tích workflow Before/After, phản biện bottleneck, đề xuất metric và rà soát các bước còn thiếu.     | Giúp nhận ra việc chỉ đo retrieval time là chưa đủ; cần tính cả công chuẩn bị, xác minh và fallback thủ công.  | Có xu hướng tập trung vào việc tối ưu bước tìm kiếm mà chưa đánh giá liệu tổng công việc thực tế có giảm hay không.               | Xây dựng lại quy trình 5 bước, ghi nhận thời gian từng bước là \[CẦN ĐO], và bổ sung tổng thời gian cùng chất lượng bằng chứng.            |
| CP5–6 Problem Statement        | Dùng AI để phản biện Problem Statement, kiểm tra tính đầy đủ của metric, boundary và cách đánh giá.             | Giúp phát hiện những thiếu sót như chưa phân biệt evidence hit rate, citation accuracy và context correctness. | Một số đề xuất có thể giả định AI mang lại lợi ích mà chưa có baseline hoặc kết quả thử nghiệm chứng minh.                        | Giữ các con số 30% là target đề xuất, không phải kết quả; bổ sung pilot 10 yêu cầu từ 3 paper và tính cả công chuẩn bị.                    |
| CP6 Mức can thiệp / quyết định | Dùng AI để so sánh các mức No AI, Rule, Workflow và Agent, đồng thời phản biện rủi ro khi đưa AI vào quy trình. | Giúp hệ thống hóa điều kiện cần thiết để nâng cấp mức can thiệp và các rủi ro tương ứng.                       | Không thể tự quyết định AI có thực sự cần thiết khi chưa có dữ liệu thực nghiệm về pain point và hiệu quả của phương án đơn giản. | Chọn No AI First và Not Yet. Chỉ cân nhắc Workflow nếu No AI/Rule chưa đủ và thử nghiệm chứng minh được lợi ích mà không giảm chất lượng.  |

---

## 6. Reflection (CP7)

### 6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?

Mình nhận thấy có rất nhiều research gap và optimization gap trong workflow của những người xung quanh. Trước đây, khi nghĩ đến việc cải thiện một quy trình, mình thường có xu hướng nghĩ đến việc ứng dụng một công nghệ hoặc xây dựng một công cụ mới. Tuy nhiên, qua các problem được trình bày, mình nhận ra có nhiều vấn đề có thể được cải thiện chỉ bằng cách thay đổi habit, tổ chức lại thông tin hoặc sử dụng tốt hơn những công cụ hiện có.

Một workflow có thể đang tốn nhiều thời gian không nhất thiết vì thiếu AI, mà có thể do thông tin bị phân tán, thao tác lặp lại hoặc cách tổ chức công việc chưa hợp lý. Mình cũng học được rằng một vấn đề nhìn có vẻ nhỏ đối với người ngoài nhưng lại có thể ảnh hưởng đáng kể đến người trực tiếp thực hiện công việc đó.

Điều mình rút ra là cần hiểu rõ pain point và bối cảnh của actor trước khi nghĩ đến solution. Không phải problem nào cũng cần được giải quyết bằng một sản phẩm công nghệ mới.

### 6.2. Nhóm có lúc nào bị "solution-first" không? Lúc đó nhóm nhận ra và xử lý thế nào?

Có. Mình nhận thấy điều này khá rõ khi nhóm thảo luận solution của bạn An. Hướng giải quyết ban đầu có xu hướng ứng dụng AI vào workflow, trong khi một số thao tác thực tế có thể được xử lý bằng scripting hoặc deterministic algorithm.

Mình đã đặt câu hỏi liệu có thực sự cần sử dụng ML cho bài toán đó hay không, đặc biệt khi kết quả của một thuật toán xác định có thể dễ kiểm soát và dự đoán hơn. Nhóm đã phản biện lại solution và nhận ra rằng việc đưa AI vào không mặc nhiên tạo ra giá trị nếu một phương pháp đơn giản hơn đã giải quyết được vấn đề.

Qua tình huống này, mình thấy việc phân biệt problem với solution rất quan trọng. Nếu bắt đầu bằng việc tìm cách ứng dụng AI, nhóm có thể vô tình cố gắng tìm một problem phù hợp với công nghệ thay vì tìm giải pháp phù hợp nhất cho người dùng.

### 6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.

Có. Một ví dụ cụ thể là khi nhóm xây dựng quy trình và Problem Statement cho bài toán tìm lại dẫn chứng trong paper.

Ban đầu, mình tập trung khá nhiều vào việc tìm đúng đoạn thông tin trong PDF và giảm thời gian tìm kiếm. Tuy nhiên, sau khi nhận phản biện, mình nhận ra rằng tìm được một đoạn có từ khóa liên quan chưa đồng nghĩa với việc tìm được bằng chứng thực sự hỗ trợ nhận định. Một kết quả có thể đúng vị trí nhưng vẫn sai ngữ cảnh, bỏ qua điều kiện áp dụng hoặc diễn giải vượt quá kết luận của paper.

Vì vậy, mình đồng ý với việc mở rộng tiêu chí đánh giá. Thay vì chỉ đo retrieval time, nhóm bổ sung evidence hit rate, citation accuracy và context correctness. Đồng thời, tổng thời gian phải bao gồm cả công chuẩn bị ghi chú và xác minh PDF. Điều này khiến mình thay đổi cách nhìn về success metric: tối ưu tốc độ không có ý nghĩa nếu chất lượng bằng chứng bị giảm.

### 6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?

Có. Điều khiến mình bất ngờ là kết quả trao đổi cho thấy một số researcher tương đối chấp nhận việc mất thời gian tìm lại dẫn chứng. Họ cho rằng quá trình tự tìm kiếm và đọc lại nguồn, dù tốn thời gian, vẫn có thể giúp họ ghi nhớ và hiểu rõ hơn nội dung cũng như giới hạn của dẫn chứng.

Điều này khiến mình nhận ra rằng không phải mọi thao tác tốn thời gian đều là một pain point cần loại bỏ. Đôi khi, chính quá trình thực hiện thủ công lại đóng góp vào chất lượng học tập và nghiên cứu của người dùng.

Mình cũng nhận thấy rằng nếu chỉ nhìn vào thời gian hoàn thành tác vụ, nhóm có thể đưa ra một solution tối ưu sai mục tiêu. Việc tự động hóa tìm kiếm có thể giảm thời gian thao tác nhưng cũng có nguy cơ khiến người dùng ít đọc lại ngữ cảnh hơn.

Do đó, mình cho rằng cần phân biệt giữa thao tác lặp lại không tạo thêm giá trị và những thao tác thực sự giúp người học hiểu sâu hơn. Một solution tốt không nhất thiết phải loại bỏ toàn bộ thời gian làm việc thủ công.

### 6.5. Điều khó nhất khi viết Problem Statement là gì?

Theo mình, khó nhất là xác định chính xác bottleneck và xây dựng success metric đủ phản ánh giá trị thực tế của solution.

Ban đầu, việc mô tả workflow khá dễ vì có thể chia thành các bước như ghi chú, xác định paper, dò PDF, đọc ngữ cảnh và lưu vị trí nguồn. Tuy nhiên, để kết luận bước nào thực sự là bottleneck thì cần quan sát và đo lường chứ không thể chỉ dựa vào cảm nhận.

Ngoài ra, mình thấy việc xây dựng metric cũng khó hơn dự kiến. Nếu chỉ đo thời gian tìm kiếm, nhóm có thể bỏ qua công chuẩn bị ghi chú, thời gian xác minh và những trường hợp phải quay lại tìm thủ công. Tương tự, tìm được đúng trang nhưng hiểu sai ngữ cảnh vẫn không thể xem là thành công.

Vì vậy, nhóm phải tách các tiêu chí về tốc độ và chất lượng, đồng thời xác định rõ boundary: người học luôn phải kiểm tra PDF gốc trước khi chấp nhận bằng chứng. Mình học được rằng Problem Statement tốt không chỉ mô tả một vấn đề nghe có vẻ hợp lý, mà còn phải có cách kiểm chứng và điều kiện đánh giá cụ thể.

### 6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?

Nếu làm lại, mình sẽ dành nhiều thời gian hơn cho việc thu thập bằng chứng từ workflow thực tế ngay từ đầu, thay vì nhanh chóng chuyển sang thảo luận giải pháp. Cụ thể, mình muốn quan sát một researcher thực hiện một tác vụ tìm dẫn chứng từ đầu đến cuối, ghi lại thời gian từng bước và những lần phải tìm lại thông tin.

Mình cũng sẽ phản biện mạnh hơn về tính đại diện của dữ liệu. Việc trao đổi với hai sinh viên có thể cung cấp những góc nhìn ban đầu, nhưng chưa đủ để kết luận rằng vấn đề phổ biến hoặc đủ nghiêm trọng để cần xây dựng một giải pháp mới.

Một điểm nữa mình muốn làm tốt hơn là đặt câu hỏi về chi phí chuyển đổi workflow. Ví dụ, structured notes và Zotero có thể giúp tìm lại nguồn nhanh hơn, nhưng việc tạo và duy trì các ghi chú có cấu trúc cũng tiêu tốn thời gian. Nếu không tính phần công này, nhóm có thể đánh giá quá cao hiệu quả của phương án mới.

Cuối cùng, mình sẽ yêu cầu nhóm xác định rõ điều kiện dừng trước khi thảo luận nâng cấp lên AI. Nếu No AI hoặc Rule đã đáp ứng được nhu cầu thì không có lý do thực tế để tiếp tục tăng độ phức tạp của solution.

### 6.7. Hiểu bài

Bài toán của nhóm là hỗ trợ sinh viên tìm lại bằng chứng từ những paper nghiên cứu đã đọc khi cần kiểm chứng một nhận định. Quy trình hiện tại gồm ghi chú, xác định paper, dò PDF, đọc ngữ cảnh và lưu lại vị trí nguồn. Bottleneck giả thuyết là việc tìm đúng đoạn, hình hoặc bảng khi ghi chú không lưu vị trí nguồn, nhưng nhóm vẫn cần đo baseline để xác nhận. Metric không chỉ gồm retrieval time mà còn có evidence hit rate, citation accuracy, context correctness và tổng thời gian bao gồm cả công chuẩn bị. Boundary là người học phải mở PDF gốc để kiểm tra nguồn, bằng chứng và ngữ cảnh, không chấp nhận nhận định khi chưa đủ căn cứ. Nhóm chọn No AI First với structured notes và Zotero, sau đó mới cân nhắc Rule hoặc Workflow nếu phương án đơn giản chưa đủ. AI chưa được triển khai vì nhóm chưa có baseline và bằng chứng chứng minh nó tạo ra giá trị tốt hơn các phương án hiện tại. Vì vậy, quyết định hiện tại là Not Yet, tiếp tục kiểm chứng và thử nghiệm trước khi xem xét triển khai AI.

---

## 7. Tài liệu tham khảo
