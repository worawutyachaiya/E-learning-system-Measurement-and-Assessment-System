# 🎓 ระบบเรียนรู้ HTML & CSS ออนไลน์

ระบบการเรียนรู้ออนไลน์สำหรับวิชา HTML และ CSS ที่มีระบบข้อสอบและการติดตามผลการเรียนสำหรับนักเรียน พร้อมระบบจัดการสำหรับผู้ดูแล

## ✨ คุณสมบัติหลัก

### 👨‍🎓 สำหรับนักเรียน
- 📚 **ระบบเรียนออนไลน์** - เรียน HTML และ CSS ผ่านวิดีโอบทเรียน
- 📝 **ระบบข้อสอบ** - Pre-test และ Post-test สำหรับแต่ละบทเรียน
- 📊 **ติดตามผลการเรียน** - ดูคะแนนและความก้าวหน้าของตนเอง
- 🔐 **ระบบสมาชิก** - ลงทะเบียนและเข้าสู่ระบบที่ปลอดภัย
- 📱 **Responsive Design** - ใช้งานได้ทุกอุปกรณ์

### 👨‍💼 สำหรับผู้ดูแลระบบ
- 📊 **Dashboard** - ภาพรวมสถิติการใช้งานระบบ
- 👥 **จัดการนักเรียน** - ดูข้อมูลและผลการเรียนของนักเรียน
- 📝 **จัดการข้อสอบ** - สร้าง แก้ไข และจัดการข้อสอบ
- 🎥 **จัดการวิดีโอ** - อัปโหลดและจัดการวิดีโอบทเรียน
- 📈 **รายงานผล** - วิเคราะห์ผลการเรียนและสถิติต่างๆ

## 🛠️ เทคโนโลยีที่ใช้

### Frontend
- **Next.js 15** - React Framework
- **TypeScript** - Type Safety
- **Tailwind CSS 4** - Styling
- **Lucide React** - Icons

### Backend
- **Next.js API Routes** - Backend API
- **Prisma** - Database ORM
- **PostgreSQL** - Database
- **JWT** - Authentication
- **bcrypt** - Password Hashing

### Cloud Services
- **Cloudinary** - Image/Video Storage
- **Nodemailer** - Email Service

## 🚀 การติดตั้งและใช้งาน

### 1. Clone Repository
```bash
git clone https://github.com/your-username/project-end.git
cd project-end
```

### 2. ติดตั้ง Dependencies
```bash
npm install
```

### 3. ตั้งค่า Environment Variables
สร้างไฟล์ `.env.local` และกรอกข้อมูลต่อไปนี้:

```env
# Database
DATABASE_URL="postgresql://username:password@localhost:5432/your-database"

# JWT Secret
JWT_SECRET="your-super-secret-jwt-key"

# Cloudinary (สำหรับจัดเก็บรูปภาพ)
CLOUDINARY_CLOUD_NAME="your-cloud-name"
CLOUDINARY_API_KEY="your-api-key"
CLOUDINARY_API_SECRET="your-api-secret"

# Email Service (NodeMailer)
EMAIL_HOST="smtp.gmail.com"
EMAIL_PORT=587
EMAIL_USER="your-email@gmail.com"
EMAIL_PASS="your-app-password"
```

### 4. ตั้งค่า Database
```bash
# Generate Prisma Client
npm run db:generate

# Push schema to database
npm run db:push

# หรือใช้ migrations
npm run db:migrate
```

### 5. เริ่มต้นใช้งาน
```bash
# Development mode
npm run dev

# Production build
npm run build
npm start
```

เปิดเบราว์เซอร์ไปที่ [http://localhost:3000](http://localhost:3000)

## 📁 โครงสร้างโปรเจค

```
project-end/
├── app/                    # Next.js App Router
│   ├── admin/             # หน้าจัดการสำหรับ Admin
│   │   ├── quiz/          # จัดการข้อสอบ
│   │   ├── students/      # จัดการนักเรียน
│   │   └── video/         # จัดการวิดีโอ
│   ├── api/               # API Routes
│   │   ├── auth/          # Authentication
│   │   ├── quizzes/       # Quiz Management
│   │   └── videos/        # Video Management
│   ├── login/             # หน้าเข้าสู่ระบบ
│   ├── register/          # หน้าลงทะเบียน
│   └── course/            # หน้าเรียนออนไลน์
├── components/            # React Components
├── lib/                   # Utilities และ Configurations
├── prisma/               # Database Schema และ Migrations
├── public/               # Static Files
└── scripts/              # Utility Scripts
```

## 🔑 การใช้งานระบบ

### สำหรับนักเรียน
1. **ลงทะเบียน** - สร้างบัญชีใหม่ด้วยข้อมูลนักเรียน
2. **เข้าสู่ระบบ** - ใช้รหัสนักเรียนและรหัสผ่าน
3. **ทำ Pre-test** - ทำข้อสอบก่อนเรียนเพื่อประเมินความรู้เดิม
4. **เรียนบทเรียน** - ดูวิดีโอและศึกษาเนื้อหา
5. **ทำ Post-test** - ทำข้อสอบหลังเรียนเพื่อประเมินความเข้าใจ

### สำหรับผู้ดูแลระบบ
1. **เข้าสู่ระบบ Admin** - ใช้บัญชีผู้ดูแล
2. **จัดการข้อสอบ** - สร้างและแก้ไขข้อสอบ
3. **จัดการวิดีโอ** - อัปโหลดวิดีโอบทเรียน
4. **ติดตามนักเรียน** - ดูผลการเรียนและความก้าวหน้า

## 📊 คุณสมบัติพิเศษ

- **🔒 ระบบรักษาความปลอดภัย** - JWT Authentication & Password Hashing
- **📱 Responsive Design** - ใช้งานได้ทุกอุปกรณ์
- **⚡ Performance Optimized** - Image optimization และ Lazy loading
- **🎨 Modern UI/UX** - ออกแบบด้วย Tailwind CSS
- **📈 Analytics** - สถิติการใช้งานและผลการเรียน

## 🤝 การมีส่วนร่วม

หากต้องการมีส่วนร่วมในการพัฒนา:

1. Fork repository นี้
2. สร้าง feature branch (`git checkout -b feature/amazing-feature`)
3. Commit การเปลี่ยนแปลง (`git commit -m 'Add amazing feature'`)
4. Push ไปยัง branch (`git push origin feature/amazing-feature`)
5. เปิด Pull Request

## 📝 License

โปรเจคนี้อยู่ภายใต้ MIT License - ดูไฟล์ [LICENSE](LICENSE) สำหรับรายละเอียด

## 👥 ผู้พัฒนา

- **Developer** - [Your Name](https://github.com/your-username)

## 📞 ติดต่อ

หากมีคำถามหรือต้องการความช่วยเหลือ สามารถติดต่อได้ที่:
- Email: your-email@example.com
- GitHub Issues: [Create an issue](https://github.com/your-username/project-end/issues)

---

⭐ ถ้าโปรเจคนี้มีประโยชน์ อย่าลืม Star repository นี้นะครับ!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
