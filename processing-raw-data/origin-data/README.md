<img width="275" height="80" alt="image" src="https://github.com/user-attachments/assets/2802e2ea-7d03-4b01-8269-8d20bf32d76d" /># Tổng quan dữ liệu đầu vào. 
Đây là bộ dữ liệu gồm thông tin của hơn 70.000 ứng viên của một công ty công nghệ với quy mô toàn cầu.
Tổng quan bộ dữ liệu gốc như sau:
| Chỉ tiêu     	| Giá trị|
|--------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Số bản ghi        	| 73.426 |
| Số trường dữ liệu     	| 15  |
| Được tuyển (Employed = 1)   	| 39.392    |
| Không được tuyển (Employed = 0)	| 34.070   |

### Đặc điểm dữ liệu
Các trường dữ liệu có thể được chia thành các nhóm thông tin gồm thông tin cá nhân, trình độ học vấn và tình trạng việc làm, kinh nghiệm lập trình, mức lương, kỹ năng máy tính, và biến mục tiêu Employed.

Trong đó, Employed là biến mục tiêu được sử dụng để phân biệt ứng viên đã được tuyển dụng và ứng viên chưa được tuyển dụng. Các trường YearsCode, YearsCodePro, PreviousSalary và ComputerSkills cung cấp các thông tin định lượng phục vụ quá trình phân tích; trong khi EdLevel, Gender, MainBranch và Employment cung cấp các chiều phân loại ứng viên.

## Hồ sơ chi tiết các ứng viên của công ty công nghệ: [stackoverflow_full.csv](https://github.com/EnbacMig21/HR_Analyst_IT_employee/blob/main/processing-raw-data/origin-data/stackoverflow_full.csv)
| Tên cột      	| Ý nghĩa | Type |
|--------------	|-------------------------------------------------------------------------------	|--------------	|
| ID        	| ID của ứng viên | Integer  |
| Age        	| Tuổi của ứng viên (<35 or >35) | String  |
| Accessibility | Có bị khiếm khuyết hay không ? | Boolean  |
| Edlevel        	| Trình độ học vấn | String  |
| Employment        	| Tình trạng việc làm tại thời điểm hiện tại | Boolean  |
| Gender        	| Giới tính của ứng viên | String  |



