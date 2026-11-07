# 📊 โครงร่างสไลด์นำเสนอโครงงาน: Job Application Tracker (9 สไลด์)

เอกสารสรุปเนื้อหาและแนวทางการจัดวางองค์ประกอบบนสไลด์ Presentation สำหรับนำเสนออาจารย์และคณะกรรมการ

---

## สไลด์ที่ 1: ข้อมูลโครงงานและสมาชิก (Project Title & Team)

* **ชื่อโครงงานภาษาไทย:** ระบบติดตามและวิเคราะห์สถานะการสมัครงานและฝึกงานอัจฉริยะ (Job Application Tracker)
* **ชื่อโครงงานภาษาอังกฤษ:** Smart Job & Internship Application Tracker with Analytics Dashboard
* **ชื่อย่อ / รหัสโครงงาน:** JobTracker Desktop GUI
* **ข้อมูลสมาชิกในกลุ่ม:**
  * **[ใส่รูปถ่ายสมาชิก 1]** : ชื่อ-นามสกุล | รหัสนักศึกษา | บทบาท: Project Manager & System Architect
  * **[ใส่รูปถ่ายสมาชิก 2]** : ชื่อ-นามสกุล | รหัสนักศึกษา | บทบาท: Core Logic & Database Developer
  * **[ใส่รูปถ่ายสมาชิก 3]** : ชื่อ-นามสกุล | รหัสนักศึกษา | บทบาท: UI/UX & Data Visualization Developer
  * **[ใส่รูปถ่ายสมาชิก 4]** : ชื่อ-นามสกุล | รหัสนักศึกษา | บทบาท: Software QA, Testing & Documentation
* **ข้อมูลรายวิชาและสถาบัน:** ภาควิชา/สาขาวิชา, คณะ, สถาบันการศึกษา และชื่ออาจารย์ที่ปรึกษาประจำวิชา

> **🖼️ คำแนะนำภาพประกอบ:** วาง Logo โครงงานกึ่งกลางด้านบน จัดบล็อกข้อมูลสมาชิกเป็น 2–4 คอลัมน์สมมาตร โดยใช้กรอบรูปถ่ายหน้าตรงแบบทางการตัดมุมมน

---

## สไลด์ที่ 2: ความเป็นมาของโครงงาน (Background & Problem Statement)

* **ปัญหาการจัดการข้อมูลกระจัดกระจาย (Data Fragmentation):** นิสิต/นักศึกษาและผู้หางานสมัครหลายตำแหน่งผ่านหลากช่องทาง (LinkedIn, เว็บบริษัท, อีเมล, Job Portals) ทำให้ไม่มีศูนย์กลางบันทึกข้อมูล
* **ปัญหาการพลาดการติดตามผล (Lack of Follow-up Tracking):** ไม่ทราบระยะเวลาที่รอผลหลังยื่นใบสมัคร ส่งผลให้พลาดช่วงเวลาเหมาะสมในการสอบถาม (Follow-up) หรือแก้ปัญหาเมื่อบริษัทปฏิเสธโดยไม่แจ้ง
* **ข้อจำกัดของ Spreadsheets ทั่วไป (Spreadsheet Inefficiency):** การจดบันทึกลง Excel หรือสมุดโน้ตไม่มีระบบคำนวณวันรอผลอัตโนมัติ ขาดการแจ้งเตือนเคสเร่งด่วน และไม่มี Dashboard วิเคราะห์อัตราความสำเร็จ (Success Rate)

> **🖼️ คำแนะนำภาพประกอบ:** ภาพกราฟิกเปรียบเทียบ "Before & After" (ด้านซ้าย: ภาพไอคอนกระดาษจดโน้ต/ตาราง Excel ยุ่งเหยิงและเครื่องหมายกากบาทสีแดง, ด้านขวา: หน้าโปรแกรม Dashboard ที่เป็นระเบียบพร้อมเครื่องหมายถูกสีเขียว)
> 
> * **ไฟล์ภาพกราฟิกพร้อมใช้งาน:** `before_after_comparison.png` (และ `before_after_comparison.jpg`) บันทึกอยู่ในโฟลเดอร์โปรเจกต์ นำไปวางบนหน้าสไลด์ได้ทันที

---

## สไลด์ที่ 3: วัตถุประสงค์ของโครงงาน (Objectives)

