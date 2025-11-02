# MiniERP_PhuLocGreen
Hệ thống MiniERP (Excel-VBA-Python-SQL .NET) cho PhuLoc Green Environment JSC
---

## 📦 Phiên bản mới nhất: MiniERP_AllInOne_v1.0_2025-11-02

### ⚙️ Cấu trúc

### 🚀 Hướng dẫn chạy
1. Tải file **MiniERP_AllInOne_v1.0_2025-11-02.zip** về máy.  
2. Giải nén → chạy file `builders/ERP_App_Starter/build_app_v1.vbs`.  
3. File **ERP_App_Starter_v1.0.xlsm** sẽ tự tạo ra trong thư mục chính.  
4. Mở file `.xlsm` → **Enable Macro**.  
5. Dùng 3 nút chính trên Dashboard:
   - 🟢 **Quản lý Khách hàng** → mở form thật `frmDMKH`
   - ⚪ **Ẩn/Hiện Ribbon** → bật/tắt menu App Mode
   - 📂 **Mở file dữ liệu** → mở nhanh `data\ERP_Data.xlsx`
6. Form có nền xanh nhạt `#E8F5E9`, tiêu đề xanh lá `#008000`, kích thước 400×260, canh giữa màn hình.

---

### 🧩 Cấu trúc module VBA
- `modConst` → Khai báo hằng số, đường dẫn data  
- `modUtil` → ToggleRibbon, MsgInfo, Open_DataFile  
- `dalDMKH` → Đọc dữ liệu KH  
- `bllDMKH` → Xử lý thêm mới KH  
- `uiDMKH` → Hiển thị form `frmDMKH`  
- `modStartup` → Auto_Open khởi tạo hệ thống

---

**© 2025 Phu Lộc Green Environment JSC**  
Hệ thống MiniERP – Giải pháp quản lý nội bộ gọn nhẹ, thân thiện, tích hợp Excel-VBA-Python-SQL-.NET.
