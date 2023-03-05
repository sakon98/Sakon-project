# โปรเจคทดสอบการใช้ git
คำสั่งการใช้ git เบื้องต้น
- git --version // แสดง version ของ git ในตัวเครื่อง
- git config -- list // แสดงการตั้งค่าของ git ของเรา
- git config --global user.email "test@gmail.com" // add email
- git config --global user.name "name" // ตั้งชื่อ git
- git init // สร้าง local git repository
- git add <file_name> // เพิ่มไฟล์เข้าไปใน staging area (check in)ระบุไฟล์ตามชื่อไฟล์
- git add *.html // เพิ่มไฟล์เข้าไปใน staging area (check in) ระบุไฟล์ตามนามสกุล
- git add . // เพิ่มไฟล์เข้าไปใน staging area (check in) ระบุไฟล์ทั้งหมดใน repository
- git rm --cached . // ลบไฟล์หรือโฟลเดอร์ออกจาก git repository (remove) ลบทั้งหมด
- git rm --cached <file_name> // ลบไฟล์หรือโฟลเดอร์ออกจาก git repository (remove) ระบุไฟล์
- git status // ดูสถานะเปลี่ยนแปลงของ repository
- touch app.js // เพิ่มไฟล์
- git commit -m "comment" // เก็บประวัติถาวรไว้ในเครื่องและใส่ comment
- git log // แสดง log ทั้งหมด
- git log --oneline // แดสง log เหลือบรรทัดเดียว
- git log --graph // แสดง log เป็น branch
- git diff <commit_id> // ตรวจสอบและเปรียบเทียบไฟล์แบบระบุ commit id
- git diff <commit_id> <commit_id> // ตรวจสอบและเปรียบเทียบไฟล์แบบเปรียบเทียบระหว่าง commit id
- git checkout <file_name> // คำสั่งย้อนกลับไปยัง commit ล่าสุดหรือยกเลิกการแก้ไข file
- git reset // การย้อน version กลับไปสภาพก่อน add file เข้าสู่ staging area 
- git reset -- option(soft,miced,hard) <commit_id> 
// soft = ลบ commit ทั้งหมดที่อยู่หลัง commit id แล้วนำไฟล์ที่เคยอยู่ใน commit นั้นกลับมายัง staging area
// mixed = ลบ commit ทั้งหมดที่อยู่หลัง commit id แล้วนำไฟล์ที่เคยอยู่ใน commit นั้นกลับมายัง working directory
// hard = ลบ commit ทั้งหมดที่อยู่หลัง commit id แล้วนำไฟล์ที่เคยอยู่ใน commit
- git branch // แสดงชื่อ branch
- git checkout -b <name_branch> // สลับและสร้าง branch ห้ามเว้นวรรคให้ใช้ขีดแทน
- git branch -d <name_branch> // delete branch
- git checkout <name_branch> // สลับไป branch ที่ต้องการ
- git checkout main หรือ master // สลับไปใช้ branch หลัก
- git merge <name_branch> // การรวม branch ให้อยู่ที่ branch หลักก่อนใช้ merge
- git branch -M main // สั่งให้อยู่ที่ branch main ก่อนทำการ push
- git remote add origin <https://github.com/test.git> // การ add file เตรียมส่งไปยัง github ที่เราต้องการ
- git push -u origin main // push file ขึ้น git hub 
- git push // กรณี push โปรเจคที่มีการผูกกับ git hub แล้วใช้แค่คำสั่งนี้ได้เลย
- git pull // ดึงข้อมูลบน remote repository(server) มาอัพเดตเครื่องของเรา (local repository)
- touch READMR.md // สร้างไฟล์ READMR.md เพื่อเป็นเอกสารประกอบ project
- git clone <https://github.com/test.git> // clone โปรเจคบน github มายังเครื่อง local
