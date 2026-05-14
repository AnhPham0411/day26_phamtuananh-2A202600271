---
artifact: 03-takenotes — Quan sát cá nhân sau phần chia sẻ nhóm khác
bai-tap: 3 — Quan sát + rút ra bài học (cá nhân)
phase: Sau phần shareout của các nhóm
time: 15 phút (xem deck slide 4 để biết khung giờ chính xác)
input: Phần thuyết trình của ít nhất 2 nhóm khác trên lớp
nop-cuoi: Có — file cuối Lab 3 (cá nhân)
---

# 03 — Take notes: quan sát + bài học cá nhân

Đây là phần cá nhân. Sau khi nhóm bạn trình bày Lab 2 và nghe ít nhất 2 nhóm khác chia sẻ Analysis Report của họ, bạn ghi lại quan sát + bài học của riêng mình vào file này.

Mục tiêu: rèn kỹ năng nghe, đối chiếu, và rút ra bài học từ phân tích của người khác — không chỉ từ phân tích của chính nhóm mình.

Quy tắc khi viết:

- Trích dẫn cụ thể tên sản phẩm + nhóm đã quan sát (không nói chung chung).
- Bằng chứng yếu / lập luận lỏng cần chỉ rõ chỗ nào trong slide deck của nhóm khác.
- Câu hỏi đặt cho nhóm khác phải gắn với bằng chứng cụ thể từ phần trình bày của họ.

---

## Thông tin

- **Mã học viên**: 2A202600271
- **Họ tên**: Phạm Tuấn Anh
- **Ngày**: 2026-05-14
- **Nhóm Lab 2 của tôi**: NotebookLM vs Elicit trong ngành Nghiên cứu học thuật (Research)

---

## Phần 1 — Nhóm đã quan sát (≥ 2 nhóm khác)

| # | Tên nhóm / mã 2 học viên | Ngành | 2 sản phẩm họ test |
|---|---|---|---|
| 1 | Quách Ngọc Quang (2A202600285) & Nguyễn Đông Hưng (2A202600392) | Lập trình / Developer Tools | Cursor vs GitHub Copilot |
| 2 | Hồ Thị Tố Nhi (2A202600369) | Nghiên cứu học thuật | Elicit vs NotebookLM |

---

## Phần 2 — Điều thấy hay từ nhóm khác

Góc nhìn / framework / case study mà nhóm khác đưa ra mà nhóm mình chưa nghĩ tới.

**Quan sát 1** (từ nhóm: Quách Ngọc Quang & Nguyễn Đông Hưng — Cursor vs Copilot):

- Cụ thể họ đưa ra: Trust signal cho sản phẩm AI viết code không phải là "citation" (trích dẫn nguồn) mà là "unit test" — người dùng verify output bằng cách chạy test, không cần đọc nguồn. Nhóm phân tích rõ rằng Cursor cho phép verify trong IDE nhanh hơn Copilot.
- Vì sao tôi thấy hay: Nhóm mình khi phân tích NotebookLM vs Elicit đã mặc định áp trust signal kiểu research (citation, source highlight). Nhưng thực ra "trust signal" phải được định nghĩa theo loại task — code dùng unit test, research dùng citation. Đây là sự phân biệt tinh tế mà nhóm mình bỏ qua.

**Quan sát 2** (từ nhóm: Quách Ngọc Quang & Nguyễn Đông Hưng — Cursor vs Copilot):

- Cụ thể họ đưa ra: GitHub Copilot có Distribution Moat mạnh hơn Cursor nhờ hệ sinh thái Microsoft/GitHub (PR, code review, issue), trong khi Cursor chỉ có Product Moat (UX tốt hơn). Nhóm nhận xét UX có thể bị sao chép, còn Distribution thì không.
- Vì sao tôi thấy hay: Nhóm mình phân tích NotebookLM có Distribution Moat (Google ecosystem) nhưng không đối chiếu trực tiếp với câu hỏi "moat nào bền hơn?" Cách nhóm Cursor/Copilot đặt câu hỏi này rõ ràng hơn và giúp người nghe hiểu ngay tại sao Copilot ít có nguy cơ bị disrupt hơn dù UX thua.

---

## Phần 3 — Điểm yếu / chỗ chưa thuyết phục

Bằng chứng yếu, lập luận lỏng, framework dùng sai. Chỉ rõ chỗ nào trong slide deck của nhóm khác.

**Điểm yếu 1** (từ nhóm: Quách Ngọc Quang & Nguyễn Đông Hưng — Cursor vs Copilot):

- Cụ thể: Phần Friction Analysis nhận định Copilot tạo "cognitive burden" do phải copy-paste thủ công từ chat sang editor, nhưng không có số liệu cụ thể — bao nhiêu bước, mất bao nhiêu giây so với Cursor's "Apply" button.
- Bằng chứng gì còn thiếu: Một con số thực nghiệm đơn giản (vd: "Cursor tốn 2 click, Copilot tốn 5 bước copy-paste") sẽ làm lập luận này thuyết phục hơn nhiều thay vì chỉ mô tả định tính.
- Tôi sẽ đề xuất họ làm thêm gì: Quay màn hình một workflow cụ thể (fix một bug nhỏ) trên cả hai tool, đếm số thao tác thủ công — dữ liệu quan sát trực tiếp này là "evidence" mạnh nhất.

