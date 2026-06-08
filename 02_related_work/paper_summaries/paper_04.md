# Paper 04 Summary

## Citation

Tên bài: Requirements Engineering for Machine Learning-Based AI Systems: A Tertiary Study
Tác giả: Mariana Crisostomo Martins, Lívia Mancine C. Campos, João Lucas R. Soares, Taciana Novo Kudo, Renato F. Bulcão-Neto
Năm: 2025
Nguồn: Journal of Software Engineering Research and Development
DOI/Link: https://journals-sol.sbc.org.br/index.php/jserd/article/view/4892/3438

## Problem

- Bài báo giải quyết vấn đề phân mảnh và thiếu sự đồng bộ trong tri thức về Kỹ nghệ Yêu cầu cho Hệ thống học máy (RE4ML). Mặc dù có rất nhiều nghiên cứu thứ cấp (như Systematic Mapping, Systematic Literature Review) về chủ đề này trong thập kỷ qua, nhưng chưa có một nghiên cứu bậc 3 (Tertiary Study) nào đứng ra tổng hợp, phân tích và đánh giá chất lượng của chính các nghiên cứu thứ cấp đó nhằm đưa ra một bức tranh toàn cảnh, có hệ thống về các giải pháp, công cụ, thách thức và khoảng trống nghiên cứu hiện tại.

## Method

- Bài báo sử dụng phương pháp Nghiên cứu tổng quan cấp bậc 3 (Tertiary Study / Guidelines by Kitchenham):
  - Thực hiện một quy trình nghiêm ngặt từ lập đề cương (Protocol), tìm kiếm tự động trên 5 cơ sở dữ liệu lớn và áp dụng kỹ thuật tìm kiếm "Snowballing".

  - Lọc và chọn ra 11 nghiên cứu thứ cấp chất lượng cao (được xuất bản từ năm 2019 đến 2023).

  - Áp dụng thang đo DARE (Database of Abstracts of Reviews of Effects) để đánh giá chất lượng (Quality Assessment) của các nghiên cứu thứ cấp này trước khi tổng hợp tri thức.

## Context

- Bối cảnh đặt trong hệ sinh thái Kỹ nghệ Phần mềm cho AI (SE4AI / RE4ML) toàn cầu. Nghiên cứu xem xét toàn bộ các giai đoạn trong vòng đời RE truyền thống (Lấy yêu cầu, Phân tích, Đặc tả, Kiểm chuẩn, Quản lý) nhưng đặt trong bối cảnh bị thách thức bởi các đặc tính kỹ thuật phức tạp của Học máy (ML) như tính phụ thuộc dữ liệu, tính bất định (uncertainty) và "hộp đen" thuật toán.

## Key Findings

- Các giai đoạn RE được tập trung nhiều nhất: Giai đoạn Lấy yêu cầu (Elicitation) và Đặc tả yêu cầu (Specification) là hai nhánh được nghiên cứu sâu nhất và có nhiều giải pháp đề xuất nhất, vì đây là nơi xảy ra xung đột lớn nhất giữa yêu cầu người dùng và khả năng của dữ liệu.

- Các phương pháp/công cụ RE4ML phổ biến: Bài báo chỉ ra các công cụ/framework hàng đầu hiện nay được áp dụng cho AI bao gồm: GR4ML (Goal-Oriented RE cho ML), Straw-man proposal, các mẫu biểu đặc tả (Templates), và Ma trận chất lượng dữ liệu (Data Quality Matrices).

- Sự dịch chuyển của Yêu cầu phi chức năng (NFRs): Khẳng định lại tính sống còn của các thuộc tính: Tính giải thích được (Explainability), Tính minh bạch (Transparency), Độ tin cậy (Reliability), và Tính an toàn (Safety) đối với hệ thống AI.

- Các khoảng trống lớn (Research Gaps): \* Thiếu các công cụ tự động hóa hỗ trợ kỹ sư làm RE4ML.
  - Giai đoạn Kiểm chuẩn yêu cầu (Validation) và Quản lý yêu cầu (Management) cho AI còn rất sơ khai, chưa được quan tâm đúng mức.

  - Thiếu các nghiên cứu thực nghiệm quy mô lớn trong môi trường công nghiệp thực tế.

## Limitations

- Giới hạn thời gian thu thập dữ liệu thứ cấp: Các nghiên cứu thứ cấp được chọn chỉ bao gồm các bài xuất bản từ năm 2019 đến năm 2023, điều này có nghĩa là một số nghiên cứu mới xuất sắc trong giai đoạn 2024–2025 chưa được tích hợp vào mô hình phân tích của bài báo này.

- Sự phụ thuộc vào chất lượng của nghiên cứu gốc: Vì là nghiên cứu bậc 3, nếu các nghiên cứu thứ cấp hoặc các nghiên cứu sơ cấp (primary studies) trước đó có những sai lệch về dữ liệu hoặc báo cáo không rõ ràng, kết quả tổng hợp của bài báo này cũng sẽ bị ảnh hưởng theo (bài báo có thừa nhận thách thức này trong phần Threat to Validity).

## Relevance to our topic

- Cung cấp bằng chứng thuyết phục cho phần Introduction/Abstract: Nhóm có thể dùng kết luận của bài báo này (một bài báo năm 2025) để lập luận: "Nghiên cứu bậc 3 mới nhất cho thấy quy trình Kiểm chuẩn (Validation) và công cụ hỗ trợ RE cho AI vẫn còn bỏ ngỏ. Nghiên cứu này của nhóm đóng đóng góp vào việc lấp đầy khoảng trống đó bằng cách áp dụng quy trình RE cụ thể vào hệ thống cảnh báo sớm sinh viên".

- Định hướng lựa chọn Công cụ/Framework: Giúp nhóm tự tin lựa chọn hướng tiếp cận Goal-Oriented (GR4ML) hoặc sử dụng các Mẫu biểu đặc tả (Specification Templates) cho hệ thống SEWS của mình, vì bài báo đã chứng minh đây là các giải pháp có độ đồng thuận và hiệu quả cao nhất trong giới học thuật hiện tại.
