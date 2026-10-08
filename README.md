# สมการชีวิต — 21 Days Challenge

เว็บต้นแบบสำหรับพนักงาน ใช้งานบน GitHub Pages ได้ฟรี

## ฟังก์ชันในตัวอย่าง
- หน้า Login พนักงาน
- Daily Check-in
- Progress 21 วัน
- My Journey
- เนื้อหา Level 1
- Badge / Recognition
- HR Dashboard ตัวอย่าง
- บันทึก Progress ใน browser เพื่อทดลองได้ทันที

## เปิดเว็บบน GitHub Pages
1. สร้าง Repository ใหม่ใน GitHub เช่น `21days-challenge`
2. Upload ไฟล์ทั้งหมดในโฟลเดอร์นี้ไปที่ root ของ Repository
3. ไปที่ Settings > Pages
4. Source เลือก `Deploy from a branch`
5. Branch เลือก `main` และ `/ (root)` แล้ว Save
6. รอสักครู่ GitHub จะแสดง URL ของเว็บ

## การต่อฐานข้อมูลจริงด้วย Firebase
ไฟล์ `firebase-config.example.js` เป็น Template สำหรับตั้งค่า Firebase และ `firestore.rules` เป็นกฎเริ่มต้นที่จำกัดข้อมูลของผู้ใช้แต่ละคน

ก่อนใช้กับพนักงานจริง ควรเพิ่ม Firebase Authentication, Firestore และสิทธิ์ HR/Admin โดยไม่เก็บ Reflection ส่วนบุคคลไว้ใน Repository

## หมายเหตุด้านข้อมูล
GitHub Pages เป็น static hosting ดังนั้นห้ามใส่รายชื่อพนักงาน คำตอบ Check-in หรือข้อมูลส่วนบุคคลลงในไฟล์ของ Repository โดยตรง ข้อมูลจริงควรอยู่ในฐานข้อมูลที่ตั้งสิทธิ์ไว้ เช่น Firebase Firestore