* **พัฒนาระบบศูนย์กลางบันทึกข้อมูล (Centralized CRUD System):** เพื่อบันทึก ค้นหา แก้ไข และจัดหมวดหมู่ประวัติการสมัครงานได้อย่างเป็นระบบและปลอดภัยในเครื่องผู้ใช้
* **สร้างระบบแจ้งเตือนระยะเวลารอผลอัจฉริยะ (Automated Follow-up Alert):** เพื่อคำนวณจำนวนวันจากวันที่สมัครถึงวันปัจจุบัน พร้อมจัดกลุ่มระดับความเร่งด่วน (> 14 วัน และ > 30 วัน) อัตโนมัติ
* **ออกแบบแผงควบคุมและแสดงสถิติเชิงภาพ (Visualized Analytics Dashboard):** เพื่อสรุปสถิติสำคัญ (KPIs) อัตราตอบรับ และแสดงผลแผนภูมิสัดส่วนสถานะและช่องทางการสมัคร
* **ส่งเสริมการพกพาและใช้งานง่าย (Zero-Dependency Standalone Architecture):** เพื่อให้โปรแกรมทำงานได้ทันทีแบบ Standalone โดยไม่ต้องติดตั้งแพ็กเกจภายนอกเพิ่มเติม

> **🖼️ คำแนะนำภาพประกอบ:** แผนผังไอคอนเป้าหมาย 4 เสาหลัก (1. Centralized DB, 2. Smart Alert Engine, 3. Visual Dashboard, 4. 100% Native & Portable)
> 
> * **ไฟล์ภาพกราฟิกพร้อมใช้งาน:** `pillars_infographic.png` (และ `pillars_infographic.jpg`) บันทึกอยู่ในโฟลเดอร์โปรเจกต์ นำไปวางบนหน้าสไลด์ได้ทันที

---

## สไลด์ที่ 4: ขีดความสามารถและตัวอย่างผลงานจริง (Key Capabilities & Demo Preview)

* **ระบบจัดการข้อมูลครบวงจร (Full CRUD & Direct Link):** บันทึกสถานะ 5 ระดับ, ค้นหา/กรองข้อมูลเรียลไทม์, แก้ไขผ่าน Dialog และคลิกเปิดลิงก์ประกาศงานผ่านเบราว์เซอร์ได้ทันที
* **ระบบติดตามผลด่วน (Urgent Follow-up Hub):** ตรวจจับเคสรอนานเกิน 14 วัน (เตือนติดตาม) และเกิน 30 วัน (วิกฤต) พร้อมปุ่ม Quick Actions เช่น "ส่งใบสมัครซ้ำ/Follow-up" และ "อัปเดตสถานะสัมภาษณ์" ในคลิกเดียว
* **แผงวิเคราะห์สถิติและการส่งออก (Visual Analytics & CSV Export):** แสดงตัวชี้วัด (Total, Pending, Interview, Offer, Rejected, Success Rate %), กราฟ Donut Chart, กราฟแท่งจำแนกตามช่องทาง และส่งออกไฟล์ CSV ภาษาไทยมาตรฐาน (`utf-8-sig`)
* **ระบบจำลองข้อมูลสาธิต (One-Click Demo Seeder):** ปุ่มเติมชุดข้อมูลตัวอย่าง 7 บริษัทชั้นนำ เพื่อพร้อมนำเสนอและทดสอบการทำงานของระบบได้ทันที

> **🖼️ คำแนะนำภาพประกอบ:** แคปเจอร์หน้าจอจริง 3 ส่วนนำมาประกบกัน:
> 1. หน้าต่าง **แดชบอร์ดสรุป** (โชว์การ์ดตัวเลขและ Donut Chart)
> 2. หน้าต่าง **ติดตามผลด่วน** (โชว์การ์ดสีส้ม/แดงเตือนเคสเกินกำหนด)
> 3. หน้าต่าง **รายการทั้งหมด** (โชว์ตารางข้อมูล Treeview พร้อมแถบสีสถานะ)

---

## สไลด์ที่ 5: โมเดลการพัฒนาซอฟต์แวร์และการแบ่งหน้าที่ (Software Development Model & Roles)

* **โมเดลการพัฒนาที่เลือกใช้:** **Iterative & Incremental Prototyping (แบบวนรอบพัฒนาต้นแบบ)**
  * *เหตุผล:* ช่วยให้สามารถสร้าง UI ต้นแบบและ Core Function ออกมาทดสอบการใช้งานจริงได้อย่างรวดเร็ว จากนั้นจึงปรับปรุงระบบแจ้งเตือนและกราฟสถิติตาม Feedback
* **การจัดสรรบทบาทหน้าที่ของสมาชิก:**
  * **Sprint 1: วิเคราะห์และออกแบบ (Requirement & Architecture):** สำรวจ Pain Points ของผู้สมัครงาน ออกแบบ Database Schema และ Data Flow Diagram
  * **Sprint 2: พัฒนาฐานข้อมูลและตรรกะระบบ (Backend & Business Logic):** จัดทำโครงสร้าง SQLite CRUD, ฟังก์ชันคำนวณวันรอผล และระบบคัดกรองเคสเกินกำหนด
  * **Sprint 3: พัฒนาส่วนติดต่อผู้ใช้ (Frontend & Visualization):** พัฒนา Tkinter GUI, ระบบ High-DPI, GDI Font Injection และอัลกอริทึมวาด Canvas Charts
  * **Sprint 4: ทดสอบและประกันคุณภาพ (QA, Testing & Documentation):** ทดสอบ Edge Cases วันที่, ทดสอบการแสดงผลภาษาไทยบน Excel, จัดทำคู่มือและสไลด์

