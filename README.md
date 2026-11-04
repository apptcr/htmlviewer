# 🌐 Minimal HTML Reader & Viewer

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.2.0-indigo.svg)
![Build](https://img.shields.io/badge/build-passing-brightgreen.svg)

**Minimal HTML Reader** คือเว็บแอปพลิเคชันสำหรับเปิดอ่านและตรวจทานไฟล์ HTML ที่เน้นความโปร่ง สบายตา และใช้งานง่าย (Focus & Readability) ออกแบบมาเพื่อให้ผู้ใช้สามารถอ่านเนื้อหาในไฟล์ HTML ได้อย่างเต็มที่ โดยปราศจากสิ่งรบกวน พร้อมระบบจัดการหลายไฟล์ (Multi-File Management) ในหน้าเดียว

---

## 📸 คุณสมบัติเด่น (Key Features)

* **👁️ Default Preview Focus:** เปิดหน้าเว็บมาพร้อมโหมดแสดงผล (Preview Mode) ทันที ให้ความรู้สึกเหมือนกำลังอ่านเอกสารจริง
* **📂 Multi-File Workspace:** นำเข้าไฟล์ HTML ได้พร้อมกันหลายไฟล์ และจัดการสลับไฟล์อ่านได้จาก Sidebar ทางด้านซ้าย
* **↔️ Collapsible Sidebar:** แถบรายการไฟล์ด้านข้างสามารถพับเก็บ (Collapse) หรือเปิดออกได้อย่างลื่นไหล เพื่อเพิ่มพื้นที่การอ่านแบบไร้สิ่งรบกวน
* **🎨 3 View Modes:**
  * **Preview Mode:** แสดงผลการเรนเดอร์หน้าเว็บผ่าน Isolated Sandbox Iframe
  * **Code Mode:** ตรวจดู Source Code พร้อมระบบ Syntax Highlighting (PrismJS)
  * **Split Mode:** แสดงผล Preview คู่กับ Source Code เพื่อเปรียบเทียบโค้ดและผลลัพธ์พร้อมกัน
* **☁️ Drag & Drop Support:** ลากไฟล์ HTML มาวางที่ส่วนใดก็ได้ของหน้าจอเพื่อนำเข้าไฟล์ทันที
* **🌙 Dark / Light Mode:** สลับธีมสว่างและมืดได้ตามต้องการ เพื่อการอ่านที่ถนอมสายตา
* **⚡ One-Click Copy & Fullscreen:** ปุ่มคัดลอกโค้ดไปยัง Clipboard และปุ่มขยายการแสดงผลแบบเต็มหน้าจอ (Fullscreen)

---

## 🛠️ เทคโนโลยีที่ใช้ (Tech Stack)

| ส่วนประกอบ | เทคโนโลยีที่ใช้ | รายละเอียด |
| :--- | :--- | :--- |
| **Core** | HTML5, JavaScript (ES6+) | Single-page application ทำงานบนเบราว์เซอร์ 100% |
| **Styling** | [Tailwind CSS](https://tailwindcss.com/) | ตกแต่ง UI ด้วย Utility-first CSS เรียบหรู ละมุนตา |
| **Icons** | [Font Awesome 6](https://fontawesome.com/) | ไอคอนสัญลักษณ์ระบบ |
| **Code Highlight** | [PrismJS](https://prismjs.com/) | ระบบจัดสี Syntax Highlighting สำหรับ Source Code |

---

## 🚀 วิธีการใช้งาน (Getting Started)

เนื่องจากเว็บแอปพลิเคชันนี้ถูกออกแบบมาในรูปแบบ **Single File Mandate** จึงไม่จำเป็นต้องติดตั้งโปรแกรมหรือ Node.js ใดๆ

1. **ดาวน์โหลดไฟล์** `index.html` ลงในเครื่องคอมพิวเตอร์
2. **ดับเบิลคลิกเปิดไฟล์** `index.html` ผ่านเว็บเบราว์เซอร์ใดก็ได้ (Chrome, Edge, Firefox, Safari)
3. **เริ่มอ่านไฟล์ HTML:**
   * กดปุ่ม **`+ เพิ่มไฟล์`** บนแถบเมนูด้านบน เพื่อเลือกเปิดไฟล์ HTML ของคุณ (เลือกพร้อมกันหลายไฟล์ได้)
   * หรือ **ลากไฟล์ HTML มาวาง (Drag & Drop)** ลงบนหน้าเว็บได้ทันที
   * คลิกเลือกชื่อไฟล์ที่ Sidebar ด้านซ้ายเพื่อสลับไฟล์ที่ต้องการอ่าน
   * กดปุ่ม `<` หรือไอคอนเมนูเพื่อพับเก็บ Sidebar เมื่อต้องการพื้นที่อ่านแบบเต็มจอ

---

## 🖥️ ภาพรวมการทำงาน (UI Overview)

```text
+-----------------------------------------------------------------------+
| [☰ เมนูไฟล์] [+ เพิ่มไฟล์]  sample.html    [👁 Preview|⌨ Code|▥ Split]  [📋][⛶][🌙]|
+------------------+----------------------------------------------------+
| 📁 ไฟล์ทั้งหมด (3)  |                                                    |
| ---------------- |                                                    |
|  📄 index.html   |                 PREVIEW / CODE PANE                |
|  📄 page2.html   |                 (Focus Reading Area)               |
|  📄 test.html    |                                                    |
|                  |                                                    |
|                  |                                                    |
+------------------+----------------------------------------------------+
```

---

## 📄 ใบอนุญาต (License)

โปรเจกต์นี้จัดทำขึ้นภายใต้ใบอนุญาต **MIT License** - สามารถนำไปใช้งาน ปรับแต่ง และเผยแพร่ได้อย่างอิสระ
