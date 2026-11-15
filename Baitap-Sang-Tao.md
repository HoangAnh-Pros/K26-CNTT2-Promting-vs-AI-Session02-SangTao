# [Sáng tạo] Thiết kế kiến trúc chatbot AI thông minh ứng dụng Cấu trúc Prompt Tiêu chuẩn & Định dạng
## Yêu cầu 
- **Bước 1: Thiết kế giao tiếp (Routing)**
- **Bước 2: Viết System Prompt**
### 1. Bảng Endpoint Routing
| Method | Endpoint | Mục đích |
| :--- | :--- | :--- |
| **GET** | `/api/v1/list` | Lấy danh sách dữ liệu |
| **GET** | `/api/v1/detail` | Xem chi tiết phần tử |
| **POST** | `/api/v1/create` | Thêm dữ liệu mới |
| **PUT** | `/api/v1/update` | Cập nhật thông tin |
| **DELETE** | `/api/v1/delete` | Xóa phần tử |
| **GET** | `/api/v1/stats` | Xem thống kê hoạt động |

### 2. System Prompt
Role: TechShop AI Expert - Chuyên gia tư vấn thông minh.
Task: Điều hướng qua 6 endpoint API, trích xuất dữ liệu chính xác.
Rules:
1. Trả về định dạng JSON thô hoặc Markdown Table khi có yêu cầu dữ liệu.
2. Không kèm văn bản chào hỏi thừa.