> **🖼️ คำแนะนำภาพประกอบ:** แผนผังวงจร Prototyping Cycle (Requirements ➔ Design ➔ Prototype ➔ Testing ➔ Review) พร้อมตารางสรุปหน้าที่ของสมาชิกตามบทบาท
> 
> * **ไฟล์ภาพกราฟิกพร้อมใช้งาน:** `prototyping_and_roles.png` (และ `prototyping_and_roles.jpg`) บันทึกอยู่ในโฟลเดอร์โปรเจกต์ นำไปวางบนหน้าสไลด์ได้ทันที

---

## สไลด์ที่ 6: โครงสร้างโครงงานในภาพรวม (System Architecture & Overview)

* **สถาปัตยกรรมระบบ (Layered Architecture):**
  * **Presentation Layer:** Tkinter Desktop GUI (Custom ttk Styles, Canvas Vector Graphics, Dialog Windows)
  * **Business Logic Layer:** Application Controller, Date Difference Engine, Dynamic Filtering, CSV Serialization
  * **Data Access Layer:** SQLite3 Embedded Engine, Parameterized Queries, Database Connection Factory
* **เทคโนโลยีและเครื่องมือที่ใช้ (Tech Stack):**
  * **ภาษาหลัก:** Python 3 (100% Python Standard Library ไม่ต้องลงแพ็กเกจเพิ่ม)
  * **ฐานข้อมูล:** SQLite3 (Local File Database: `job_tracker.db`)
  * **กราฟิก & ฟอนต์:** Windows GDI API (`AddFontResourceExW`), Windows DPI Awareness (`shcore.dll`), ฟอนต์ Prompt
  * **การส่งออกข้อมูล:** Python CSV Module พร้อมเข้ารหัส `utf-8-sig` สำหรับเปิดใน Microsoft Excel

> **🖼️ คำแนะนำภาพประกอบ:** ไดอะแกรม System Architecture 3 ชั้น (UI Layer ➔ Logic Layer ➔ Data Layer) พร้อมสัญลักษณ์ Data Flow แสดงการไหลของข้อมูลจากผู้ใช้ไปยังฐานข้อมูล SQLite

---

## สไลด์ที่ 7: อธิบายการทำงานของโค้ดในแต่ละส่วน (Code Overview)

* **โมดูลการตั้งค่าสภาพแวดล้อม (System & Environment Setup):**
  * จัดการ High-DPI ผ่าน `ctypes` เพื่อความคมชัดบนจอ 2K/4K
  * ฟังก์ชัน `register_local_fonts()` โหลดไฟล์ฟอนต์ `fonts/Prompt-*.ttf` เข้าสู่ Windows Memory โดยตรง
* **โมดูลจัดการฐานข้อมูล (Data Layer & CRUD Functions):**
  * ฟังก์ชัน `init_db()` ตรวจสอบและสร้างตาราง `applications`
  * รวมคำสั่ง `db_create()`, `db_read_all()`, `db_update()`, `db_delete()`, `db_update_status()`, `db_reapply_followup()` แบบ Parameterized SQL
* **โมดูลส่วนติดต่อผู้ใช้และแผนภูมิ (GUI & Canvas Engine):**
  * คลาส `JobTrackerApp(tk.Tk)` ควบคุม 4 แท็บหลักผ่าน `ttk.Notebook`
  * อัลกอริทึมวาดเวกเตอร์บน `tk.Canvas` สำหรับ `draw_donut_chart()` (คำนวณองศา Arcs) และ `draw_bar_chart()`
* **โมดูลการทำงานเสริม (Utility & Export):**
  * `export_to_csv()` ประมวลผลข้อมูลออกเป็นไฟล์ Spreadsheet
  * `webbrowser.open_new_tab()` สำหรับเชื่อมโยง URL ภายนอก

> **🖼️ คำแนะนำภาพประกอบ:** แผนผัง Tree Diagram แสดงโครงสร้างไฟล์ของโปรแกรม (`app.py`, `job_tracker.db`, โฟลเดอร์ `fonts/`, `run.bat`) ควบคู่กับบล็อกสรุปหน้าที่ของฟังก์ชันหลักใน `app.py`

---

## สไลด์ที่ 8: ปัญหาและแนวทางแก้ไข (Obstacles & Solutions)

