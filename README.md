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

## Bài toán kinh tế 
### Định nghĩa Sự sai lệch tiêu chí tuyển dụng
Sai lệch tuyển dụng là hiện tượng người phỏng vấn hoặc người ra quyết định tuyển dụng bị chi phối bởi các yếu tố không liên quan trực tiếp đến năng lực thực tế của ứng viên, như: ngoại hình, giới tính, độ tuổi, trường đại học, giọng nói, xuất thân, hay thậm chí là “cảm giác hợp gu”. Thay vì dựa trên tiêu chí rõ ràng về kỹ năng, kinh nghiệm và tiềm năng đóng góp, quyết định lại bị dẫn dắt bởi định kiến vô thức. Hậu quả trực tiếp là: nhiều ứng viên tiềm năng bị loại đáng tiếc, trong khi một số ứng viên được chọn chưa chắc đã phù hợp nhất với công việc và văn hóa công ty. - [hiring bias](https://glints.com/vn/blog/hiring-bias-la-gi/)
### Ảnh Hưởng - Tại Sao Cần Hạn Chế Sai Lệch Tuyển Dụng?
2.1. Chi phí tài chính: “Tuyển sai – trả đắt”
Một trong những lý do rõ ràng nhất để hạn chế sai lệch tuyển dụng là chi phí. Tuyển sai người không chỉ tốn tiền cho quảng cáo, phỏng vấn, đào tạo, mà còn kéo theo hàng loạt chi phí ẩn.

Theo nhiều nghiên cứu, chi phí cho một quyết định tuyển dụng sai có thể lên tới 30–200% lương năm đầu của nhân sự đó, tùy cấp độ và độ phức tạp của vị trí (Talent Traction, 2025; Talen.to, 2026; Treegarden, 2026).

Khoản chi này bao gồm:

Chi phí tuyển dụng lại (đăng tin, agency, thời gian sàng lọc, phỏng vấn).

Chi phí đào tạo, onboarding cho người mới.

Chi phí cơ hội do vị trí trống hoặc do người mới làm việc kém hiệu quả.

Trợ cấp thôi việc, chi phí pháp lý (nếu có tranh chấp).

Mất doanh thu, mất khách hàng do sai sót trong công việc hoặc dịch vụ kém (Dice, 2022; RippleHire, 2024).

Khi sai lệch tuyển dụng khiến doanh nghiệp liên tục “chọn nhầm người”, chi phí này sẽ lặp đi lặp lại, ăn mòn lợi nhuận và làm giảm khả năng cạnh tranh.

2.2. Năng suất và hiệu quả làm việc bị suy giảm
Một nhân sự không phù hợp sẽ khó đạt được kỳ vọng về hiệu suất. Họ có thể:

Làm việc chậm, sai sót nhiều, cần người khác hỗ trợ liên tục.

Không hòa nhập được với quy trình, công cụ, hoặc cách làm việc của team.

Không đáp ứng được áp lực công việc, dẫn đến chậm deadline, chất lượng đầu ra thấp.

Điều này không chỉ ảnh hưởng đến cá nhân đó, mà còn kéo cả nhóm đi xuống: những người giỏi phải gánh thêm việc, bị quá tải, dần dần mất động lực (Studocu, 2025; ViecTotNguoiTot, 2025; RippleHire, 2024).

Về dài hạn, năng suất trung bình của cả phòng ban giảm, mục tiêu KPI/OKR khó đạt, và doanh nghiệp mất đi lợi thế về tốc độ và chất lượng so với đối thủ.

2.3. Tác động đến văn hóa và tinh thần nhân viên
Sai lệch tuyển dụng không chỉ tạo ra “người sai”, mà còn gửi đi một tín hiệu văn hóa rất mạnh trong nội bộ.

Khi nhân viên thấy rằng:

Quyết định tuyển dụng dường như dựa trên “quen biết”, “cùng trường”, “cùng gu” hơn là năng lực.

Một số nhóm người (theo giới tính, độ tuổi, vùng miền…) luôn bị thiệt thòi trong cơ hội.

Họ sẽ dần mất niềm tin vào tính công bằng của tổ chức. Cảm giác “chơi không fair” này làm giảm engagement, tăng bất mãn và khiến người giỏi dễ tìm cơ hội khác (Studocu, 2025; VietnamWorks, 2024; Talemy, 2025).

Ngược lại, khi doanh nghiệp chủ động hạn chế sai lệch, xây dựng quy trình tuyển dụng minh bạch, dựa trên năng lực, nhân viên sẽ cảm thấy được tôn trọng, từ đó gắn bó và cống hiến nhiều hơn.

2.4. Bỏ lỡ nhân tài và giảm tính đa dạng
Một hệ quả “thầm lặng” nhưng rất nguy hiểm của sai lệch tuyển dụng là bỏ lỡ nhân tài.

Khi nhà tuyển dụng vô thức ưu tiên những ứng viên “giống mình” hoặc符合 định kiến (ví dụ: chỉ tin tưởng ứng viên từ một số trường, một số công ty cũ, một độ tuổi nhất định), họ dễ bỏ qua những người thực sự có năng lực nhưng khác biệt về nền tảng, phong cách, hoặc con đường sự nghiệp (HBR Việt Nam, 2026; HBR Việt Nam, 2025; VietnamWorks, 2024).

Điều này dẫn đến:

Đội ngũ thiếu đa dạng về tư duy, kinh nghiệm, góc nhìn.

Khả năng sáng tạo và giải quyết vấn đề bị hạn chế.

Tổ chức khó thích ứng với thị trường đa dạng và khách hàng ngày càng phức tạp.

Nhiều nghiên cứu chỉ ra rằng, các đội ngũ đa dạng thường có hiệu quả ra quyết định tốt hơn, sáng tạo hơn và đạt kết quả kinh doanh cao hơn. Theo Gartner, sự khác biệt về tuổi tác, dân tộc, giới tính và các khía cạnh khác thúc đẩy hiệu suất cao, với mức chênh lệch 12% giữa tổ chức đa dạng và không đa dạng (ECI Solutions, 2025; IJRPR, 2025). Do đó, hạn chế sai lệch tuyển dụng chính là cách để mở rộng “sân chơi” cho nhân tài, thay vì thu hẹp lại trong một “vòng an toàn” hẹp.

2.5. Rủi ro pháp lý và tổn hại danh tiếng
Ở nhiều quốc gia, phân biệt đối xử trong tuyển dụng (theo giới tính, tuổi tác, dân tộc, tôn giáo, tình trạng sức khỏe…) không chỉ là vấn đề đạo đức, mà còn vi phạm pháp luật (Studocu, 2025).

Nếu một ứng viên cho rằng họ bị đối xử bất công trong quá trình tuyển dụng, họ có thể:

Khiếu nại nội bộ.

Tố cáo lên cơ quan chức năng.

Khởi kiện doanh nghiệp.

Những vụ việc như vậy không chỉ gây tốn kém về pháp lý, mà còn tổn hại nghiêm trọng đến danh tiếng của công ty. Trong thời đại mạng xã hội, một câu chuyện “tuyển dụng thiên vị”, “phân biệt đối xử” có thể lan nhanh, tạo hình ảnh tiêu cực trong mắt ứng viên, khách hàng và đối tác (Glints, 2024; ViecTotNguoiTot, 2025).

Ngược lại, những doanh nghiệp được biết đến với quy trình tuyển dụng công bằng, minh bạch sẽ dễ thu hút nhân tài, xây dựng thương hiệu nhà tuyển dụng mạnh và tạo lòng tin trên thị trường.

2.6. Ảnh hưởng đến chiến lược dài hạn của doanh nghiệp
Tuyển dụng không chỉ là giải quyết nhu cầu “trước mắt”, mà còn là xây đội ngũ cho tương lai. Mỗi quyết định tuyển dụng sai sẽ tạo ra một “mắt xích yếu” trong chuỗi giá trị của tổ chức.

Khi sai lệch tuyển dụng trở thành “thói quen”:

Cơ cấu nhân sự dần lệch lạc: thiếu người giỏi thực sự, thừa người “vừa đủ” hoặc “không phù hợp”.

Leadership pipeline bị ảnh hưởng: những người được thăng tiến có thể không phải là người xuất sắc nhất, mà là người “được ưu ái”.

Chiến lược kinh doanh dài hạn khó thực hiện vì thiếu nhân sự chủ chốt đủ năng lực (HBR Việt Nam, 2026; RippleHire, 2024).

Ngược lại, khi doanh nghiệp kiên quyết hạn chế sai lệch, xây dựng quy trình tuyển dụng dựa trên dữ liệu và tiêu chí rõ ràng, họ đang đầu tư vào chất lượng đội ngũ – yếu tố then chốt để thực hiện chiến lược và duy trì lợi thế cạnh tranh.
### Mục đích phân tích 

