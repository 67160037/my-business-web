# ☕ Daily Grind Coffee — Website

เว็บไซต์สำหรับร้านกาแฟ Daily Grind Coffee ถูกออกแบบขึ้นเพื่อเป็นช่องทางประชาสัมพันธ์ออนไลน์ ให้ลูกค้าสามารถเข้าถึงข้อมูลเกี่ยวกับร้าน เมนูบริการ ทีมงาน และช่องทางการติดต่อได้อย่างสะดวก ทุกหน้าได้รับการจัดโครงสร้างอย่างเป็นระบบและอ่านง่าย รวมถึงมีฟอร์มติดต่อและแผนที่เพื่อช่วยให้ค้นหาร้านได้ง่ายขึ้น เว็บไซต์นี้ช่วยเพิ่มความน่าเชื่อถือของร้านและเป็นสื่อกลางในการเชื่อมต่อกับลูกค้าอย่างมีประสิทธิภาพ

## รายละเอียดโปรเจค

โปรเจคนี้ประกอบด้วย 4 หน้า ได้แก่:

- `index.html` — หน้าแรก แนะนำร้าน และบริการเด่น
- `about.html` — ข้อมูลเกี่ยวกับร้านและทีมงาน
- `services.html` — แสดงรายการบริการ พร้อมตารางเปรียบเทียบแพ็กเกจ
- `contact.html` — ฟอร์มติดต่อ และแผนที่ Google Maps

หน้าเว็บทั้งหมดเชื่อมโยงถึงกันด้วย navigation menu

---

## โครงสร้างไฟล์ (File Structure)

```
my-business-web/
├── index.html
├── about.html
├── services.html
├── contact.html
├── images/
│   ├── bakery.webp
│   ├── barista
│   ├── cafe logo.png
│   ├── cafe.jpg
│   ├── co working.jpg
│   ├── co-working.jpg
│   ├── manager
│   ├── Screenshot 2025-12-06 135605.png
│   ├── Screenshot 2025-12-06 135618.png
│   ├── Screenshot 2025-12-06 140528.png
│   ├── Screenshot 2025-12-06 140538.png
│   ├── Screenshot 2025-12-06 143159.png
│   ├── Screenshot 2025-12-06 143242.png
│   └── Screenshot 2025-12-06 143609.png
│   ├── กาแฟ.jpg
│   ├── คนทำเบเกอรี่.jpg
│   ├── เครื่องดื่ม.jpg
│   ├── เบเกอรี่.jpg
│   └── เมล็ดกาแฟ.jpg
└── README.md
```

---

## รูปหน้าจอหน้าเว็บ (Screenshots)

### หน้าแรก (Home)

![Home](images/Screenshot%202025-12-06%20135605.png)
![Home](images/Screenshot%202025-12-06%20135618.png)

### หน้าเกี่ยวกับ (About)

![About](images/Screenshot%202025-12-06%20140528.png)
![About](images/Screenshot%202025-12-06%20140538.png)

### หน้าบริการ (Services)

![Services](images/Screenshot%202025-12-06%20143609.png)
![Services](images/Screenshot%202025-12-06%20143159.png)

### หน้าติดต่อ (Contact)

![Contact](images/Screenshot%202025-12-06%20143242.png)

---

## รายละเอียดของแต่ละหน้า

### index.html (หน้าแรก)

- Header พร้อม logo และชื่อร้าน
- Navigation menu เชื่อมทุกหน้า
- Hero section พร้อมภาพและข้อความต้อนรับ
- Featured services 3 รายการ (ใช้ `<article>`, `<figure>`)
- Footer

### about.html (เกี่ยวกับ)

- ข้อมูลเรื่องราวร้าน
- รูปทีมงาน (ใช้ `<figure>` + `<figcaption>`)
- Vision & Mission
- ลิงก์กลับหน้าแรก

### services.html (บริการ)

- รายการบริการทั้งหมด
- Section แยกบริการแต่ละอย่าง
- ตารางเปรียบเทียบแพ็กเกจ (`<table>`)

### contact.html (ติดต่อ)

- ฟอร์มติดต่อ (name, email, message)
- HTML5 validation (`required`, `type="email"`)
- ที่อยู่ร้าน
- แผนที่ Google Maps (iframe embed)

---

## ลิงก์ไปยังแต่ละหน้า

- หน้าแรก (Home): `./index.html`
- เกี่ยวกับ (About): `./about.html`
- บริการ (Services): `./services.html`
- ติดต่อ (Contact): `./contact.html`

---

## ตัวอย่างคำสั่ง Git (Commit แบบละเอียด)

```bash
git init
git config user.name "67160037"
git config user.email "67160037@go.buu.ac.th"

# 1.1 Header
git add index.html"
git commit -m "1.1: Add Header"

# 1.2 Navigation
git add index.html
git commit -m "1.2: Add navigation menu"

# 1.3 Hero Section
git add index.html images/hero-coffee.jpg
git commit -m "1.3: Add hero section"

# 1.4 Featured Services
git add index.html images/service-1.jpg images/service-2.jpg images/service-3.jpg
git commit -m "1.4: Add featured services"

# 1.5 Footer
git add index.html
git commit -m "1.5: Add footer"

# About Page
git add about.html
git commit -m "Add about page structure and content"

# Services Page
git add services.html
git commit -m "Add services page with table"

# Contact Page
git add contact.html
git commit -m "Add contact form and Google Map"

# Push
git remote add origin https://github.com/username/my-business-web.git
git push -u origin master
```

---

## How to Run

1. เปิด index.html in browser
2. หรือเปิดด้วย Live Server in VS Code

---
