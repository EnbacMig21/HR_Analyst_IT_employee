# Tổng quan dữ liệu đầu vào. 
Đây là bộ dữ liệu gồm thông tin của hơn 70.000 ứng viên của một công ty công nghệ với quy mô toàn cầu.
Tổng quan bộ dữ liệu gốc như sau:
| Chỉ tiêu     	| Giá trị|
|--------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Bản ghi        	| 73.426 |
| Số cột     	| 15  |
| Được tuyển (Employed = 1)   	| 39.392    |
| Không được tuyển (Employed = 0)	| 34.070   |

### Đặc điểm dữ liệu
Các trường dữ liệu có thể được chia thành các nhóm thông tin gồm thông tin cá nhân, trình độ học vấn và tình trạng việc làm, kinh nghiệm lập trình, mức lương, kỹ năng máy tính, và biến mục tiêu Employed.

Trong đó, Employed là biến mục tiêu được sử dụng để phân biệt ứng viên đã được tuyển dụng và ứng viên chưa được tuyển dụng. Các trường YearsCode, YearsCodePro, PreviousSalary và ComputerSkills cung cấp các thông tin định lượng phục vụ quá trình phân tích; trong khi EdLevel, Gender, MainBranch và Employment cung cấp các chiều phân loại ứng viên.

## Hồ sơ chi tiết các ứng viên của công ty công nghệ: [stackoverflow_full.csv](https://github.com/EnbacMig21/HR_Analyst_IT_employee/blob/main/processing-raw-data/origin-data/stackoverflow_full.csv)
| Tên cột      	| Ý nghĩa|
|--------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Player        	| Tên của các cầu thủ |
| Short pass back     	| Chuyền ngắn về phía sau  |
| Short pass forward   	| Chuyền ngắn lên phía trước    |
| Short pass wide	| Chuyền ngắn ra biên   |
| Long pass back	| Chuyền dài về phía sau |
| Long pass forward	| Chuyền dài lên phía trước  |
| Long pass wide	| Chuyền dài ra biên  | 
| Cross	 | Tạt bóng  |
| Heading	 | Đánh đầu  |
| Finishing	 | Dứt điểm   | 
| Long shot	 | Sút xa |
| Dribbles	 | Rê dắt bóng, qua người  | 
|  Reception	| Khống chế bóng bước một  |
| Interceptions	 | Cắt bóng |
| Goalkeeping	 | Cản phá bóng(GK)  |
| Goal kick	 | Phát bóng dài (GK)  |
| Set pieces	| Tình huống cố định   |
| Short pass	 | Chuyền ngắn (Tổng quát)  |
| Long Passes	 | Chuyền dài(Tổng quát)  |
| Pressing	    | Áp sát, gây áp lực |
