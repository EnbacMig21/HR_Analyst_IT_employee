# Phân tích tình hình nhân sự tuyển dụng
Sử dụng bộ dữ liệu về tình hình nhân sự tuyển dụng tại công ty để tiến hành phân tích. Dưới đây là quy trình phân tích, truy cập bằng cách bấm vào tiêu đề của quy trình:

1. [Hiểu bài toán kinh tế](##Bài-toán-kinh-tế)
2. [Thu thập dữ liệu và xử lý dữ liệu]()
3. [Phân tích dữ liệu]()
   - Khám phá dữ liệu
   - Tiến hành phân tích và đánh giá các xu hướng
4. [Kể chuyện qua dữ liệu và đề xuất hành động]()
   - Insight 1
   - Insight 2
   - Insight 3

Trong file README.md này sẽ giải thích thứ tự đọc file, mục đích phân tích và trong các file đó có gì. Bên dưới đây sẽ là tổng quan, bối cảnh của bài phân tích từ đó giúp người đọc hiểu rõ về đề tài này.

## Danh mục nội dung 
- [Bài toán kinh tế]()
- [Mục đích phân tích]()
- [Giải thích file]()
- [Lời kết]()

### Bài toán kinh tế 
"Sự sai lệch tiêu chí tuyển dụng" để chỉ việc từ chối hoặc chọn lựa sai ứng viên (trong thời gian dài) khỏi quy trình tuyển dụng do tiêu chí đánh giá không phù hợp, thời gian xem xét sai lầm, hoặc định giá sai ứng viên. Lỗi này dẫn đến thiệt hại kinh tế đáng kể cho doanh nghiệp.
#### Ảnh Hưởng - Tại Sao Cần Hạn Chế Sai Lệch Tuyển Dụng?
Sai lệch trong tuyển dụng có thể khiến những ứng viên có năng lực không được đánh giá công bằng, làm giảm cơ hội tiếp cận việc làm của một số nhóm ứng viên. Các nghiên cứu thực nghiệm cho thấy tình trạng phân biệt đối xử trong tuyển dụng vẫn tồn tại ở nhiều nhóm đối tượng. Meta-analysis của Lippens, Vermeiren và Baert (2023) trên European Economic Review tổng hợp các nghiên cứu về phân biệt đối xử trong tuyển dụng và cho thấy sự bất lợi vẫn xuất hiện đối với nhiều nhóm ứng viên, trong đó có người lớn tuổi, người khuyết tật và các nhóm có đặc điểm chủng tộc hoặc dân tộc nổi bật. Nghiên cứu cũng không tìm thấy bằng chứng về sự thay đổi theo thời gian một cách có hệ thống sau khi xem xét các yếu tố liên quan.

Tại Mỹ, nghiên cứu của Quillian và cộng sự (2017) cho thấy từ năm 1989, ứng viên da trắng nhận được trung bình nhiều hơn 36% lời mời phản hồi (callback) so với ứng viên người Mỹ da đen có hồ sơ tương đương. Nghiên cứu cũng không ghi nhận sự suy giảm đáng kể trong mức độ phân biệt đối xử đối với ứng viên người Mỹ da đen trong khoảng thời gian được nghiên cứu.

Những kết quả trên cho thấy việc xây dựng các tiêu chí tuyển dụng phù hợp và đánh giá ứng viên dựa trên những yếu tố liên quan đến năng lực là cần thiết nhằm hạn chế sai lệch trong quá trình tuyển dụng. Đây cũng là cơ sở để sử dụng dữ liệu nhằm xem xét các yếu tố liên quan đến khả năng được tuyển dụng và hỗ trợ quá trình ra quyết định nhân sự.

### Mục đích phân tích 

