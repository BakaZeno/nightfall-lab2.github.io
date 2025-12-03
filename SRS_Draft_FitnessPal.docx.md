**Software Requirements Specification**  
**(SRS)**

**FitnessPal**

ENGCE301: การออกแบบและพัฒนาซอฟต์แวร์  
Software Design and Development

Term Project \- NightFall

| ชื่อ-นามสกุล | รหัสนักศึกษา | Role |
| :---- | :---- | :---- |
| **นายจักรกฤษณ์ จาปัญญะ** | 66543206040-8 | **Team Leader / Tester / Frontend** |
| **นายเมย์คาร์ สุวรรณวิสุทธิ์** | 66543206085-3 | **Frontend** |
| **นายปรเมษฐ สุริคำ** | 66543206038-2 | **Frontend / System Analysis** |
| **นายณัฐกิตติ์ ยั่งยืนปิยรัตน์** | 66543206014-3 | **Backend** |
| **นายจิรวัฒน์ มาลัยวรรณ** | 66543206070-5 | **Backend** |

Version: 1.0  
Date: วันที่ / 27/11/2568  
มหาวิทยาลัยเทคโนโลยีราชมงคลล้านนา  
Rajamangala University of Technology Lanna

# **Document Control**

## **Version History**

| Version | Date | Author | Description of Change |
| :---- | :---- | :---- | :---- |
| **1.0** | 27/11/2568 | Team FitnessPal | Initial draft |

## **Document Approvals**

| Role | Name | Signature & Date |
| :---- | :---- | :---- |
| **Product Owner** | Team FitnessPal |  |
| **Team Lead** | นายจักรกฤษณ์ จาปัญญะ | จักรกฤษณ์ |
| **Instructor** | อาจารย์ ธนิต เกตูเเก้ว |  |

# **Table of Contents**

