# Paper 07 Summary

## Citation

Tên bài: Developing an Early Warning System with Personalized Interventions to Enhance Academic Outcomes for At-Risk Students in Taiwanese Higher Education
Tác giả: Yuan-Hsun Chang, Feng-Chueh Chen, Chien-I Lee
Năm: 2025
Nguồn: Google Scholar
DOI/Link: https://www.mdpi.com/2227-7102/15/10/1321

## Problem

- Bài báo giải quyết vấn đề sự đứt gãy giữa mô hình dự đoán thuật toán và quy trình can thiệp thực tế trong các hệ thống cảnh báo sớm (EWS). Hầu hết nghiên cứu hiện tại chỉ tập trung tối ưu độ chính xác của AI (chạm trần lý thuyết) mà bỏ quên việc kiểm chứng thực nghiệm xem các biện pháp can thiệp có thực sự giúp sinh viên thoát rủi ro hay không. Đồng thời, các hệ thống EWS hiện nay phần lớn được thiết kế dựa trên văn hóa phương Tây (đề cao tính tự chủ cá nhân), tạo ra một khoảng trống lớn khi áp dụng vào các nền giáo dục Đông Á vốn chịu ảnh hưởng bởi Nho giáo (coi trọng thẩm quyền của giảng viên và mạng lưới hỗ trợ tập thể).

## Method

- Bài báo sử dụng phương pháp Thiết kế hỗn hợp hai giai đoạn (Two-phase mixed-methods design):
  - Giai đoạn 1 (Xây dựng mô hình): Khai phá dữ liệu giáo dục từ 2.856 sinh viên thuộc 64 khóa học trên hệ thống LMS để huấn luyện các mô hình học máy (Decision Trees, Random Forests, XGBoost) độc lập cho từng môn học.
  - Giai đoạn 2 (Thực nghiệm can thiệp): Tiến hành một thử nghiệm bán thực nghiệm (Quasi-experimental trial) trên nhóm sinh viên có rủi ro (n=48) vào tuần thứ 6 của học kỳ để đánh giá trực tiếp hiệu quả của các chiến lược can thiệp cá nhân hóa được điều chỉnh theo bối cảnh văn hóa.

## Context

- Bối cảnh nghiên cứu diễn ra tại một trường đại học tổng hợp ở Đài Loan. Đây là môi trường đại học đang phải đối mặt với tình trạng già hóa dân số (tỷ lệ sinh giảm), dẫn đến việc mở rộng cửa tuyển sinh đại học gần như đại trà (tỷ lệ trúng tuyển đạt 98% năm 2024), khiến chất lượng và mức độ chuẩn bị học thuật của sinh viên đầu vào vô cùng chênh lệch.

## Key Findings

- Trọng số của các biến dự đoán: Điểm số học thuật lịch sử (Previous semester grades), tỷ lệ điểm danh trên lớp (Attendance), và mô hình nộp bài tập (Assignment submission patterns) là những biến hành vi cốt lõi trên LMS giúp mô hình đạt độ chính xác phân loại cao (Balanced AUC = 0.85).
- Hiệu quả can thiệp vượt trội nhờ yếu tố văn hóa: Khi áp dụng cơ chế can thiệp cá nhân hóa có sự chủ động thúc đẩy của giảng viên/cố vấn (phù hợp với tư duy Nho giáo thích nghe theo chỉ dẫn của người có chuyên môn), 73% sinh viên thuộc nhóm nguy cơ cao đã lội ngược dòng thành công và đạt điểm qua môn.
- Kích thước hiệu ứng (Effect Size) khổng lồ: Phân tích thực nghiệm cho thấy mức độ cải thiện học thuật của nhóm can thiệp đạt chỉ số Cohen's d = 0.91. Đây là một con số cực lớn so với các tiêu chuẩn công nghệ giáo dục thông thường (chỉ dao động từ 0.3 - 0.5).
- Bằng chứng về Hệ thống Kinh tế - Kỹ thuật (Socio-Technical): Nghiên cứu chứng minh tính đúng đắn của giả thuyết: Sự thành công của một hệ thống AI giáo dục không nằm ở thuật toán tách biệt, mà nằm ở sự phối hợp nhịp nhàng giữa cảnh báo chính xác của máy và mạng lưới hỗ trợ nhân văn của con người (giảng viên, trung tâm tư vấn, cố vấn học tập).

## Limitations

- Giới hạn quy mô mẫu thử nghiệm thực tế: Dù dữ liệu huấn luyện thuật toán ở Giai đoạn 1 rất lớn (hơn 2.800 sinh viên) , quy mô nhóm đối chứng và thực nghiệm ở Giai đoạn 2 phục vụ cho việc can thiệp chuyên sâu chỉ giới hạn ở mức 48 sinh viên của một khóa học cụ thể. Do đó, hiệu quả can thiệp trên diện rộng ở các ngành học có đặc thù khác nhau (như khối kỹ thuật chuyên sâu so với khối khoa học xã hội) cần được kiểm chứng thêm.
- Ràng buộc đạo đức trong nghiên cứu: Do yêu cầu đạo đức giáo dục không cho phép bỏ mặc sinh viên yếu kém (không thể chia nhóm một cách ngẫu nhiên tuyệt đối để một nhóm rủi ro hoàn toàn không được hỗ trợ làm đối chứng), nhóm nghiên cứu phải sử dụng nhóm sinh viên không bị cảnh báo làm nhóm đối chứng. Điều này làm ảnh hưởng phần nào đến tính thuần khiết của thiết kế thực nghiệm truyền thống.

## Relevance to our topic

- Hợp thức hóa bối cảnh văn hóa tương đồng: Hệ thống giáo dục đại học Việt Nam (và cụ thể là tại Đại học FPT) có sự tương đồng rất lớn với Đài Loan về bối cảnh văn hóa Đông Á, nơi sinh viên tôn trọng giảng viên và quen với việc được dẫn dắt chủ động thay vì hoàn toàn tự học kiểu phương Tây. Nhóm có thể bê lập luận này vào phần đặc tả yêu cầu của hệ thống: "Hệ thống SEWS không chỉ gửi mail tự động cho sinh viên (mô hình phương Tây), mà phải cung cấp một Dashboard chuyên biệt cho Giảng viên và Phòng dịch vụ sinh viên để họ chủ động can thiệp (mô hình Đông Á đã được Chang et al., 2025 chứng minh hiệu quả cực cao)".
- Thiết kế tính năng can thiệp khép kín (Closed-loop): Giúp nhóm đưa ra các yêu cầu chức năng cụ thể cho hệ thống: Ghi nhận trạng thái can thiệp (Giảng viên đã gặp sinh viên chưa? Sinh viên có cải thiện bài tập tuần sau không?), thực hiện đúng chu trình "Dự đoán - Can thiệp - Đánh giá lại hành vi" mà bài báo đề xuất.
