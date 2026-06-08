# Paper 02 Summary

## Citation

Tên bài: Early Prediction of Student Dropout in Higher Education using Machine Learning Models
Tác giả: Or Goren, Liron Cohen, Amir Rubinstein
Năm: 2024
Nguồn: EDM 2024 Short Papers
DOI/Link: https://www.educationaldatamining.org/edm2024/proceedings/2024.EDM-short-papers.32/2024.EDM-short-papers.32.pdf

## Problem

- Bài báo giải quyết vấn đề dự đoán sớm nguy cơ bỏ học (dropout) của sinh viên ngay trong giai đoạn đầu của lộ trình học tập (thường là học kỳ đầu tiên hoặc năm đầu tiên). Nghiên cứu tập trung vào việc vượt qua rào cản về mặt thời gian: làm sao để chỉ với dữ liệu tĩnh ban đầu (như thông tin nhân khẩu học, điểm số đầu vào) và dữ liệu học tập sơ khởi, mô hình vẫn đạt độ chính xác cao nhằm giúp nhà trường can thiệp kịp thời trước khi quá muộn.

## Method

- Bài báo sử dụng phương pháp Thực nghiệm/Kỹ thuật (Experiment / Quantitative Methodology) đặc thù của ngành Khai thác dữ liệu giáo dục (EDM):
  - Áp dụng và so sánh nhiều thuật toán Học máy khác nhau (như Random Forest, XGBoost, Support Vector Machine (SVM), Logistic Regression, và K-Nearest Neighbors).

  - Quy trình xử lý bao gồm: Tiền xử lý dữ liệu (Data Preprocessing), Lựa chọn đặc trưng (Feature Selection) nhằm lọc ra các biến số có trọng số quyết định, Huấn luyện mô hình và Đánh giá hiệu năng dựa trên các chỉ số chuẩn như Accuracy, F1-Score, và AUC-ROC.

## Context

- Nghiên cứu được thực hiện trong bối cảnh giáo dục đại học (Higher Education) đối mặt với tỷ lệ hao hụt sinh viên lớn ở các năm đầu. Dữ liệu thực nghiệm được thu thập từ hệ thống quản lý thông tin sinh viên của một trường đại học, bao gồm các nhóm thuộc tính chính: Thông tin nhân khẩu học (Demographics), Hoàn cảnh kinh tế - xã hội (Socio-economic background), và Kết quả học tập học kỳ đầu (First-semester academic performance).

## Key Findings

- Hiệu năng của các mô hình cây quyết định: Các thuật toán dạng Ensemble Learning như Random Forest và XGBoost cho kết quả dự đoán vượt trội về cả độ chính xác (Accuracy) lẫn khả năng cân bằng giữa độ nhạy và độ đặc hiệu (F1-Score) so với các mô hình truyền thống như Logistic Regression.

- Thời điểm vàng để dự đoán: Bài báo chứng minh rằng việc kết hợp dữ liệu nền của sinh viên với kết quả kiểm tra/điểm số của học kỳ 1 là thời điểm tối ưu nhất để chạy mô hình, vừa đảm bảo tính "sớm" (Early) của cảnh báo, vừa cung cấp đủ lượng thông tin có nghĩa cho thuật toán học máy.

- Các đặc trưng quyết định (Key Features): Kết quả học tập giai đoạn đầu (GPA học kỳ 1, số tín chỉ tích lũy bị trượt) và mức độ tương tác ban đầu là những biến số có trọng số cao nhất (highest feature importance) quyết định khả năng rời đi hay ở lại của sinh viên, vượt trội hơn hẳn so với các yếu tố nhân khẩu học thuần túy.

## Limitations

- Tính phụ thuộc vào dữ liệu tĩnh: Vì tập trung vào dự đoán "sớm", mô hình phụ thuộc nhiều vào các dữ liệu cố định từ đầu, chưa tích hợp được các luồng dữ liệu động theo thời gian thực (real-time/behavioral data) như tần suất đăng nhập LMS, thời gian làm bài tập hay mức độ tương tác trên forum ở các tuần giữa kỳ.

- Khả năng tổng quát hóa (Generalizability): Nghiên cứu dựa trên tập dữ liệu của một trường đại học hoặc một bối cảnh giáo dục cụ thể, do đó các trọng số đặc trưng có thể bị thay đổi hoặc không còn chính xác khi áp dụng sang các cơ sở đào tạo có phương thức quản lý hoặc tệp sinh viên khác biệt.

- Thiếu giải thích cơ chế hộp đen: Bài báo tập trung nhiều vào việc tối ưu điểm số hiệu năng (performance metrics) hơn là việc giải thích tường tận tại sao mô hình lại đưa ra quyết định đó (XAI - Explainable AI).

## Relevance to our topic

- Xác định các Yêu cầu chức năng (Functional Requirements) về mặt dữ liệu: Nhóm có thể dựa vào danh mục các đặc trưng (features) mà bài báo này đã chứng minh hiệu quả để thiết kế cơ sở dữ liệu (Database Schema) cho hệ thống của mình. Nó chỉ ra rằng hệ thống cần phải có các cổng kết nối (APIs) để lấy được dữ liệu điểm số học kỳ 1 và lịch sử trượt môn từ phòng đào tạo.

- Định hình thuật toán xử lý: Cung cấp cơ sở lý thuyết để nhóm đưa thuật toán Random Forest hoặc XGBoost vào danh sách các Core Engine cần triển khai cho hệ thống AI của nhóm.

- Xác lập mốc thời gian lấy yêu cầu (RE Timeline): Giúp nhóm làm rõ yêu cầu về mặt thời gian của hệ thống: Hệ thống bắt buộc phải xử lý và đưa ra báo cáo cảnh báo muộn nhất là ngay sau khi có điểm học kỳ 1.
