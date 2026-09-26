# EV Charge Tracker — Free Mobile PWA

เวอร์ชันนี้ทำให้เว็บแอปติดตั้งบน Android และ iPhone ได้ฟรีผ่านเบราว์เซอร์ (PWA) และใช้งานออฟไลน์ได้สำหรับตัวแอปที่โหลดไว้แล้ว

## วิธีออนไลน์ฟรีที่แนะนำ: GitHub Pages
1. สร้าง GitHub repository ใหม่ เช่น `ev-charge-tracker`
2. อัปโหลด **ไฟล์และโฟลเดอร์ทั้งหมดในโฟลเดอร์นี้** โดยให้ `index.html` อยู่ระดับบนสุด
3. ไปที่ Settings → Pages
4. เลือก Deploy from branch → `main` → `/ (root)` → Save
5. รอ GitHub สร้างเว็บ แล้วเปิด URL ที่ได้

## Android
เปิด URL ด้วย Chrome → เลือก Install app / Add to Home screen → ติดตั้ง

## iPhone / iPad
เปิด URL ด้วย Safari → Share → Add to Home Screen → Add

## ข้อจำกัดที่ต้องรู้
- ข้อมูลในแอปเก็บในเครื่องของผู้ใช้ ไม่ได้มีระบบบัญชี/ซิงก์ข้ามเครื่อง
- ถ้าล้างข้อมูลเว็บไซต์/เบราว์เซอร์โดยไม่สำรอง ข้อมูลอาจหายได้ ควรใช้ปุ่ม “สำรองข้อมูล” เป็นระยะ
- OCR ใช้ Tesseract.js จาก CDN เมื่อเรียกใช้ครั้งแรก จึงควรเปิดอินเทอร์เน็ตในครั้งแรกที่ใช้สแกน
- การติดตั้ง PWA ฟรี แต่ถ้าต้องการลงเป็นแอปใน Apple App Store หรือ Google Play แบบ native จะมีค่าบัญชีนักพัฒนา/ค่าธรรมเนียมตามแพลตฟอร์ม

## ไฟล์
- `index.html` — เว็บแอป
- `manifest.webmanifest` — ข้อมูลสำหรับติดตั้งเป็น PWA
- `sw.js` — offline cache/service worker
- `icons/` — ไอคอนแอป
