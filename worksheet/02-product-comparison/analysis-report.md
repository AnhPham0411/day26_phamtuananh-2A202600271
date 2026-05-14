---
title: Báo cáo Phân tích Sản phẩm AI (Lab 2)
author: Nguyễn Xuân Hoàng & Phạm Tuấn Anh
date: 2026-05-14
---

# Báo cáo Phân tích Sản phẩm AI - Track [D] Nghiên cứu

**Nhóm thực hiện:**
- Nguyễn Xuân Hoàng (2A202600488)
- Phạm Tuấn Anh (2A202600271)

**Sản phẩm:** NotebookLM (Google) vs. Elicit
**Nhiệm vụ:** Tổng hợp bằng chứng thực nghiệm về tác động của Generative AI đến năng suất lập trình viên phần mềm.

---

## S1 — Product Moment

- **Sản phẩm & Nhiệm vụ:** NotebookLM và Elicit cùng xử lý nhu cầu nghiên cứu chuyên sâu (Deep Research).
- **Entry Point (Điểm bắt đầu):** 
  - **NotebookLM:** Giao diện quản lý "Notebook". Người dùng phải chủ động tải lên (upload) các tài liệu nguồn (PDF, link web, text) trước khi bắt đầu đặt câu hỏi.
  - **Elicit:** Giao diện tìm kiếm trực tiếp trên cơ sở dữ liệu học thuật. Người dùng nhập câu hỏi nghiên cứu thẳng vào thanh tìm kiếm.

---

## S2 — Workflow Evidence

**Quy trình (Trước / Trong / Sau):**
1. **Trước:** 
   - *NotebookLM:* Tải 3 bài báo PDF về năng suất AI (vd: báo cáo của GitHub Copilot, Microsoft) vào hệ thống.
   - *Elicit:* Nhập câu hỏi "Impact of Generative AI on software developer productivity empirical evidence".
2. **Trong:** 
   - *NotebookLM:* Xử lý nội bộ (RAG cá nhân) rất nhanh.
   - *Elicit:* Quét qua hơn 200 triệu bài báo trong database, lọc ra top 4-8 bài báo liên quan nhất.
3. **Sau:** 
   - *NotebookLM:* Trả lời dạng văn bản hội thoại, đính kèm các "chấm" trích dẫn. Click vào trích dẫn sẽ mở giao diện chia đôi màn hình (split-screen), highlight đúng đoạn văn trong PDF.
   - *Elicit:* Trả về dạng Bảng (Table) so sánh. Các cột gồm: Tên bài báo, Main Findings, Methodology, Population.

**3 Điểm nghẽn (Friction Areas) trong Workflow:**
- *Friction 1 (Quyền truy cập dữ liệu):* Elicit bị giới hạn bởi các bài báo Open Access; nếu bài báo bị paywall, nó chỉ đọc được abstract. NotebookLM yêu cầu người dùng phải tự có sẵn file PDF.
- *Friction 2 (Định dạng đầu ra):* Khi cần so sánh đa chiều, dạng chat của NotebookLM khó nhìn hơn dạng Bảng của Elicit.
- *Friction 3 (Đóng khung kiến thức):* NotebookLM hoàn toàn "mù" về thế giới bên ngoài nếu thông tin không có trong file PDF tải lên. Elicit có thể bị "lạc" sang các bài báo không thực sự chất lượng nếu câu prompt không đủ hẹp.

---

## S3 — Output & Trust

**Chất lượng đầu ra & Tín hiệu đáng tin (Trust Signals):**
- **NotebookLM:** 
  - *Trust Signal cực mạnh:* "Grounded AI" (AI bám sát nguồn). Nếu tài liệu không có, nó sẽ trả lời "Tài liệu không đề cập". 
  - Giao diện highlight nguyên văn trong file PDF gốc giúp người dùng tin tưởng 100% vào nguồn gốc thông tin.
- **Elicit:** 
  - *Trust Signal học thuật:* Trích xuất trực tiếp câu văn từ bài báo. 
  - Cung cấp các meta-data quan trọng của giới nghiên cứu như: Số lượng trích dẫn (Citations), tạp chí đăng bài, năm xuất bản, giúp đánh giá độ uy tín của nguồn.

---

## S4 — Business Signal

- **Giá cả & Giới hạn:** 
  - **NotebookLM:** Miễn phí (hiện tại). Bị giới hạn 50 nguồn/notebook, 500.000 từ/nguồn.
  - **Elicit:** Có gói miễn phí (giới hạn số lượt tóm tắt/trích xuất). Gói Plus ($12/tháng), Pro ($49/tháng).
- **Cost-Capability-Speed:** Cả hai đều cung cấp "siêu năng lực" (Capability) phân tích lượng lớn văn bản trong vài giây, thay thế hàng giờ đồng hồ đọc tài liệu thủ công.

---

## S5 — Product Judgment (Mở rộng 8 mục)

