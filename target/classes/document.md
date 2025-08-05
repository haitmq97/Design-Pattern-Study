1. Các Design Patterns phổ biến trong Java EE
a. MVC (Model-View-Controller)
Model: Xử lý logic dữ liệu (JavaBeans, Entities).
View: Giao diện người dùng (JSP, JSF, HTML).
Controller: Quản lý luồng dữ liệu giữa Model và View (Servlet, Managed Beans).
b. DAO (Data Access Object)
Tách rời logic truy xuất dữ liệu ra khỏi business logic.
Các DAO class thực hiện truy vấn, thao tác với cơ sở dữ liệu.
c. Singleton
Đảm bảo chỉ có một instance của một class tồn tại (ví dụ: Connection Pool).
d. Factory & Abstract Factory
Tạo ra các object mà không cần chỉ rõ class cụ thể.
Được dùng nhiều trong việc khởi tạo các service hoặc component.
e. Front Controller
Một điểm đầu mối nhận tất cả các request (Servlet chính hoặc Filter) và phân phối cho các xử lý khác.
f. Service Locator
Quản lý việc tìm kiếm và truy xuất các service (JNDI, EJB, DataSource).
g. Dependency Injection (DI)
Inject các dependency vào component (ví dụ: sử dụng CDI, EJB, Spring framework).
2. Java EE Architecture
a. Multi-Tier Architecture (Kiến trúc nhiều lớp)
Thông thường, ứng dụng Java EE được chia thành các lớp chính:

Client Tier: Giao diện người dùng (Web Browser, Mobile App)
Web Tier: Xử lý request của client (Servlet, JSP, JSF)
Business Tier: Xử lý logic nghiệp vụ (EJB, Beans)
Integration Tier: Tương tác với hệ thống phụ trợ (Web Service, JMS)
Data Tier: Lưu trữ dữ liệu (Database, File System)
b. Component-based Architecture
Java EE gồm nhiều thành phần, như Servlets, JSP, JSF, EJB, JPA, JMS, v.v.
Mỗi thành phần thực hiện một vai trò riêng biệt.
c. Layered Architecture
Chia ứng dụng thành các lớp (presentation, business, persistence) để dễ quản lý và bảo trì.
3. Ví dụ về ứng dụng Design Patterns trong Java EE
Ví dụ: Khi xây dựng một hệ thống quản lý thư viện, bạn có thể:

Dùng MVC để tách biệt giao diện, logic và dữ liệu.
Dùng DAO để truy xuất thông tin sách từ database.
Dùng Singleton cho Connection Pool.
Dùng Dependency Injection để inject các service vào controller.
4. Tài liệu tham khảo
Java EE Patterns
Jakarta EE Documentation
Sách: "Core J2EE Patterns" (Deepak Alur, John Crupi, Dan Malks)