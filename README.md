# Lab_CCNA

## Các kiến thức đã thực hành

Trong quá trình thực hành bài lab CCNA, tôi đã triển khai và cấu hình các nội dung sau:

---

### 1. Cấu hình VLAN với Router-on-a-Stick và VTP

- **Router-on-a-Stick**:
  - Sử dụng một cổng trunk trên router để định tuyến giữa các VLAN.
  - Tạo các sub-interface trên router với `encapsulation dot1q`.
  - Gán IP cho từng sub-interface tương ứng với các VLAN.

- **VTP (VLAN Trunking Protocol)**:
  - Cấu hình VTP Server và VTP Client.
  - Quản lý tập trung VLAN trên toàn bộ hệ thống switch.
  - Kiểm tra hoạt động VTP qua việc đồng bộ VLAN giữa các switch.

---

### 2. Cấu hình Static Route và OSPF

- **Static Routing**:
  - Thiết lập tuyến tĩnh giữa các mạng không cùng router.
  - Sử dụng lệnh `ip route` để định tuyến thủ công.

- **OSPF (Open Shortest Path First)**:
  - Cấu hình OSPF liên vùng giữa các router.
  - Sử dụng `router ospf` và các `network` để quảng bá mạng.
  - Kiểm tra quan hệ láng giềng (neighbor) và bảng định tuyến OSPF.

---

### 3. Cấu hình HSRP (Hot Standby Router Protocol)

- Thiết lập **HSRP** giữa hai router để đảm bảo tính sẵn sàng cao.
- Cấu hình địa chỉ IP ảo cho gateway mặc định.
- Thử nghiệm failover: tắt router chính để kiểm tra chuyển đổi sang router dự phòng.

---

### 4. Cấu hình VPN Tunnel bằng GRE (Generic Routing Encapsulation)

- Tạo interface `Tunnel0` trên hai router đầu cuối.
- Gán địa chỉ IP trong cùng một subnet cho Tunnel.
- Cấu hình tuyến định tuyến để chuyển dữ liệu qua tunnel.
- Mô phỏng môi trường Internet bằng router trung gian để kiểm tra kết nối GRE VPN.

---

### 5. Cấu hình NAT Static và ACLs (Access Control Lists)

- **Static NAT**:
  - Ánh xạ địa chỉ IP riêng (Private IP) với IP công cộng (Public IP).
  - Kiểm tra khả năng truy cập từ bên ngoài vào bên trong mạng.

- **ACLs**:
  - Tạo danh sách điều khiển truy cập để lọc lưu lượng mạng.
  - Ứng dụng vào việc bảo mật, giới hạn truy cập giữa các mạng hoặc dịch vụ cụ thể.
  - Kết hợp ACL với NAT để kiểm soát lưu lượng phù hợp.
