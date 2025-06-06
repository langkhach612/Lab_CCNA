# Lab_CCNA

## Các kiến thức đã thực hành

Bài lab mô phỏng một hệ thông mạng doanh nghiệp được triển khai và cấu hình các nội dung sau:

---

### 1. Cấu hình VLAN với Router-on-a-Stick và VTP

- **Router-on-a-Stick**:
  - Cấu hình cổng trunk trên router để định tuyến giữa các VLAN.
  - Tạo các sub-interface trên router với `encapsulation dot1q`.
  - Gán IP cho từng sub-interface tương ứng với các VLAN.

- **VTP (VLAN Trunking Protocol)**:
  - Cấu hình VTP Server và VTP Client.
  - Quản lý tập trung VLAN trên toàn bộ hệ thống switch.
  - Kiểm tra hoạt động VTP qua việc đồng bộ VLAN giữa các switch.

---

### 2. Cấu hình Static Route và OSPF

- Cấu hình OSPF cho các Vùng mạng được chỉ định trong bài lab.
- Cấu hình Static route cho 2 vùng mạng lan thông qua tunnel0(sử dụng khi thiết lập VPN-GRE)
- Cấu hình default route cho các gói tin đi từ các mạng lan ra ngoài internet.
- kết hợp OSPF và static route bằng **default-infomation oringinate**.

---

### 3. Cấu hình HSRP (Hot Standby Router Protocol)

- Thiết lập **HSRP** giữa hai router trong vùng lan chứa các Server để đảm bảo tính sẵn sàng cao.
- Cấu hình địa chỉ IP ảo cho gateway mặc định.

---

### 4. Cấu hình VPN Tunnel bằng GRE (Generic Routing Encapsulation)

- Tạo interface `Tunnel0` trên hai router đầu cuối.
- Gán địa chỉ IP trong cùng một subnet cho Tunnel.
- Cấu hình tuyến định tuyến để chuyển dữ liệu qua tunnel.
- Mô phỏng môi trường Internet bằng router trung gian để kiểm tra kết nối GRE VPN.

---

### 5. Cấu hình DNS và DHCP

- Cấu hình, tạo các A Record cho các DNS Server.
- Thực hiện cấu hình DHCP Server trên các Router để thực hiện quá trình cấp IP động đến các máy trong các Vlan.

---

### 6. Cấu hình NAT Static và ACLs (Access Control Lists)

- **Static NAT**:
  - Ánh xạ địa chỉ IP riêng (Private IP) của các Server thành các IP công cộng (Public IP).
  - Kiểm tra khả năng truy cập từ bên ngoài vào bên trong mạng.

- **ACLs**:
  - Tạo danh sách điều khiển truy cập để lọc lưu lượng mạng.
  - Kết hợp ACL với NAT để kiểm soát lưu lượng phù hợp.
