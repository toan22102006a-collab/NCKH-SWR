# Paper 06 Summary

## Citation

Tên bài: Predicting Academic Success and Identifying At-Risk Students: A Systematic Review of Data Analytics and Machine Learning Approaches in Higher Education Institutions
Tác giả: Patrick Ngulube, Mthokozisi Masumbika Ncube
Năm: 2025
Nguồn: Google Scholar
DOI/Link: https://www.researchgate.net/profile/Patrick-Ngulube/publication/388481720_Predicting_Academic_Success_and_Identifying_At-Risk_Students_A_Systematic_Review_of_Data_Analytics_and_Machine_Learning_Approaches_in_Higher_Education_Institutions/links/67b930908311ce680c6f60d2/Predicting-Academic-Success-and-Identifying-At-Risk-Students-A-Systematic-Review-of-Data-Analytics-and-Machine-Learning-Approaches-in-Higher-Education-Institutions.pdf

## Problem

- Bài báo giải quyết vấn đề thiếu một sự tổng hợp toàn diện và đánh giá có hệ thống về tính hiệu quả, các thuật toán phổ biến và các nguồn dữ liệu đầu vào được sử dụng để dự đoán thành tích học tập và phát hiện sinh viên có rủi ro (at-risk) tại các cơ sở giáo dục đại học (HEIs). Mặc dù có nhiều nghiên cứu đơn lẻ, nhà quản lý giáo dục vẫn thiếu một cái nhìn tổng quan để biết mô hình nào hoạt động tốt nhất và những rào cản nào đang cản trở việc triển khai thực tế.

## Method

- Bài báo sử dụng phương pháp Tổng quan tài liệu có hệ thống (Systematic Literature Review - SLR):

    - Thực hiện tìm kiếm nghiêm ngặt theo các tiêu chuẩn học thuật trên các cơ sở dữ liệu lớn (như Scopus, Web of Science, Google Scholar).

    - Áp dụng các tiêu chí lựa chọn và loại trừ nghiêm ngặt để lọc ra các bài báo chất lượng cao.

    - Tổng hợp dữ liệu để trả lời các câu hỏi nghiên cứu về: loại thuật toán, loại dữ liệu sử dụng, độ chính xác của mô hình và các thách thức khi triển khai thực tế tại các trường đại học.

## Context

- Bối cảnh nghiên cứu đặt tại các cơ sở giáo dục đại học (HEIs) trên toàn cầu đang đối mặt với áp lực lớn trong việc nâng cao tỷ lệ tốt nghiệp, giảm tỷ lệ bỏ học và tối ưu hóa các chiến lược hỗ trợ sinh viên. Nghiên cứu xem xét các hệ thống phân tích dữ liệu dưới góc nhìn quản lý giáo dục và ứng dụng kỹ thuật thực tế.

## Key Findings

- Các thuật toán thống trị hiệu năng: Khẳng định các thuật toán như Random Forest, Support Vector Machines (SVM), và K-Nearest Neighbors (KNN) là những mô hình được sử dụng phổ biến nhất và liên tục đạt độ chính xác cao nhất trong việc phân loại sinh viên có rủi ro học thuật.

- Các nguồn dữ liệu đầu vào cốt lõi: Dữ liệu để dự đoán thành công của sinh viên được chia làm 3 nhóm chính: Kết quả học tập lịch sử (GPA, điểm thi), Dữ liệu nhân khẩu học (Demographics), và Mức độ tương tác hành vi trên Hệ thống quản lý học tập (LMS/VLE log data). Sự kết hợp đa nguồn dữ liệu luôn cho kết quả tốt hơn đơn nguồn.

- Lợi ích thực tế mang lại: Việc triển khai các mô hình này giúp các trường đại học chuyển dịch từ cơ chế "ứng phó thụ động" (đợi sinh viên trượt mới xử lý) sang "can thiệp chủ động" (hỗ trợ ngay khi hệ thống cảnh báo sớm).

- Thách thức lớn trong thế giới thực: Các rào cản lớn nhất không nằm ở thuật toán mà nằm ở Chất lượng dữ liệu (Data quality) bị phân mảnh giữa các phòng ban, Rủi ro về quyền riêng tư dữ liệu sinh viên, và Sự thiếu hụt kỹ năng công nghệ của đội ngũ giáo vụ/giảng viên khi sử dụng công cụ cảnh báo.

## Limitations

- Tính chất tổng quan cấp cao: Vì là một bài Systematic Review tập trung vào bức tranh toàn cảnh mang tính quản lý giáo dục, bài báo không đi sâu vào chi tiết mã nguồn, cách cấu hình siêu tham số (hyperparameters tuning) cụ thể của từng thuật toán hoặc kiến trúc hệ thống phần mềm.

- Khoảng cách giữa dự đoán và can thiệp: Bài báo chứng minh được mô hình AI dự đoán rất tốt, nhưng chưa tổng hợp sâu được các minh chứng thực nghiệm về việc sau khi can thiệp dựa trên AI thì tỷ lệ sinh viên giữ lại trường tăng chính xác bao nhiêu phần trăm.

## Relevance to our topic

- Hỗ trợ viết phần Introduction và Background: Nhóm có thể trích dẫn bài báo năm 2025 này để khẳng định xu hướng tất yếu của việc áp dụng ML trong giáo dục đại học, đồng thời lấy số liệu từ bài báo để chứng minh Random Forest là thuật toán có độ tin cậy cao trong thực tế, làm cơ sở lựa chọn thuật toán cho hệ thống của nhóm.

- Xác thực Yêu cầu hệ thống từ thực tế (Real-world Requirement Validation): Những thách thức mà bài báo chỉ ra (dữ liệu phân mảnh, người dùng thiếu kỹ năng) chính là những manh mối đắt giá để nhóm đưa vào danh sách Yêu cầu hệ thống (System Requirements). Ví dụ: Hệ thống SEWS của nhóm phải có giao diện cực kỳ trực quan (Dashboard đơn giản) để giảng viên không thạo công nghệ vẫn dùng được, và hệ thống phải có tính năng hợp nhất dữ liệu từ nhiều nguồn để giải quyết bài toán dữ liệu phân mảnh.