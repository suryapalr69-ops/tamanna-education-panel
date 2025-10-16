# tamanna-education-panel
Education Management Panel for Tamanna Educations (Admin, Counselor, and B2B Partner System)
# 🎓 Tamanna Educations – Education Management Panel (Final Version)

## 💡 Overview
Tamanna Educations ka panel ek **multi-role management system** hai — jisme 3 role honge:
- **Admin**
- **Counselor**
- **B2B Partner**

Ye system student admission, course fee management, document upload, I-card generation, aur WhatsApp notification ke liye banaya gaya hai.  
Theme color – **White & Blue** (Modern and Responsive for mobile and desktop).

---

## 🔐 1. Login Roles

### 🧑‍💼 Admin
Admin poore system ka head hai.  
Admin ke paas sabhi control honge:
- Universities add/edit karna  
- Courses aur fee structure Excel file se upload karna  
- Centers create karna (address, mobile no., owner name, mail ID, sharing percentage ke sath)  
- Counselors assign karna centers ko  
- Students ka data manage karna  
- OA Number aur Enrollment Number Excel se update karna  
- News post karna (auto WhatsApp notification ke sath B2B partners ko)  
- All documents download karna (Reference Number ke basis par zip file form me)  
- I-cards generate karna enrolled students ke liye  
- Wallet recharge approval manage karna  

### 🧑‍🏫 Counselor
Counselor centers ke head hote hain.  
- B2B partner ke liye form upload kar sakte hain (center code fill karke)  
- Students ke application process kar sakte hain  
- Assigned centers ke forms edit kar sakte hain  
- B2B partners ke pending forms ko verify kar sakte hain  
- B2B partner form process kare to approval notification WhatsApp par jata hai  

### 🤝 B2B Partner
B2B partner student admission upload karta hai.  
- Student ke form upload karne ke time:
  - 10th, 12th, UG, PG details (Subject, Passing Year, Board, Passed/Discontinue)
  - Inke documents upload karne ka option alag-alag (10th, 12th, UG, PG)
  - Student photo, aadhar, signature upload karna
  - Payment section me:
    - Payment Type: UPI / NEFT / Bank Transfer
    - UTR Number aur Payment Date
- Wallet balance auto deduct hoga jab form process karega  
  - Agar balance kam hai → “Please Recharge Wallet” show karega  
- Wallet section me 2 options:
  1. **Recharge** (Scan QR / GPay–Paytm–PhonePe / Bank Transfer with proof upload)
  2. **Payment History** (all transactions with date, amount, proof)
- All Students page me filter:
  1. All Students  
  2. Pending Students  
  3. Processed Students  
  4. Enrolled Students  
- Checkbox ke sath student select kar ke “Process Form” kar sakta hai
  - Counselor process kare to B2B partner ko WhatsApp approval jata hai  
  - B2B partner approve kare tabhi counselor form finalize kar sakega  
- Notification panel me latest admin news aur updates show honge  

---

## 💳 2. Wallet System (Auto Deduction)
- Admin define karega course fees structure Excel se.  
- Jab B2B partner kisi course ka form process kare:
  - Agar wallet me sufficient balance hai → amount auto deduct ho jaye  
  - Agar balance kam hai → "Insufficient Balance, Please Recharge First" alert aaye  
- Admin recharge approve karega proof verify karne ke baad.

---

## 📁 3. Document Management & Bulk Download (Admin)
- Admin ke paas **Documents Download** option hoga.  
- Admin multiple reference numbers paste kare:
  - System automatically un students ke sabhi uploaded documents zip file me download karega:
    - 10th Documents → `10th_docs.zip`
    - 12th Documents → `12th_docs.zip`
    - UG Documents → `ug_docs.zip`
    - PG Documents → `pg_docs.zip`
    - Aadhar → `aadhar_docs.zip`
    - Photos → `photos.zip`
  - File names Reference Number ke hisab se honge (e.g., `REF2025-0001_Aadhar.jpg`).

---

## 🪪 4. Student ID Card Generation
- Jis student ka Enrollment Number update ho gaya hai, unka I-card auto generate ho jaye.  
- ID card me:
  - Student Name  
  - Course Name  
  - Enrollment Number  
  - University Name  
  - Student Photo  
  - QR Code (Student Reference Number se linked)  
  - Tamanna Educations logo aur tagline: *"Where Learning Meets Excellence"*  

---

## 🧾 5. Excel Upload / Update (Admin)
Admin ke liye 2 Excel upload features:

### a. OA Number Updater
| Reference Number | OA Number |
|------------------|-----------|

### b. Enrollment Number Updater
| Reference Number | Enrollment Number |

System automatically student data match karke update karega.  

### c. Course Fees Structure Uploader
| Course Name | University | Session | Fees | Duration |

---

## 📢 6. WhatsApp Notification System
- Jab koi counselor form process kare, to B2B partner ke WhatsApp par approval notification jaye.  
- Jab admin news update kare, sabhi B2B partners ke WhatsApp par message jaye.  
- Jab wallet recharge request approve ho, notification jaye.  
(Mock system for now — Twilio sandbox or dummy popup se simulate karna.)

---

## 🧮 7. Panel Interface & Design
- Theme: **White + Blue** (same as reference image)
- Sidebar always visible (no need to click 3-line icon)
- Responsive on mobile and desktop
- Header:
  - Logo (Tamanna Educations 3D green–pink version)
  - Wallet Balance (₹ symbol ke sath)
  - Logged-in user role indicator (Admin / Counselor / B2B Partner)
- Sidebar Items:
  - Dashboard  
  - All Students  
  - New Application  
  - Re-Registration  
  - Exams (coming soon)  
  - Wallet  
  - News  
  - Documents Download  
  - Logout  

---

## 🔧 8. Database & Storage
- Database: **MongoDB**
- Files Storage: Local `/uploads/` folder
  - Subfolders: `/uploads/students`, `/uploads/payments`, `/uploads/10th`, `/uploads/12th`, `/uploads/ug`, `/uploads/pg`, `/uploads/idcards`

---

## 🧩 9. Technologies
- Frontend: React + TailwindCSS
- Backend: Node.js + Express.js
- Database: MongoDB
- File Uploads: Multer
- PDF/ID Card: jsPDF or PDFKit
- Notifications: Twilio Sandbox (mock)
- Excel Handling: XLSX (SheetJS)
- Authentication: JWT Tokens

---

## ✅ 10. Additional Functionalities
- Auto reference number generation: `REFYYYY-000X`
- Search bar for students by name, reference, or center code
- Quick filter tabs for All / Pending / Processed / Enrolled
- Download Student Form (PDF) option
- Multi-user login dashboard with role-based routing

---

# ⚙️ Final Output
Ek complete, professional, and responsive **Tamanna Educations Management System**,  
jisme Admin, Counselor, aur B2B partner ke sabhi role seamlessly integrated hain  
aur mobile/desktop dono view me attractive interface ke sath kaam karta hai.