### S5.1 Verdict (Đánh giá)
- **NotebookLM: Strong.** Trải nghiệm UI/UX xuất sắc nhất cho tác vụ "trò chuyện với dữ liệu cá nhân/nội bộ". Tính năng Audio Overview tạo ra sự khác biệt lớn.
- **Elicit: Strong (trong niche).** Là công cụ không thể thiếu cho các nhà nghiên cứu, sinh viên làm Literature Review nhờ giao diện Bảng (Table) chuyên biệt.

### S5.2 User Base & Growth
- **NotebookLM:** Tăng trưởng bùng nổ trong năm 2024 (vài triệu MAU), thu hút cả người dùng phổ thông nhờ tính năng tạo Podcast từ PDF.
- **Elicit:** Quy mô nhỏ hơn (vài trăm ngàn users), tập trung vào ngách học thuật (Researcher, PhD).

### S5.3 Doanh thu / Pricing Power
- **NotebookLM:** Không có doanh thu trực tiếp, đóng vai trò tạo hệ sinh thái kéo người dùng mua Google One AI Premium.
- **Elicit:** Có Pricing Power rất cao trong giới hàn lâm vì nó giải quyết trực tiếp "nỗi đau" đọc hàng trăm bài báo tốn thời gian.

### S5.4 Moat (Lợi thế cạnh tranh 5 loại)
- **NotebookLM:** Dựa vào **Distribution Moat** (hệ sinh thái Google) và lợi thế công nghệ (Context window 2M tokens). Tuy nhiên, vì "tốc độ không phải là moat vĩnh cửu", NotebookLM cần nhanh chóng chuyển hóa tập user hiện tại thành *Switching Cost Moat* (chi phí chuyển đổi) khi người dùng đã tạo quá nhiều Notebook và quen thuộc với hệ thống.
- **Elicit:** Sở hữu **Data Moat** vững chắc (200M+ bài báo khoa học được cấu trúc hóa). Đây là tầng phòng thủ (defensibility) quan trọng giúp Elicit không bị các Horizontal AI (như ChatGPT) sao chép dễ dàng.

### S5.5 Data Flywheel
- **Elicit:** Càng nhiều người dùng đánh giá (Thumbs up/down) kết quả trích xuất, mô hình càng học được cách tìm kiếm và tóm tắt bài báo khoa học chính xác hơn.
- **NotebookLM:** Google thu thập hành vi người dùng tương tác với tài liệu lớn để tối ưu hóa thuật toán RAG nội bộ.

### S5.6 Niche Down & AI Feature Map
- **NotebookLM:** 
  - **Niche Down:** Tỏa sáng nhờ *proprietary functionality* (Audio Overview, Grounded UI) và *accuracy/citation* (bám sát 100% tài liệu). 
  - **AI Feature Map:** Đạt *User Value* cao (nắm bắt nhanh kiến thức nội bộ); *User Alignment* hoàn hảo (không hallucinate, tin tưởng tuyệt đối); *Business Value* lớn khi đổi chi phí inference lấy capability đọc hiểu hàng triệu token.
- **Elicit:**
  - **Niche Down:** Phòng thủ bằng *proprietary data* (kho bài báo khoa học) và giải quyết *translation work* (làm thay việc tổng hợp Literature Review).
  - **AI Feature Map:** *User Value* rõ ràng (tiết kiệm hàng tuần đọc bài); *User Alignment* tốt (dẫn nguồn chính xác, minh bạch); *Business Value* tối ưu (người dùng sẵn sàng trả $12/tháng để làm việc của một trợ lý nghiên cứu).

### S5.7 Spark → Loop → System
- **NotebookLM:** Đang ở giai đoạn chuyển giao từ **Spark** sang **Loop**. Tính năng Audio Overview tạo ra một "Spark" lan truyền (viral) khổng lồ trên mạng xã hội. Tuy nhiên, Google cần xây dựng các "Loop" (như chia sẻ Notebook cộng tác) để giữ chân người dùng lâu dài trước khi tạo thành một **System** bền vững.
- **Elicit:** Đã tiến vào giai đoạn **System** trong ngách học thuật. Nó sở hữu các loop tự củng cố: người dùng review kết quả trích xuất -> data tốt hơn -> kết quả chính xác hơn -> tiếp tục củng cố giá trị cho giới researcher.

### S5.8 Liên hệ Lab 1 (Disruption Risk)
- Sự phát triển của các công cụ Deep Research (như Elicit và NotebookLM) mang đến nguy cơ gián đoạn (disruption) mạnh mẽ cho các dịch vụ Research Assistant cấp thấp hoặc các công ty chuyên làm báo cáo tổng hợp dữ liệu thứ cấp (Desk Research). Giống như cách Klarna loại bỏ 700 FTEs của BPO (Lab 1), một nhà phân tích giờ đây có thể dùng Elicit làm lượng công việc của 5 trợ lý nghiên cứu cộng lại.
