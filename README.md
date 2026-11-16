Đề bài / Yêu cầu

1. Mục tiêu

- Nhận diện đúng bản chất hoạt động xác suất thống kê (Next Token Prediction) của các mô hình ngôn ngữ lớn (LLM).

- Phân biệt sự khác nhau giữa một "hệ thống suy tư/tính toán logic" với một "máy tính toán xác suất chuỗi từ" dựa trên dữ liệu Pre-training.

2. Bối cảnh & Phát biểu sai

Nam là chuyên viên dữ liệu tại Siêu thị MartX. Khi nhập câu hỏi: "15.480 + 28.750 bằng bao nhiêu?" vào ChatGPT, Nam nhận được kết quả sai là 44.130 (đáp án đúng phải là 44.230). Nam hoảng loạn và viết báo cáo lên Trưởng phòng:

> "AI bị hỏng phần mềm hoặc máy chủ bị lỗi tính toán! ChatGPT là kho trí tuệ nhân tạo thông minh có dung lượng hàng trăm tỷ tham số thì chắc chắn phải có bộ vi xử lý máy tính bên trong để tính toán chính xác 100% mọi phép tính số học tiểu học này chứ!"

3. Bẫy tư duy

Bẫy: Nam lầm tưởng LLM là một máy tính bỏ túi (Calculator) có khả năng thực thi thuật toán số học logic, trong khi thực tế LLM chỉ ghép từ tiếp theo dựa trên xác suất xuất hiện chuỗi ký tự trong giai đoạn Pre-training.

4. Yêu cầu đầu ra

- Phần 1 (Bóc tách nhận thức sai): Dựa vào Mục 2.1 Lesson 01, hãy chỉ ra 2 điểm sai lầm trong báo cáo của Nam. Trích dẫn thuật ngữ "Next Token Prediction" và "Pre-training" từ bài đọc để giải thích tại sao LLM lại tính sai phép cộng trên.

2 điểm sai lầm của Nam:

Nhầm lẫn LLM với một máy tính bỏ túi (Calculator) thực thi thuật toán logic.

Quy chụp hệ thống bị lỗi phần mềm hoặc máy chủ khi AI tính sai.

Giải thích nguyên nhân: LLM không biết làm toán logic mà chỉ hoạt động theo cơ chế Next Token Prediction (dự đoán từ/ký tự tiếp theo). Nó ghép các con số dựa trên xác suất thống kê từ dữ liệu Pre-training (huấn luyện trước), nên dễ đoán nhầm với các phép tính phức tạp

- Phần 2 (Sửa lỗi & Prompting): Đề xuất câu lệnh (Prompt) chuẩn giúp ChatGPT kích hoạt công cụ bổ trợ (ví dụ: Code Interpreter / Python) hoặc yêu cầu AI suy luận để cho ra kết quả số học chính xác 100%.

Prompt chuẩn: "Hãy sử dụng công cụ Python (Code Interpreter) để tính chính xác phép tính: 15.480 + 28.750 và chỉ trả về kết quả cuối cùng."

Tác dụng: Ép AI dùng trình chạy mã thực thụ để tính toán chuẩn xác 100%, thay vì tự đoán chữ số theo xác suất.

