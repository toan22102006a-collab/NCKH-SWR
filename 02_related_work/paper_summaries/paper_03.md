# Paper 03 Summary

## Citation

Tên bài: A Requirements Engineering Perspective to AI-based Systems Development: A Vision Paper 
Tác giả: Xavier Franch, Andreas Jedlitschka, Silverio Martínez-Fernández
Năm: 2023
Nguồn: Springer
DOI/Link: https://upcommons.upc.edu/server/api/core/bitstreams/590b8cce-d439-4b67-8958-d00ed7802cef/content

## Problem

- Bài báo giải quyết vấn đề sự thiếu hụt một khung phương pháp luận hoàn chỉnh và vai trò cốt lõi của Kỹ nghệ Yêu cầu (RE) trong quy trình phát triển hệ thống dựa trên AI. Các đặc tính đặc thù của AI (như tính bất định, sự phụ thuộc vào dữ liệu, hành vi tự học) làm sụp đổ các cách tiếp cận RE truyền thống. Bài báo đặt câu hỏi lớn: RE cần phải thay đổi như thế nào về mặt vai trò nhân sự, phạm vi yêu cầu và các yêu cầu phi chức năng để trở thành nền tảng thành công cho các dự án AI?

## Method

- Bài báo sử dụng phương pháp Bài báo định hướng tầm nhìn (Vision Paper) kết hợp với Phân tích học thuật phê phán (Conceptual Analysis & Roadmapping). Nhóm tác giả dựa trên kinh nghiệm nghiên cứu, các thách thức thực tế và lý thuyết phần mềm hiện tại để tổng hợp, cấu trúc hóa vấn đề thành 3 trụ cột lớn, từ đó vạch ra một lộ trình nghiên cứu (Research Roadmap) cho tương lai.

## Context

- Bối cảnh nghiên cứu đặt trong giai đoạn các hệ thống tích hợp mô hình AI/ML đang bùng nổ và len lỏi vào mọi góc cạnh của xã hội (giai đoạn 2022–2023 trở đi). Nghiên cứu không giới hạn ở một ngành cụ thể mà xem xét toàn cục quy trình kỹ nghệ phần mềm cho hệ thống AI (SE4AI), nơi có sự tham gia của nhiều bên liên quan mới và có sự giao thoa phức tạp giữa kỹ nghệ mã nguồn (Code engineering) và kỹ nghệ dữ liệu (Data engineering).

## Key Findings

- Sự chuyển dịch về Vai trò (Roles Involved): Quy trình làm RE cho AI không còn là việc riêng của Kỹ sư yêu cầu (Requirements Engineer) và Khách hàng. Nó bắt buộc phải tích hợp vai trò của Nhà khoa học dữ liệu (Data Scientist). Bài báo nhấn mạnh RE phải là "cầu nối ngôn ngữ" giữa mục tiêu kinh doanh của khách hàng và các thuật toán toán học của Data Scientist.

- Mở rộng Phạm vi Yêu cầu (Requirements' Scope): Yêu cầu đối với hệ thống AI không chỉ dừng lại ở chức năng phần mềm mà phải mở rộng ra 3 thành phần: Yêu cầu về Phần mềm (Software), Yêu cầu về Mô hình AI (Model), và Yêu cầu về Dữ liệu (Data). RE phải quản lý được sự tiến hóa liên tục của dữ liệu và sự suy giảm hiệu năng của mô hình theo thời gian.

- Tái định nghĩa Yêu cầu phi chức năng (NFRs cho AI): Các đặc tính chất lượng truyền thống phải được thay thế hoặc bổ sung bằng các NFRs đặc thù của AI bao gồm: Tính công bằng (Fairness), Tính giải thích được (Explainability), Tính an toàn/bảo mật của mô hình (Robustness/Safety), và Trách nhiệm giải trình (Accountability).

## Limitations

- Mang tính lý thuyết và định hướng vĩ mô: Vì là một Vision Paper, bài báo chỉ dừng lại ở việc đưa ra tầm nhìn, khung khái niệm và vạch lộ trình nghiên cứu chứ chưa cung cấp một framework kỹ thuật chi tiết, chưa có công cụ cụ thể hoặc các số liệu thực nghiệm (empirical data) để chứng minh tính hiệu quả của các đề xuất.

- Chưa có Case Study cụ thể: Các luận điểm được đưa ra mang tính tổng quát cho mọi hệ thống AI, chưa được kiểm chứng trên các miền ứng dụng đặc thù (như y tế, giáo dục hay tài chính).

## Relevance to our topic

- Xây dựng cấu trúc cho Literature Review Matrix: Bài báo gợi ý rất rõ cho nhóm rằng khi thu thập yêu cầu cho hệ thống cảnh báo sớm AI, nhóm phải chia ma trận yêu cầu thành 3 nhánh rõ rệt: Yêu cầu về phần mềm (giao diện, thông báo), Yêu cầu về mô hình (thuật toán Random Forest/XGBoost), và Yêu cầu về dữ liệu (LMS log, điểm số).

- Định hình quy trình làm việc nhóm (gợi ý cho phần Methodology): Giúp nhóm phân định rõ vai trò khi làm RE: thành viên nào đóng vai trò Kỹ sư yêu cầu để làm việc với Phòng đào tạo/Sinh viên, thành viên nào đóng vai trò Data Scientist để dịch chuyển các yêu cầu đó thành thuộc tính dữ liệu.

- Luận điểm cốt lõi để viết Abstract: Nhóm có thể trích dẫn tư duy của bài báo này để viết phần đặt vấn đề: Do hệ thống SEWS dựa trên AI mang tính bất định, việc áp dụng cách tiếp cận RE phối hợp giữa Phần mềm - Mô hình - Dữ liệu là bắt buộc để đảm bảo hệ thống vận hành thực tế thành công.