**Điểm yếu 2** (từ nhóm: Hồ Thị Tố Nhi — Elicit vs NotebookLM):

- Cụ thể: Nhóm kết luận Elicit là "PROMISING" trong khi nhóm mình phân tích cùng hai sản phẩm nhưng kết luận Elicit "Strong (trong niche)". Hai verdict khác nhau nhưng không rõ sự khác biệt đến từ task context (nhóm tonhii dùng câu hỏi về sleep deprivation, nhóm mình dùng câu hỏi về AI productivity) hay từ cách đánh giá tiêu chí khác nhau.
- Bằng chứng gì còn thiếu: Nhóm cần làm rõ "PROMISING" nghĩa là gì trong framework đánh giá — tiêu chí nào bị thiếu khiến không đạt "Strong"? Nếu chỉ vì credit barrier (giới hạn gói miễn phí), đó là Business Moat issue chứ không phải product weakness.
- Tôi sẽ đề xuất họ làm thêm gì: Định nghĩa rõ rubric cho từng mức verdict (Weak / Promising / Strong) trước khi kết luận để người đọc có thể đối chiếu và không bị nhầm lẫn giữa product capability và pricing model.

---

## Phần 4 — Câu hỏi đặt cho nhóm khác

Câu hỏi gắn với bằng chứng cụ thể, không hỏi chung chung.

- Cho nhóm Quách Ngọc Quang & Nguyễn Đông Hưng (Cursor vs Copilot): Trong phần Data Flywheel, nhóm nói Cursor dựa vào "workspace cá nhân" còn Copilot dựa vào "toàn bộ GitHub repo" — vậy cụ thể cơ chế nào giúp Copilot học từ feedback người dùng? Nếu người dùng không chấp nhận suggestion, Copilot có ghi nhận tín hiệu đó không, hay flywheel chỉ chạy một chiều (pre-training)?
- Cho nhóm Hồ Thị Tố Nhi (Elicit vs NotebookLM): Nhóm test NotebookLM với task "sleep deprivation" — khi tải PDF lên, nhóm tự chọn các bài báo hay để Elicit tìm? Nếu tự chọn, thì đây là selection bias — người dùng đã biết trước kết quả và không phản ánh đúng trường hợp người mới hoàn toàn không có tài liệu nền.

---

## Phần 5 — Điều tôi rút ra cho bản thân

Bài học cụ thể tôi sẽ áp dụng vào lần phân tích sản phẩm AI tiếp theo. Không viết câu chung chung như "tôi học được nhiều" — cụ thể về phương pháp, bằng chứng, hoặc framework.

**Bài học 1**:

- Tôi sẽ làm khác lần sau: Định nghĩa Trust Signal theo loại task TRƯỚC khi bắt đầu phân tích, không áp dụng template chung. Code tool → verify bằng unit test / execution. Research tool → verify bằng citation và source grounding. Productivity tool → verify bằng time-on-task.
- Lý do: Nhóm Cursor/Copilot cho thấy nhóm mình đã vô tình áp "citation = trust" lên cả hai sản phẩm mà không xét xem người dùng thực sự kiểm chứng output theo cách nào.

**Bài học 2**:

- Tôi sẽ làm khác lần sau: Khi phân tích Moat, luôn kết thúc bằng câu hỏi "Moat nào bền hơn và tại sao?" thay vì chỉ liệt kê các loại moat từng sản phẩm có. Ví dụ: Distribution Moat > Product Moat vì UX có thể bị clone trong 6-12 tháng, còn ecosystem integration không thể.
- Lý do: Phần Moat của nhóm mình (NotebookLM vs Elicit) liệt kê đúng các loại moat nhưng không so sánh độ bền tương đối, khiến người đọc không biết sản phẩm nào defensible hơn về dài hạn.

**Bài học 3** (tuỳ chọn):

- Khi hai nhóm phân tích cùng sản phẩm nhưng cho verdict khác nhau (như Elicit: "PROMISING" vs "Strong in niche"), điều đó không có nghĩa là một nhóm sai — mà cho thấy verdict phụ thuộc vào task context và rubric chấm. Lần sau nên công bố rubric rõ ràng ngay từ đầu báo cáo để verdict có thể so sánh được giữa các nhóm.

---

## Checklist trước khi nộp

- [x] Phần 1 ghi rõ ≥ 2 nhóm đã quan sát (mã 2 học viên + ngành + sản phẩm).
- [x] Phần 2 có ≥ 2 quan sát hay, gắn với nhóm cụ thể.
- [x] Phần 3 có ≥ 2 điểm yếu / câu hỏi chưa được trả lời.
- [x] Phần 4 có ≥ 2 câu hỏi cụ thể cho nhóm khác.
- [x] Phần 5 có ≥ 2 bài học rút ra, kèm lý do và cách áp dụng lần sau.