* **ปัญหาที่ 1: การแสดงผลฟอนต์เบลอบนหน้าจอความละเอียดสูง (High-DPI Blurry GUI):**
  * *ปัญหา:* Tkinter บน Windows 10/11 สเกลหน้าจอผิดพลาด ตัวหนังสือและเส้นกราฟเบลอ
  * *แนวทางแก้ไข:* เรียกใช้ Windows Native API ผ่าน `ctypes.windll.shcore.SetProcessDpiAwareness(1)` บังคับให้โปรแกรม Render ที่ความคมชัด 1:1
* **ปัญหาที่ 2: เครื่องปลายทางไม่มีฟอนต์ที่กำหนดไว้ (Missing Custom Typography):**
  * *ปัญหา:* หากเครื่องอาจารย์ไม่มีฟอนต์ Prompt หน้าจอจะสลับไปใช้ฟอนต์ระบบ ทำให้ Layout บิดเบี้ยว
  * *แนวทางแก้ไข:* นำเข้าฟอนต์เข้า Process ชั่วคราวผ่าน `ctypes.windll.gdi32.AddFontResourceExW` โดยไม่ต้องติดตั้งลงเครื่อง Windows
* **ปัญหาที่ 3: ข้อความภาษาไทยเป็นภาษาต่างดาวเมื่อเปิดไฟล์ CSV บน Excel:**
  * *ปัญหา:* Excel บน Windows อ่าน UTF-8 มาตรฐานผิดรูปแบบ ทำให้ชื่อบริษัทภาษาไทยแสดงผลเสียหาย
  * *แนวทางแก้ไข:* เข้ารหัสไฟล์ส่งออกด้วย `encoding='utf-8-sig'` (เพิ่ม Byte Order Mark: BOM) ให้ Excel ตรวจพบภาษาไทยได้ถูกต้องทันที
* **ปัญหาที่ 4: การวาดแผนภูมิสถิติโดยไม่พึ่งพา External Library ขนาดใหญ่:**
  * *ปัญหา:* การใช้ Matplotlib ทำให้ไฟล์มีขนาดใหญ่และต้องติดตั้ง dependencies เพิ่มเติม
  * *แนวทางแก้ไข:* เขียนฟังก์ชันคำนวณพิกัดมุมและองศาเรขาคณิต เพื่อวาดกราฟแท่งและ Donut Chart บน `tk.Canvas` แบบ Native 100%

> **🖼️ คำแนะนำภาพประกอบ:** ภาพตารางเปรียบเทียบ "Problem vs Solution" พร้อมรูป Crop ย่อยแสดงผลลัพธ์ (เช่น ภาพเปรียบเทียบก่อน-หลังการปรับ DPI Aware หรือภาพตัวอย่างไฟล์ Excel ภาษาไทยที่ถูกต้อง)

---

## สไลด์ที่ 9: การนำไปประยุกต์ใช้งานและแนวทางต่อยอด (Applications & Future Work)

* **การนำไปประยุกต์ใช้งานจริง (Real-world Applications):**
  * **นักศึกษาจบใหม่ / ผู้หางาน:** บริหารจัดการประวัติการสมัครงานนับสิบบริษัทอย่างเป็นมืออาชีพ ไม่พลาดการสัมภาษณ์
  * **ศูนย์แนะแนวและสหกิจศึกษาของมหาวิทยาลัย:** แจกจ่ายให้นักศึกษาใช้เป็นเครื่องมือติดตามการยื่นขอฝึกงาน (Internship Tracking)
  * **ฟรีแลนซ์ / ผู้รับงานอิสระ:** ปรับใช้เป็นระบบติดตามการส่งใบเสนอราคา (Quotation / Proposal Tracker) แก่ลูกค้า
* **แนวทางการพัฒนาต่อยอดในอนาคต (Next Steps & Enhancements):**
  * **ระบบแจ้งเตือนผ่าน Desktop & Line Notify:** ส่งข้อความเตือนเมื่อมีรายการค้างรอผลเกินกำหนดเข้าสู่สมาร์ตโฟน
  * **ระบบจัดเก็บเอกสารแนบ (Resume / Portfolio Attachment):** รองรับการผูกไฟล์ PDF ของเรซูเม่แต่ละเวอร์ชันไว้กับประวัติการสมัคร
  * **ระบบสำรองข้อมูลบนคลาวด์ (Cloud Sync):** ซิงก์ฐานข้อมูล SQLite ขึ้น Google Drive / OneDrive เพื่อเปิดใช้งานได้หลายอุปกรณ์

> **🖼️ คำแนะนำภาพประกอบ:** แผนผัง Roadmap (ระยะสั้น: Attachments & Notification, ระยะยาว: Multi-device Cloud Sync) พร้อมรูป Mockup ไอคอนแอปพลิเคชันบน Desktop และมือถือ

