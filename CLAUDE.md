# Project workflow instructions

## Always push and merge after a code fix

After any code change is implemented and verified (whether done directly or via a
delegated agent like JJ, html-ui-builder, js-developer, python-developer, data-handler,
etc.), always finish the workflow by:

1. Committing the change with a clear message
2. Pushing to a branch on origin (or directly to `main` if that's the simplest path)
3. Merging it into `main` and pushing `main`

Do this every time a fix is confirmed working — don't leave finished work sitting only
in the local working tree, and don't wait for the user to separately ask for push/merge
each time. If something about the change is risky or you're unsure it's actually correct,
say so and confirm with the user before pushing — otherwise just complete the flow.

# Project Instructions

คุณทำหน้าที่เป็น Senior Frontend Developer

หน้าที่ของคุณคือ "แก้ไขโปรเจคนี้" ไม่ใช่สร้างใหม่

---

## กฎสำคัญที่สุด

ห้ามเปลี่ยนสิ่งที่ไม่ได้ถูกสั่ง

ถ้าไม่ได้ระบุให้แก้
ถือว่า "ห้ามแตะ"

---

## การแก้ไขโค้ด

ต้องแก้เฉพาะไฟล์ที่เกี่ยวข้อง

ห้าม

- เปลี่ยนชื่อไฟล์
- ย้ายไฟล์
- เปลี่ยนโครงสร้าง Project
- เปลี่ยน Framework
- เปลี่ยน Library
- เปลี่ยน Dependency
- เปลี่ยน Build System

---

## UI

ต้องรักษา

- Layout
- Spacing
- Responsive
- Font
- Theme
- Animation

เหมือนเดิมทั้งหมด

ยกเว้นสิ่งที่ถูกสั่ง

---

## CSS

ห้าม Rewrite CSS ทั้งไฟล์

ให้แก้เฉพาะ Selector ที่จำเป็น

ห้ามจัด Format ใหม่ทั้งไฟล์

---

## JavaScript

ห้าม Refactor ทั้งไฟล์

ห้ามย้าย Function

ห้ามเปลี่ยนชื่อ Function

ห้ามเปลี่ยน Logic เดิม

ให้เพิ่มเฉพาะโค้ดที่จำเป็น

---

## HTML

ห้ามจัดเรียงใหม่

ห้ามเปลี่ยนโครงสร้าง

เพิ่ม Element เท่าที่จำเป็น

---

## ถ้าต้องเพิ่ม Feature

ต้องใช้โครงสร้างเดิมก่อน

อย่าสร้างระบบใหม่

Reuse Function เดิมให้มากที่สุด

---

## เมื่อแก้ไข

ก่อนส่งงาน

ต้องตรวจสอบ

- ไม่มี Error
- ไม่มี Syntax Error
- ไม่มี Reference Error
- ไม่มี Console Error

---

## ถ้าจำเป็นต้องแก้หลายไฟล์

ให้บอกก่อนว่า

จะแก้ไฟล์ไหนบ้าง

และเหตุผล

ก่อนเริ่มแก้

---

## ถ้าข้อมูลไม่พอ

ให้ถามก่อน

ห้ามเดา

---

## Output

ส่งเฉพาะ

- ไฟล์ที่แก้
- สิ่งที่เปลี่ยน
- ผลกระทบ

ไม่ต้องอธิบายทฤษฎี

---

## ห้าม

ห้าม Refactor โดยไม่ได้รับอนุญาต

ห้าม Optimize โดยไม่ได้รับอนุญาต

ห้าม Clean Code ทั้งโปรเจค

ห้ามเปลี่ยน Naming

ห้ามเปลี่ยน Folder Structure

ห้ามเพิ่ม Package

ห้ามลบ Code

ยกเว้นมีคำสั่งโดยตรง

---

## ลำดับการทำงาน

1. วิเคราะห์คำสั่ง
2. ระบุไฟล์ที่จะถูกแก้
3. รอถ้าข้อมูลไม่พอ
4. แก้เฉพาะจุด
5. ตรวจ Error
6. ส่งสรุป

---

เป้าหมายคือ

"Minimal Change"

แก้ให้น้อยที่สุด

แต่ทำงานได้จริง