[**Document Control	2**](#heading=)

[Version History	2](#heading=)

[Document Approvals	2](#heading=)

[**Table of Contents	3**](#heading=)

[**1\. Introduction	5**](#heading=)

[1.1 Purpose	5](#heading=)

[1.2 Scope	5](#heading=)

[ขอบเขตของระบบครอบคลุม:	5](#ขอบเขตของระบบครอบคลุม:)

[ขอบเขตที่ไม่รวมในระบบ (Out of Scope):	5](#ขอบเขตที่ไม่รวมในระบบ-\(out-of-scope\):)

[1.3 Definitions, Acronyms, and Abbreviations	5](#heading=)

[1.4 References	6](#heading=)

[1.5 Overview	6](#heading=)

[**2\. Overall Description	7**](#heading=)

[2.1 Product Perspective	7](#heading=)

[2.2 Product Functions	8](#heading=)

[2.3 User Characteristics	8](#heading=)

[2.4 Constraints	8](#heading=)

[2.5 Assumptions and Dependencies	9](#heading=)

[**3\. Specific Requirements	10**](#heading=)

[3.1 Functional Requirements	10](#heading=)

[3.1.1 User Authentication Module	10](#heading=)

[3.2 Non-Functional Requirements	14](#heading=)

[3.2.1 Performance Requirements	14](#heading=)

[3.2.2 Security Requirements	14](#heading=)

[3.2.3 Usability Requirements	14](#heading=)

[3.2.4 Reliability Requirements	14](#heading=)

[3.2.5 Portability Requirements	14](#heading=)

[**4\. Appendices	15**](#heading=)

[4.1 Use Case Diagrams	15](#heading=)

[4.2 Wireframes / Mockups	15](#heading=)

[4.3 Data Dictionary	15](#heading=)

[4.4 User Interview Notes Summary	15](#heading=)

[**5\. Glossary	16**](#heading=)

[**การใช้งาน Template นี้	17**](#heading=)

# **1\. Introduction**

## **1.1 Purpose**

เอกสารฉบับนี้ระบุความต้องการ (Requirements) ของระบบ FitnessPal มีวัตถุประสงค์เพื่อ:

* ใช้เป็นแนวทางในการออกแบบ (Design) และพัฒนา (Development) ระบบ  
* ใช้เป็นเกณฑ์ในการทดสอบ (Testing) และตรวจสอบความสมบูรณ์ของระบบ  
* ใช้เป็นสัญญาระหว่างทีมพัฒนากับผู้มีส่วนได้ส่วนเสีย (Stakeholders)

## **1.2 Scope**

ระบบ **FitnessPal** เป็นเว็บแอปพลิเคชันที่มีวัตถุประสงค์เพื่อช่วยผู้ใช้บันทึกข้อมูลด้านสุขภาพ เช่น อาหาร การออกกำลังกาย และเป้าหมายส่วนบุคคล เพื่อให้ผู้ใช้สามารถติดตามและพัฒนาสุขภาพได้อย่างเป็นระบบ

### **ขอบเขตของระบบครอบคลุม:** {#ขอบเขตของระบบครอบคลุม:}

* การจัดการบัญชีผู้ใช้ (สมัครสมาชิก, เข้าสู่ระบบ, แก้ไขข้อมูลส่วนตัว)  
* การบันทึกข้อมูลอาหาร การออกกำลังกาย และน้ำหนัก  
* การแสดงสรุปข้อมูลสุขภาพในรูปแบบรายงานและกราฟความคืบหน้า

### **ขอบเขตที่ไม่รวมในระบบ (Out of Scope):** {#ขอบเขตที่ไม่รวมในระบบ-(out-of-scope):}

* การเชื่อมต่ออุปกรณ์สวมใส่อัจฉริยะ (Smartwatch / Wearable Devices)  
* ระบบแนะนำอาหารและการออกกำลังกายด้วย AI แบบอัตโนมัติ

## **1.3 Definitions, Acronyms, and Abbreviations**

| Term | Definition |
| :---- | :---- |
| **FR** | Functional Requirement |
| **NFR** | Non-Functional Requirement |
| **UI** | User Interface |
| **API** | Application Programming Interface |

## 

## **1.4 References**

* **IEEE Standard 830-1998** – Recommended Practice for Software Requirements Specifications

* **User Interview Notes** – บันทึกการสัมภาษณ์ผู้ใช้งานกลุ่มนักศึกษาและเทรนเนอร์ (จัดทำโดยทีมผู้พัฒนา)

* **ENGCE301 Course Materials** – เอกสารประกอบการเรียนรายวิชา การออกแบบและพัฒนาซอฟต์แวร์

## **1.5 Overview**

เอกสารนี้ประกอบด้วย 3 ส่วนหลัก:  
• Section 1 (Introduction) \- แนะนำภาพรวมของเอกสารและโปรเจกต์  
• Section 2 (Overall Description) \- อธิบายภาพรวมของระบบ  
• Section 3 (Specific Requirements) \- ระบุความต้องการโดยละเอียด

# **2\. Overall Description**

## **2.1 Product Perspective**

ระบบ FitnessPal เป็นเว็บแอปพลิเคชันแบบ Standalone  

ที่ทำงานบน Web Browser (Chrome, Firefox, Safari, Edge)

ระบบมีการเชื่อมต่อกับ:

• ระบบยืนยันตัวตน (Authentication System – JWT)

• ระบบฐานข้อมูล (Database Management System – SQLite/MongoDB)

## **2.2 Product Functions**

ฟังก์ชันหลักของระบบ (สรุปย่อจาก Functional Requirements):

1. ระบบจัดการบัญชีผู้ใช้ (สมัครสมาชิก, เข้าสู่ระบบ, แก้ไขข้อมูลส่วนตัว)

2. ระบบบันทึกอาหาร การออกกำลังกาย และข้อมูลสุขภาพ

3. ระบบแสดงรายงานและกราฟความคืบหน้าด้านสุขภาพ

## **2.3 User Characteristics**

กลุ่มผู้ใช้หลักของระบบ:

* **นักศึกษาทั่วไป:**  
   ผู้ใช้หลักของระบบ ส่วนใหญ่มีทักษะการใช้งานเทคโนโลยีในระดับปานกลาง  
   ต้องการระบบที่ใช้งานง่าย ไม่ซับซ้อน และแสดงผลชัดเจน  
* **เทรนเนอร์:**  
   มีความรู้ด้านการออกกำลังกาย ต้องการระบบที่สามารถสร้างโปรแกรมฝึก  
   และดูความคืบหน้าผู้ฝึกได้สะดวก  
* **อาจารย์:**  
   ต้องการดูข้อมูลเชิงภาพรวม เพื่อใช้ติดตามหรือส่งเสริมกิจกรรมด้านสุขภาพ  
* **นักกีฬา:**  
   ใช้งานระบบในระดับสูง ต้องการข้อมูลสถิติที่แม่นยำและละเอียด  
* **YouTuber:**  
   ใช้ระบบในเชิงนำเสนอผลลัพธ์ ต้องการข้อมูลที่เข้าใจง่ายและดูน่าสนใจ  
* **Developers (ผู้พัฒนา):**  
   ต้องสามารถเข้าถึงข้อมูลระบบและตรวจสอบปัญหา เพื่อดูแลบำรุงรักษาระบบ

## **2.4 Constraints**

ข้อจำกัดในการพัฒนาระบบ:

* งบประมาณ: จำกัด (ใช้ทรัพยากรฟรีหรือ Open-source เป็นหลัก)

* เวลา: ต้องพัฒนาให้แล้วเสร็จภายในภาคการศึกษานี้ (สัปดาห์ที่ 16\)

* เทคโนโลยี: ใช้ React.js สำหรับ Frontend, Node.js สำหรับ Backend, และ SQLite หรือ MongoDB สำหรับฐานข้อมูล

* ทีมพัฒนา: มีสมาชิก **5 คน** ทำงานประมาณ **3 ชั่วโมง/สัปดาห์**

## **2.5 Assumptions and Dependencies**

**สมมติฐาน (Assumptions):**

* ผู้ใช้มี Internet Connection

* ผู้ใช้มี Web Browser ที่รองรับ HTML5

* ผู้ใช้กรอกข้อมูลสุขภาพด้วยความถูกต้อง

* ผู้ใช้ยินยอมให้ระบบจัดเก็บข้อมูลส่วนบุคคลตามนโยบายความเป็นส่วนตัว

**Dependencies (สิ่งที่ระบบพึ่งพา):**

* ต้องมี Web Server สำหรับ Deploy ระบบ

* ต้องมี Database Server สำหรับจัดเก็บข้อมูล

* ระบบต้องพึ่งพา Library ของ React และ Node.js

* ต้องมีระบบ Authentication สำหรับการจัดการผู้ใช้

# **3\. Specific Requirements**

## **3.1 Functional Requirements**

### **3.1.1 User Authentication Module**

**FR-001: User Registration**

**Description:** ผู้ใช้สามารถลงทะเบียนเข้าใช้ระบบด้วยอีเมล รหัสผ่าน และข้อมูลส่วนตัว

| Input | Email (format: xxx@xxx.xxx), Password (min 8 chars), ชื่อ-นามสกุล |
| :---- | :---- |
| **Process** | ตรวจสอบ email ซ้ำในฐานข้อมูล, Hash password ด้วย bcrypt, สร้าง User account |
| **Output** | สร้าง User account สำเร็จ และส่ง confirmation email |
| **Precondition** | Email ต้องไม่ซ้ำในระบบ, Password ต้องผ่านเกณฑ์ความแข็งแรง |
| **Priority** | ⭐ Must Have |

**FR-002: User Login**

**Description:** ผู้ใช้สามารถเข้าสู่ระบบด้วย Email และ Password

| Input | Email, Password |
| :---- | :---- |
| **Process** | ตรวจสอบ email และ password จากฐานข้อมูล, สร้าง JWT Token |
| **Output** | Redirect ไปหน้า Dashboard พร้อม Session Token |
| **Precondition** | User ต้องลงทะเบียนแล้ว |
| **Priority** | ⭐ Must Have |

**FR-003: User Profile**

**Description:** ผู้ใช้สามารถแก้ไขข้อมูลสุขภาพส่วนตัว

| Input |  อายุ, เพศ, น้ำหนัก, ส่วนสูง, ระดับกิจกรรม |
| :---- | :---- |
| **Process** | ตรวจสอบและอัปเดตข้อมูลในระบบ |
| **Output** | Redirect ไปหน้า Dashboard พร้อม Session Token |
| **Precondition** | โปรไฟล์ผู้ใช้ที่อัปเดตล่าสุด |
| **Priority** | Must Have |

**FR-004: Goal Management**

**Description:** ผู้ใช้สามารถตั้งเป้าหมายสุขภาพ

| Input | เป้าหมาย (ลดน้ำหนัก / เพิ่มกล้าม / คงน้ำหนัก) |
| :---- | :---- |
| **Process** | บันทึกเป้าหมาย |
| **Output** | แสดงเป้าหมาย |
| **Precondition** | ผู้ใช้ Login แล้ว และกรอกข้อมูลพื้นฐานครบ |
| **Priority** | Must Have |

**FR-005: Meal Tracking**

**Description:** บันทึกมื้ออาหาร

| Input | ชื่ออาหาร, ปริมาณ, แคลอรี่ |
| :---- | :---- |
| **Process** | บันทึก |
| **Output** | รายการอาหาร |
| **Precondition** | ผู้ใช้ Login แล้ว และตั้งเป้าหมายแล้ว |
| **Priority** | Must Have |

**FR-006: Workout Tracking**

**Description:** บันทึกการออกกำลังกาย

| Input | ประเภท, เวลา, ความหนัก |
| :---- | :---- |
| **Process** | คำนวณแคลอรี่เผาผลาญ |
| **Output** | ประวัติการออกกำลังกาย |
| **Precondition** | ผู้ใช้ Login แล้ว |
| **Priority** | Should Have |

**FR-007: Calorie Calculation**

**Description:** ระบบคำนวณ BMR / TDEE

| Input | อายุ, น้ำหนัก, ส่วนสูง, ระดับกิจกรรม |
| :---- | :---- |
| **Process** | คำนวณสูตร |
| **Output** | ค่าแคลอรี่แนะนำ |
| **Precondition** | ผู้ใช้กรอก ข้อมูลสุขภาพครบ |
| **Priority** | Must Have |

**FR-008: Reporting Calculation**

**Description:** แสดงพลังงานเข้า–ออก

| Input | ข้อมูลสะสม |
| :---- | :---- |
| **Process** | รวมและคำนวณ |
| **Output** | สรุปพลังงาน |
| **Precondition** | มีข้อมูลอาหารหรือการออกกำลังกายในวันนั้น |
| **Priority** | Should Have |

**FR-009: รายงานรายสัปดาห์**

**Description:** แสดงรายงานย้อนหลัง

| Input | ช่วงวันที่ |
| :---- | :---- |
| **Process** | ดึงข้อมูลย้อนหลัง |
| **Output** | รายงาน |
| **Precondition** | มีข้อมูลอย่างน้อย 7 วัน |
| **Priority** | Should Have |

**FR-010: กราฟความคืบหน้า**

**Description:** แสดงกราฟแนวโน้ม

| Input | ข้อมูลประวัติ |
| :---- | :---- |
| **Process** | สร้างกราฟ |
| **Output** | กราฟ |
| **Precondition** | มีข้อมูลสะสม |
| **Priority** | Could Have |

 

**FR-011: เทรนเนอร์สร้างโปรแกรมฝึก**

**Description:** สร้างแผนฝึก

| Input | ตารางฝึก |
| :---- | :---- |
| **Process** | บันทึกแผน |
| **Output** | โปรแกรมฝึก |
| **Precondition** | เทรนเนอร์ Login แล้ว |
| **Priority** | Should Have |

**FR-012: เทรนเนอร์ติดตามผู้ฝึก**

**Description:** ดูความคืบหน้า

| Input | ข้อมูลผู้ฝึก |
| :---- | :---- |
| **Process** | วิเคราะห์ |
| **Output** | รายงาน |
| **Precondition** | มีผู้ฝึกในระบบ |
| **Priority** | Should Have |

**FR-013: Admin**

**Description:** จัดการผู้ใช้

| Input | ข้อมูลผู้ใช้ |
| :---- | :---- |
| **Process** | เพิ่ม/ลบ/แก้ไข |
| **Output** | ฐานข้อมูลอัปเดต |
| **Precondition** | Admin Login แล้ว |
| **Priority** | Should Have |

## **3.2 Non-Functional Requirements**

### **3.2.1 Performance Requirements**

| ID | Requirement | Metric/Target |
| :---- | :---- | :---- |
| **NFR-001** | Page Load Time | หน้าเว็บต้องโหลดเสร็จภายใน 2 วินาที (measured with Lighthouse) |
| **NFR-002** | API Response Time | API Response Time ต้องไม่เกิน 500ms (95th percentile) |
| **NFR-003** | Concurrent Users | ระบบต้องรองรับผู้ใช้พร้อมกัน 100 คน |

### **3.2.2 Security Requirements**

| ID | Requirement | Implementation |
| :---- | :---- | :---- |
| **NFR-004** | Password Security | รหัสผ่านต้อง hash ด้วย bcrypt (salt rounds \>= 10\) |
| **NFR-005** | Session Management | Session Token (JWT) ต้องมีอายุไม่เกิน 24 ชม. |
| **NFR-006** | Data Encryption | ต้องใช้ HTTPS สำหรับการสื่อสารทั้งหมด |

### **3.2.3 Usability Requirements**

* NFR-007: ผู้ใช้ทั่วไปต้องสามารถ \[ทำงานหลัก\] สำเร็จภายใน 3 คลิก  
* NFR-008: Interface ต้องรองรับภาษาไทยและภาษาอังกฤษ  
* NFR-009: ระบบต้องมี Error messages ที่เข้าใจง่ายและบอกวิธีแก้ไข

### **3.2.4 Reliability Requirements**

* NFR-010: ระบบต้องมี uptime 99% (downtime ไม่เกิน 3.65 วัน/ปี)  
* NFR-011: ต้องมี Backup ข้อมูลอัตโนมัติทุก 24 ชม.  
* NFR-012: ระบบต้องสามารถ recover จากความผิดพลาดได้ภายใน 5 นาที

### **3.2.5 Portability Requirements**

* NFR-013: เว็บแอปต้องทำงานได้บน Chrome, Firefox, Safari, Edge (latest versions)  
* NFR-014: รองรับทั้ง Desktop (1920x1080), Tablet (768x1024), และ Mobile (375x667)

# **4\. Appendices**

## **4.1 Use Case Diagrams**

![][image1]

## 

## **4.2 Wireframes / Mockups**

## ![][image2]

## 

![][image3]

## **![][image4]**

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## **4.3 Data Dictionary**

ตารางอธิบายโครงสร้างข้อมูลสำคัญ:

1\) ตาราง `User` – เก็บข้อมูลผู้ใช้ทุกบทบาท

| Entity/Table | Attribute | Data Type | Description |
| :---- | :---- | :---- | :---- |
| **User** | user\_id | INT | Primary Key, Auto-increment |
| **User** | email | VARCHAR(255) | อีเมลผู้ใช้, Unique, Not Null |
| **User** | password\_hash | VARCHAR(255) | รหัสผ่านที่ถูก Hash แล้ว |
| **User** | full\_name | VARCHAR(100) | ชื่อ–นามสกุลผู้ใช้ |
| **User** | role | VARCHAR(100) | บทบาทผู้ใช้ เช่น student, trainer, admin |
| **User** | gender | VARCHAR(10) | เพศ (optional) |
| **User** | height\_cm | DECIMAL(5,2) | ส่วนสูง (เซนติเมตร) |
| **User** | weight\_kg | DECIMAL(5,2) | น้ำหนัก (กิโลกรัม) |
| **User** | activity\_level | VARCHAR(20) | ระดับกิจกรรม เช่น low/medium/high |
| **User** | created\_at | DATETIME | วันที่–เวลา สมัครเข้าใช้งาน |
| **User** | updated\_at | DATETIME | วันที่–เวลา แก้ไขข้อมูลล่าสุด |

2\) ตาราง `HealthGoal` – เก็บเป้าหมายสุขภาพของผู้ใช้

| Entity/Table | Attribute | Data Type | Description |
| :---- | :---- | :---- | :---- |
| **HealthGoal** | goal\_id | INT | Primary Key, Auto-increment |
| **HealthGoal** | user\_id | INT | FK → User.user\_id |
| **HealthGoal** | goal\_type | VARCHAR(30) | ประเภทเป้าหมาย: lose\_weight / gain\_muscle / keep |
| **HealthGoal** | target\_weight\_kg | DECIMAL(5,2) | น้ำหนักเป้าหมาย (กิโลกรัม) |
| **HealthGoal** | start\_date | DATE | วันที่เริ่มต้นเป้าหมาย |
| **HealthGoal** | target\_date | DATE | วันที่คาดว่าจะถึงเป้าหมาย |
| **HealthGoal** | status | VARCHAR(20) | สถานะ: active / completed / cancelled |

3\) ตาราง `MealLog` – บันทึกมื้ออาหาร

| Entity/Table | Attribute | Data Type | Description |
| :---- | :---- | :---- | :---- |
| **MealLog** | meal\_id | INT | Primary Key, Auto-increment |
| **MealLog** | user\_id | INT | FK → User.user\_id |
| **MealLog** | log\_date | DATE | วันที่บันทึกมื้ออาหาร |
| **MealLog** | meal\_type | VARCHAR(20) | ประเภทมื้อ: breakfast / lunch / dinner / snack |
| **MealLog** | food\_name | VARCHAR(255) | ชื่ออาหาร |
| **MealLog** | quantity | DECIMAL(5,2) | ปริมาณที่กิน |
| **MealLog** | unit | VARCHAR(50) | หน่วย เช่น g, ml, ช้อน |
| **MealLog** | calories | INT | พลังงานที่ได้รับ (กิโลแคลอรี่) |
| **MealLog** | note | VARCHAR(255) | หมายเหตุเพิ่มเติม (optional) |

4\) ตาราง `WorkoutLog` – บันทึกการออกกำลังกาย

| Entity/Table | Attribute | Data Type | Description |
| :---- | :---- | :---- | :---- |
| **WorkoutLog** | workout\_id | INT | Primary Key, Auto-increment |
| **WorkoutLog** | user\_id | INT | FK → User.user\_id |
| **WorkoutLog** | log\_date | DATE | วันที่ออกกำลังกาย |
| **WorkoutLog** | activity\_type | VARCHAR(100) | ประเภทกิจกรรม เช่น running, cycling |
| **WorkoutLog** | duration\_min | INT | ระยะเวลาออกกำลังกาย (นาที) |
| **WorkoutLog** | intensity\_level | VARCHAR(20) | ความหนัก: low / medium / high |
| **WorkoutLog** | calories\_burned | INT | พลังงานที่ใช้ไป (กิโลแคลอรี่) |
| **WorkoutLog** | note | VARCHAR(255) | หมายเหตุเพิ่มเติม |

5\) ตาราง `Progress Record` – น้ำหนัก/ความคืบหน้ารายวัน

| Entity/Table | Attribute | Data Type | Description |
| :---- | :---- | :---- | :---- |
| **ProgressRecord** | progress\_id | INT | Primary Key, Auto-increment |
| **ProgressRecord** | user\_id | INT | FK → User.user\_id |
| **ProgressRecord** | record\_date | DATE | วันที่บันทึกความคืบหน้า |
| **ProgressRecord** | weight\_kg | DECIMAL(5,2) | น้ำหนักในวันนั้น |
| **ProgressRecord** | body\_fat\_percent | DECIMAL(5,2) | เปอร์เซ็นต์ไขมัน (ถ้ามี) |
| **ProgressRecord** | note | VARCHAR(255) | หมายเหตุ เช่น “ป่วย/พักผ่อนน้อย” |

6\) ตาราง `Workout Plan` – แผนฝึกที่เทรนเนอร์สร้างให้

| Entity/Table | Attribute | Data Type | Description |
| :---- | :---- | :---- | :---- |
| **WorkoutPlan** | plan\_id | INT | Primary Key, Auto-increment |
| **WorkoutPlan** | trainer\_id | INT | FK → User.user\_id (role \= trainer) |
| **WorkoutPlan** | user\_id | INT | FK → User.user\_id (ผู้ฝึก) |
| **WorkoutPlan** | plan\_name | VARCHAR(100) | ชื่อโปรแกรม เช่น “Beginner Full Body” |
| **WorkoutPlan** | start\_date | DATE | วันที่เริ่มใช้โปรแกรม |
| **WorkoutPlan** | end\_date | DATE | วันที่สิ้นสุดโปรแกรม (ถ้ามี) |
| **WorkoutPlan** | status | VARCHAR(20) | active / archived |

7\) ตาราง `WorkoutPlanItem` – รายการในโปรแกรมฝึก

| Entity/Table | Attribute | Data Type | Description |
| :---- | :---- | :---- | :---- |
| **WorkoutPlanItem** | item\_id | INT | Primary Key, Auto-increment |
| **WorkoutPlanItem** | plan\_id | INT | FK → WorkoutPlan.plan\_id |
| **WorkoutPlanItem** | day\_of\_week | TINYINT | วันที่ของสัปดาห์ (1=จันทร์ … 7=อาทิตย์) |
| **WorkoutPlanItem** | activity\_type | VARCHAR(100) | ประเภทการออกกำลังกาย |
| **WorkoutPlanItem** | duration\_min | INT | ระยะเวลา |
| **WorkoutPlanItem** | note | VARCHAR(255) | หมายเหตุ เช่น จำนวนเซต/ครั้ง |

## **4.4 User Interview Notes Summary**

ผู้ใช้ตัวอย่าง 5 คนมีเป้าหมายด้านสุขภาพต่างกัน แต่พบปัญหาร่วมคือ **บันทึกข้อมูลยาก**, **ไม่เข้าใจข้อมูลสุขภาพ**, และ **ต้องการระบบที่ใช้งานง่าย**  
 จากการสัมภาษณ์ พบว่า:

**🔹 Pain Points หลัก**

* บันทึกอาหาร/ออกกำลังกายไม่สะดวก และมักลืมบันทึก  
* ไม่รู้ BMR/TDEE และปริมาณแคลอรี่ที่ควรกิน  
* ข้อมูลย้อนหลังดูยาก ไม่เห็นความคืบหน้า  
* ระบบควรใช้ง่าย รองรับมือถือ และเป็นภาษาไทย

**🔹 ข้อเสนอแนะผู้ใช้**

* ลดขั้นตอนกรอกข้อมูล  
* มี Dashboard และกราฟสรุปชัดเจน  
* มีระบบแจ้งเตือนง่าย ๆ  
* รองรับภาษาไทย

**🔹 Requirements ที่ได้จาก Pain Points**

* **FR:** เพิ่มอาหาร/ออกกำลังกายง่าย, คำนวณ BMR/TDEE อัตโนมัติ, Dashboard \+ กราฟ, แจ้งเตือน  
* **NFR:** Mobile responsive, ใช้งานง่ายใน ≤ 3 คลิก, รองรับภาษาไทย

# 

# 

# **5\. Glossary** 

| Term | Definition |
| ----- | ----- |
| API (Application Programming Interface) | ชุดกฎและโปรโตคอลที่ใช้สำหรับเชื่อมต่อและรับส่งข้อมูลระหว่าง Client และ Server |
| Authentication | กระบวนการตรวจสอบตัวตนของผู้ใช้ก่อนเข้าระบบ เช่น Email \+ Password |
| Authorization | การกำหนดสิทธิ์ว่าผู้ใช้สามารถเข้าถึงหรือใช้งานฟีเจอร์ใดได้บ้าง |
| Bcrypt | อัลกอริทึมสำหรับ Hash รหัสผ่านเพื่อเพิ่มความปลอดภัย |
| BMR (Basal Metabolic Rate) | อัตราการเผาผลาญพลังงานพื้นฐานของร่างกายเมื่ออยู่นิ่ง |
| Calories In | ปริมาณพลังงานที่ผู้ใช้รับเข้าระบบจากการกินอาหาร |
| Calories Out | ปริมาณพลังงานที่ผู้ใช้ใช้ไปจากกิจกรรมหรือการออกกำลังกาย |
| Client | อุปกรณ์หรือเว็บเบราว์เซอร์ที่ผู้ใช้ใช้เข้าถึงระบบ |
| Dashboard | หน้าจอสรุปข้อมูลสำคัญ เช่น แคลอรี่ น้ำหนัก และกราฟความคืบหน้า |
| Data Dictionary | เอกสารอธิบายโครงสร้างข้อมูล เช่น ชื่อตาราง ฟิลด์ ประเภทข้อมูล |
| Database | ระบบจัดเก็บข้อมูลของแอป เช่น MongoDB, SQLite |
| Entity | หน่วยข้อมูลหลักในระบบ เช่น User, MealLog, WorkoutLog |
| Frontend | ส่วนของระบบที่ผู้ใช้โต้ตอบผ่าน UI เช่น Web Interface |
| Hashing | กระบวนการแปลงข้อมูล (เช่น Password) ให้เป็นรหัสที่ย้อนกลับไม่ได้ |
| JWT (JSON Web Token) | รูปแบบ Token ที่ใช้สำหรับ Authentication และ Session Management |
| Mobile Responsive | ความสามารถของเว็บแอปที่ปรับ UI ให้เหมาะสมกับทุกขนาดหน้าจอ |
| Model | โครงสร้างข้อมูลที่ใช้ใน Backend เพื่อเชื่อมต่อกับฐานข้อมูล |
| NFR (Non-Functional Requirement) | ความต้องการที่ไม่ใช่ฟังก์ชัน เช่น Performance, Security, Usability |
| Password Hash | รหัสผ่านที่ผ่านกระบวนการ Hash แล้วเพื่อความปลอดภัย |
| Performance | ความเร็วในการทำงานของระบบ เช่น API Response Time |
| Responsive Design | การออกแบบ UI ให้แสดงผลได้สวยงามบนทุกขนาดหน้าจอ |
| Session | สถานะการเข้าสู่ระบบของผู้ใช้ ใช้ในการตรวจสอบความปลอดภัย |
| Stakeholder | บุคคลหรือกลุ่มคนที่มีส่วนได้ส่วนเสียกับระบบ เช่น ผู้ใช้ ทีมพัฒนา อาจารย์ |
| TDEE (Total Daily Energy Expenditure) | ปริมาณพลังงานที่ร่างกายต้องการต่อวันรวมกิจกรรมทั้งหมด |
| Token | รหัสที่ใช้ยืนยันตัวตนหลังการเข้าสู่ระบบ (เช่น JWT) |
| UI (User Interface) | ส่วนที่ผู้ใช้มองเห็น เช่น ปุ่ม ฟอร์ม และหน้าต่างต่าง ๆ |
| UX (User Experience) | ประสบการณ์ใช้งานของผู้ใช้ว่ารู้สึกสะดวก ใช้ง่าย หรือสับสน |
| User Profile | ข้อมูลผู้ใช้ เช่น ชื่อ อายุ น้ำหนัก ส่วนสูง เป้าหมายสุขภาพ |
| Workout Log | ข้อมูลการออกกำลังกาย เช่น ประเภท ระยะเวลา แคลอรี่ที่ใช้ |

#  

**📚 แหล่งข้อมูลเพิ่มเติม:**

* IEEE Standard 830-1998: IEEE Recommended Practice for Software Requirements Specifications  
* SWEBOK v3.0 \- Chapter 1: Software Requirements  
* Book: "Software Requirements" by Karl Wiegers & Joy Beatty

─────────────────────────────────

Template created for ENGCE301: Software Design and Development  
Rajamangala University of Technology Lanna  
อาจารย์ธนิต เกตุแก้ว  
*Version 1.0 | Academic Year 2024-2025*  


[image1]: <data:image/png;base64,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>

[image2]: <data:image/png;base64,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>

[image3]: <data:image/png;base64,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>

[image4]: <data:image/png;base64,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>