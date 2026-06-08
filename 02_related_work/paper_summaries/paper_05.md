# Paper 05 Summary

## Citation

Tên bài: How mature is requirements engineering for AI‑based systems? A systematic mapping study on practices, challenges, and future research directions
Tác giả: Umm-e-Habiba, Markus Haug, Justus Bogner, Stefan Wagner
Năm: 2024
Nguồn: Springer
DOI/Link: https://link.springer.com/article/10.1007/s00766-024-00432-3

## Problem

- Bài báo giải quyết vấn đề sự mơ hồ về mức độ trưởng thành (maturity) của các phương pháp Kỹ nghệ Yêu cầu hiện tại khi áp dụng vào hệ thống AI (RE4AI). Trước làn sóng bùng nổ của AI, giới nghiên cứu và thực nghiệp vẫn chưa rõ liệu các kỹ thuật RE truyền thống có còn đủ dùng hay không, những thực tiễn (practices) nào đã có sẵn, những thách thức nào đang áp đảo và đâu là khoảng trống nghiên cứu cần được giải quyết khẩn cấp.

## Method

- Bài báo sử dụng phương pháp Nghiên cứu bản đồ hệ thống (Systematic Mapping Study - SMS) cực kỳ nghiêm ngặt:

    - Kết hợp giữa tìm kiếm bằng chuỗi truy vấn (query string search) và kỹ thuật tìm kiếm "thác đổ" mở rộng (extensive snowballing).

    - Áp dụng quy trình sàng lọc chặt chẽ để chọn lọc ra 126 nghiên cứu sơ cấp (primary studies) chất lượng cao làm dữ liệu phân tích.

    - Sử dụng phương pháp Phân tích chủ đề (Thematic Analysis) để tổng hợp, phân loại tri thức và cấu trúc hóa các phát hiện.

## Context

- Bối cảnh đặt trong toàn bộ vòng đời phát triển và các giai đoạn kỹ nghệ yêu cầu của hệ thống dựa trên AI (AI-based systems) trên quy mô toàn cầu. Nghiên cứu khảo sát từ các lý thuyết học thuật cho đến thực tiễn công nghiệp phần mềm, bao quát các khía cạnh từ việc chỉ định yêu cầu kỹ thuật (specification) cho đến các hệ quả đạo đức mới nổi ảnh hưởng đến các thuộc tính chất lượng của AI.

## Key Findings

- Sự phân bổ nghiên cứu không đồng đều: Phần lớn các nghiên cứu về RE4AI hiện tại tập trung quá nhiều vào hai giai đoạn: Phân tích yêu cầu (Requirements Analysis) và Lấy yêu cầu (Requirements Elicitation).

- Các thực tiễn (Practices) phổ biến: Đã có một số giải pháp xuất hiện như các mẫu đặc tả (specification templates), phương pháp tiếp cận dựa trên mục tiêu (goal modeling) được tùy biến cho AI, và các hướng dẫn trích xuất thuộc tính chất lượng dữ liệu.

- Thách thức lớn nhất (Dominant Challenges): * Đặc tả và Kiểm chuẩn: Việc định nghĩa rõ ràng và kiểm thử/kiểm chuẩn (validation) các yêu cầu cho AI cực kỳ khó khăn do tính không thể đoán trước (non-deterministic nature) của mô hình.

    - Yêu cầu chất lượng mới (Quality Requirements): Sự xuất hiện của các yêu cầu đạo đức học (ethical implications) ép buộc hệ thống phải tích hợp các thuộc tính phi chức năng mới.

- Kết luận về mức độ trưởng thành: Ngành RE4AI chưa thực sự trưởng thành. Các giải pháp hiện tại phần lớn mang tính đề xuất lý thuyết, thiếu các công cụ tự động hóa hỗ trợ và thiếu nghiêm trọng các thực nghiệm chứng minh trong môi trường công nghiệp thực tế.

## Limitations

- Tính chất của Systematic Mapping Study: Bài báo tập trung vào việc "vẽ bản đồ" phân loại và thống kê số lượng/xu hướng nghiên cứu (phần lớn là phân tích phân bổ bề nổi), nên nó không đi quá sâu vào việc đánh giá chi tiết tính hiệu quả kỹ thuật hoặc so sánh chuyên sâu từng thuật toán/công cụ cụ thể trong 126 bài báo đó.

- Thời điểm chốt dữ liệu: Mặc dù xuất bản năm 2024, quy trình thu thập dữ liệu (data extraction) có một khoảng trễ nhất định so với tốc độ thay đổi chóng mặt từng tháng của các công nghệ AI thế hệ mới (Generative AI/LLMs) cuối năm 2024 - 2025.

## Relevance to our topic

- Hỗ trợ xây dựng Literature Review Matrix và phần Gap: Nhóm có thể dựa vào phân tích của bài báo (ngành RE4AI thiếu các nghiên cứu thực nghiệm thực tế và thiếu công cụ cụ thể) để làm đòn bẩy lập luận. Nhóm sẽ chỉ ra rằng: "Hệ thống SEWS dựa trên AI của nhóm không chỉ dừng lại ở lý thuyết RE mà là một thực nghiệm thực tế áp dụng quy trình RE4AI vào bối cảnh giáo dục đại học, giải quyết trực tiếp bài toán thiếu kiểm chứng thực nghiệm mà Umm-e-Habiba et al. (2024) đã chỉ ra".

- Xây dựng danh mục Yêu cầu phi chức năng (NFR Checklist): Nhóm có thể kế thừa trực tiếp cấu trúc phân loại "Yêu cầu chất lượng mới do hệ quả đạo đức" được tổng hợp trong bài báo này để thiết kế các tính năng đảm bảo an toàn dữ liệu điểm số, thuật toán không thiên vị cho hệ thống cảnh báo sớm của mình.