<!-- ===================== HEADER ===================== -->
<p align="center">
  <img src="https://github.com/phucpsaigon-dev/MiniERP_PhuLocGreen/assets/your_logo_image_here" width="180" alt="PhuLocGreen Logo">
</p>

<h1 align="center">🌿 MiniERP – Phu Lộc Green Environment JSC</h1>

<p align="center">
  <strong>Giải pháp ERP mini – Quản lý nội bộ gọn nhẹ, thân thiện, linh hoạt.</strong><br>
  <em>Excel - VBA - Python - SQL - .NET Integration</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-v1.0-green?style=flat-square" alt="version"/>
  <img src="https://img.shields.io/badge/platform-Excel%2064bit-blue?style=flat-square" alt="platform"/>
  <img src="https://img.shields.io/badge/status-stable-success?style=flat-square" alt="status"/>
  <img src="https://img.shields.io/badge/license-Proprietary-orange?style=flat-square" alt="license"/>
</p>

---

## 🚀 Giới thiệu

**MiniERP_PhuLocGreen** là nền tảng ERP gọn nhẹ được thiết kế riêng cho **Phu Lộc Green Environment JSC**, phục vụ quản lý khách hàng, nhà cung cấp, nhân viên, hàng hoá và dữ liệu nghiệp vụ — **70% Excel + VBA**, **30% Python/SQL/.NET backend**.

Mục tiêu:
- Tối ưu cho doanh nghiệp nhỏ & vừa.  
- Giao diện Excel thân thuộc, không cần cài thêm phần mềm.  
- Dễ mở rộng sang WebApp hoặc VB.NET/SQL Server khi cần.  

---

## 📦 Phiên bản mới nhất: `MiniERP_AllInOne_v1.0_2025-11-02`

> 🔗 **Tải về:** [MiniERP_AllInOne_v1.0_2025-11-02.zip](https://github.com/phucpsaigon-dev/MiniERP_PhuLocGreen/raw/main/MiniERP_AllInOne_v1.0_2025-11-02.zip)

### ⚙️ Cấu trúc thư mục
MiniERP_AllInOne_v1.0_2025-11-02/
├─ ERP_App_Starter_v1.0.xlsm ← Form thật + Dashboard + VBA hoàn chỉnh
├─ data/
│ └─ ERP_Data.xlsx ← tblDMKH + __CFG
└─ README_AllInOne.txt

---

## 🧩 Tính năng nổi bật

| Nhóm | Mô tả |
|------|-------|
| 🧠 **VBA Layer (UI/BLL/DAL)** | Cấu trúc 3 lớp: UI (Form) – BLL (Logic) – DAL (Data) |
| 🪟 **Dashboard thân thiện** | Nút “Quản lý Khách hàng”, “Ẩn/Hiện Ribbon”, “Mở file dữ liệu” |
| 🧾 **Form nhập liệu DMKH thật** | `frmDMKH` có nền xanh nhạt `#E8F5E9`, tiêu đề xanh lá `#008000`, canh giữa màn hình |
| 💾 **Tự động sinh mã KHxxxx** | Lưu trực tiếp xuống `data\tblDMKH` |
| 🎨 **Giao diện App Mode** | Tắt gridlines, font Segoe UI, màu thương hiệu Phu Lộc Green |
| ⚙️ **Module mở rộng** | Có sẵn `ToggleRibbon()` và `Open_DataFile()` |

---

## 🧱 Cấu trúc module VBA

| Module | Mục đích |
|---------|----------|
| **modConst** | Khai báo hằng số, đường dẫn data |
| **modUtil** | Hàm tiện ích, ToggleRibbon, MsgInfo, Open_DataFile |
| **dalDMKH** | Data Access Layer – đọc danh mục khách hàng |
| **bllDMKH** | Business Logic Layer – xử lý thêm mới KH |
| **uiDMKH** | Giao diện – hiển thị form `frmDMKH` |
| **modStartup** | Auto_Open khởi tạo hệ thống |

---

## 🖼️ Minh hoạ giao diện

<p align="center">
  <img src="https://github.com/phucpsaigon-dev/MiniERP_PhuLocGreen/assets/your_dashboard_screenshot_here" width="800" alt="Dashboard Screenshot"/>
</p>

<p align="center"><em>Dashboard – nền trắng sạch, theme xanh lá, Segoe UI 11pt</em></p>

<p align="center">
  <img src="https://github.com/phucpsaigon-dev/MiniERP_PhuLocGreen/assets/your_form_screenshot_here" width="450" alt="frmDMKH Form"/>
</p>

<p align="center"><em>Form “QUẢN LÝ KHÁCH HÀNG (DMKH)” – nền #E8F5E9, tiêu đề xanh lá, nút Lưu/Đóng thân thiện</em></p>

---

## ⚙️ Hướng dẫn cài đặt & chạy

1️⃣ **Tải về & giải nén:**  
   Tải gói `MiniERP_AllInOne_v1.0_2025-11-02.zip` và giải nén vào ổ đĩa cục bộ.  

2️⃣ **Chạy script builder:**  
   Mở file `builders/ERP_App_Starter/build_app_v1.vbs`  
   → script sẽ tự tạo `ERP_App_Starter_v1.0.xlsm`.

3️⃣ **Mở Excel:**  
   Mở file `.xlsm` → chọn **Enable Content** để kích hoạt macro.

4️⃣ **Thao tác chính:**  
   - 🟢 `Quản lý Khách hàng` → mở form nhập KH thật  
   - ⚪ `Ẩn/Hiện Ribbon` → chuyển chế độ App view  
   - 📂 `Mở file dữ liệu` → truy cập nhanh `data\ERP_Data.xlsx`

5️⃣ **Yêu cầu quyền truy cập VBA Project:**  
   Trong Excel → Options → Trust Center → Macro Settings → tick  
   **"Trust access to the VBA project object model"**

---

## 🧰 Công nghệ & Ngôn ngữ

- **Microsoft Excel 2016/2021 (64-bit)**  
- **VBA 7.1**  
- **Python (xlwings, pandas)** – dự kiến mở rộng  
- **SQL Server / SQLite** – backend data layer  
- **VB.NET / .NET 8 LTS** – app extension  

---

## 📈 Lộ trình phát triển

| Phiên bản | Trạng thái | Tính năng chính |
|------------|-------------|----------------|
| **v1.0** | ✅ Hoàn thành | Dashboard + frmDMKH thật |
| **v1.1** | 🔄 Dự kiến | Thêm `frmDMNCC` (Nhà cung cấp) |
| **v2.0** | 🧱 Đang thiết kế | Tích hợp Python & SQL realtime |
| **v3.0** | 🧩 Dài hạn | VB.NET desktop app + WebAPI |

---

## 🧾 Giấy phép
> **© 2025 Phu Lộc Green Environment JSC**  
> Mọi quyền được bảo lưu.  
> Phiên bản này dùng cho nội bộ hoặc huấn luyện nhân viên kỹ thuật.

---

## 🌐 Liên hệ
**Phu Lộc Green Environment JSC**  
📍 Website: [www.phulocgreen.com](https://www.phulocgreen.com)  
📧 Email: dunglocphat@gmail.com  
📞 Hotline: 0913 131 961  
📦 GitHub: [phucpsaigon-dev](https://github.com/phucpsaigon-dev)

---

<p align="center">
  <em>MiniERP – Tinh gọn mà mạnh mẽ 🌱<br>
  Excel là nền tảng, VBA là linh hồn, Python/SQL là tương lai.</em>
</p>
