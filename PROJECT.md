# PROJECT.md

# Project Name

Boiler Energy Data
---
# Purpose
เว็บสำหรับบันทึกข้อมูลประจำวันของหน่วยงาน Boiler
ปัญหาที่แก้:
- ลดการกรอกข้อมูลหลายไฟล์ Excel
- รวมข้อมูลไว้ในระบบเดียว
- ลดเวลาการทำงาน
- ช่วยให้สมาชิกใหม่เรียนรู้ระบบได้ง่ายขึ้น
---
# Main Feature
## Boiler Data Entry
ระบบสำหรับบันทึกข้อมูล Boiler จำนวน 3 เครื่อง
---
# Boiler Information
## Boiler No.5
Type:
Palm Shell Boiler
Capacity:
20 ton
Fuel:
Palm Kernel Shell
### Input Data
| Data | Unit | Description |
|---|---|---|
| Feed water | m³ | ปริมาณน้ำที่ใช้ผลิตไอน้ำจากมิเตอร์ |
| Operating hour | hr | ชั่วโมงการทำงานจาก Hour meter |
| Fuel consumption | kg | ปริมาณเชื้อเพลิงที่ใช้ แยกซ้าย/ขวาห้องเผาไหม้ |
| ASH | kg | ปริมาณขี้เถ้าที่เกิดขึ้น |
### ASH Detail
มีช่องกรอก:
- ASH รอบที่ 1
- ASH รอบที่ 2
- ASH รอบที่ 3
- ASH รอบที่ 4
Additional:
- ASH from wet scrubber
- ใช้กรอกเมื่อมีการตักบ่อ Wet Scrubber
### Blowdown Setting
Valve:
- Valve 1
- Valve 2
- Valve 3
ข้อมูลที่บันทึก:
- Operating cycle time
- Valve opening duration
---
## Boiler No.2
Type:
Bunker Oil Boiler
Capacity:
4 ton
### Input Data
| Data | Unit | Description |
|---|---|---|
| Feed water | m³ | ปริมาณน้ำผลิตไอน้ำ |
| Operating hour | hr | ชั่วโมงทำงาน |
| Fuel consumption | liter | ปริมาณน้ำมันเตาที่ใช้ |
### Blowdown Setting
Valve:
- Valve 1
- Valve 2
ข้อมูล:
- Operating cycle time
- Valve opening duration
---
## Boiler No.4
Type:
Bunker Oil Boiler
Capacity:
10 ton
### Input Data
| Data | Unit | Description |
|---|---|---|
| Feed water | m³ | ปริมาณน้ำผลิตไอน้ำ |
| Operating hour | hr | ชั่วโมงทำงาน |
| Fuel consumption | liter | ปริมาณน้ำมันเตาที่ใช้ |
### Blowdown Setting
Valve:
- Valve 1
- Valve 2
- Valve 3
ข้อมูล:
- Operating cycle time
- Valve opening duration
# Feature 2: Palm Shell
## Purpose
หน้าสำหรับบันทึกข้อมูลการรับกะลาปาล์ม และติดตาม Stock Card
---
## Data Entry
### Receiving Table
รองรับการรับเข้าจำนวน 6 เที่ยวต่อวัน
ข้อมูลที่ต้องบันทึก:
| Field | Unit |
|---|---|
| Supplier Weight | kg |
| Supplier Moisture | % |
| LUF Weight | kg |
| LUF Moisture | % |
---
## Palm Shell Price / Ash Removal
ข้อมูล:
- ราคากะลาปาล์ม
- น้ำหนักขี้เถ้าที่นำออกจากบริษัท
---
## Palm Shell Stock Card
แสดงข้อมูล:
- ยอดคงเหลือจากเมื่อวาน
- ปริมาณใช้รวมต่อวัน
- ยอดรับเข้า
- ยอดคงเหลือวันนี้
---
# Feature 3: Bunker Oil
## Purpose
หน้าสำหรับบันทึกข้อมูลการรับน้ำมันเตาและติดตาม Stock
---
## Oil Receiving
ข้อมูล:
- ปริมาณน้ำมันเตารับเข้า
- ราคาน้ำมันเตา
---
## Bunker Oil Stock Card
แสดงข้อมูล:
- ยอดคงเหลือจากเมื่อวาน
- ปริมาณใช้รวมต่อวัน
- ยอดรับเข้า
- ยอดคงเหลือวันนี้
---
# Feature 4: Water
## Purpose
หน้าสำหรับบันทึกค่ามิเตอร์น้ำภายในโรงงาน
รายละเอียด:
- จำนวนมิเตอร์ทั้งหมด 23 จุด
ข้อมูลที่บันทึก:
- ค่า Meter
- ปริมาณการใช้
---
# Feature 5: Electricity
## Purpose
หน้าสำหรับบันทึกข้อมูลการใช้ไฟฟ้าประจำวัน
ข้อมูล:
- ค่าไฟฟ้าที่ใช้ในแต่ละวัน
---
# Feature 6: LPG
## Status
อยู่ระหว่างปรับปรุง
---
# Feature 7: Report Dashboard
## Purpose
Dashboard สำหรับแสดงข้อมูลจากระบบทั้งหมด
---
## Report Types
### Daily Report
สรุปข้อมูลรายวัน
### Monthly Report
สรุปข้อมูลรายเดือน
### Accounting Report
รายงานสำหรับส่งฝ่ายบัญชี
มี:
- Export Form
### Water Usage Report
รายงานการใช้น้ำ
---
# Feature 8: Import Excel
## Purpose
นำเข้าข้อมูลจาก Excel เข้าสู่ระบบ
---
# Import Main Data
Button:
`importBtn`
## File Support
รองรับ:
- .xlsx
- .xlsm
---
## Sheet Selection
Requirement:
- ต้องระบุชื่อ Sheet
- ค่าเริ่มต้น: 0726
กรณีไม่พบ Sheet:
ระบบต้อง:
- แจ้ง Sheet ที่มีอยู่จริง
- ให้เลือกใหม่
---
## Data Range
อ่านข้อมูล:
- เริ่ม Row 5
- ถึง Row 60
---
## Date Validation
Column A ต้องเป็น Date
ถ้าไม่ใช่:
- ข้าม Row นั้น
---
## Header Detection
ข้อมูลบางประเภท:
- Electricity
- Boiler 5 Fuel
- Ash
- Palm Shell
ระบบต้อง:
- ค้นหาจาก Header อัตโนมัติ
- ไม่ใช้ Column Index ตายตัว
เหตุผล:
Layout Excel สามารถเปลี่ยนตำแหน่ง Column ได้ในแต่ละเดือน
---
## Data Filtering
ไม่บันทึกข้อมูลที่:
- ค่าเป็น 0
- ช่องว่าง
- ขึ้นต้นด้วย #
---
# Import Water Meter
Button:
`importWaterBtn`
## File Rule
เหมือน Import Main Data:
- .xlsx
- .xlsm
- ระบุ Sheet
- อ่าน Row 5-60
- Column A ต้องเป็น Date
---
## Meter Validation
Meter:
- M1-M31
- ต้องเป็นตัวเลขเท่านั้น
ถ้าอ่านไม่ได้:
- ข้ามข้อมูล
---
# Import Utility Data
Button:
`importUtilityBtn`
## File Support
รองรับ:
- .xls
- .xlsx
- .xlsm
---
## Required Sheets
รองรับ 3 Sheet:
1. เชื้อเพลิง
2. ชั่วโมงทำงาน
3. กะลาปาล์ม Boiler 5
Requirement:
- ต้องระบุชื่ออย่างน้อย 1 Sheet
- ไม่จำเป็นต้องครบทั้ง 3
---
## Missing Sheet Handling
กรณี Sheet ที่ระบุไม่พบ:
ระบบต้อง:
- แจ้งชื่อ Sheet ที่หาย
- นำเข้า Sheet อื่นที่ถูกต้องต่อได้
ไม่หยุดทั้งหมด
---
## Data Range
อ่านข้อมูล:
Row 4-60
---
## Date Validation
Column A ต้องเป็น Date
ถ้าไม่ใช่:
- ข้าม Row นั้น

# Business Rules
## Stock Calculation
Palm Shell:
ยอดคงเหลือวันนี้ =
ยอดคงเหลือเมื่อวาน + รับเข้า - ใช้งาน
Bunker Oil:
ยอดคงเหลือวันนี้ =
ยอดคงเหลือเมื่อวาน + รับเข้า - ใช้งาน
## Water Usage
ปริมาณใช้ =
Meter ปัจจุบัน - Meter ก่อนหน้า
## Import Rules
ห้าม:
- เปลี่ยน Header Detection เป็น Column Fix
- บันทึกข้อมูลที่ไม่ผ่าน Validation
