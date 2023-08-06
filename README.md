# CT519-JRW  นาย จิรวัฒน์ นพชัยอำนวยโชค 65130029

### หลักการออกแบบ ออกแบบเป็น single page application
แยกระบบออกเป็นหน้าบ้านและหลังบ้าน โดยใช้หน้าบ้านเป็น react และหลังบ้านเป็น nodejs และฐานข้อมูลเป็น mongodb 
และใช้ cloud Aws docker แบ่งเป็น frontend, backend และ databases แยก container กัน
ส่วน cloud ที่ใช้ deploy นั้นจะเป็น aws ec2 (Instance type t2.micro) สถาปัตยกรรม X86 

โดยเว็บจะมี 1 หน้า,single page application เรียงเนื้อหาลงมาแยกองค์ประกอบเป็น  
1.ส่วนของ About ชื่อ นามสกุล และรูป
2.เลื่อนลงมาจะเจอส่วนของ research อธิบายส่วนของงานวิจัย
3.Mycontact สามารถกรอก ชื่อ-และเบอร์โทร เพิ่มได้ การลบสามารถคลิกลบที่ปุ่มข้อมูลที่เพิ่มมาได้เลย

### การเตรียมการระบบ Cloud 
เป็นการใช้ ec2 โดยใช้ aws linux ในการทำ และ install docker environment รวมถึง git เพืื่อ clone data มาเพื่อ deploy 

###การ deploy ตัว code มาทำงาน
1.สร้างเว็บและ sql ให้เรียบร้อย พร้อมทั้ง dockerfile และ docker-compose.yaml
2.เตรียม git ให้พร้อม
3.สร้าง repositories ct519-JRW
4.อัพโหลด 1 ขึ้น repositories ct519-JRW
5.ใน Aws install docker engine ให้เรียบร้อย
6.ใน Aws install docker compose ให้เรียบร้อย
7.ใน command line git clone (https://github.com/JP-jirawat/CT519-JRW.git)
8.cd ct519-JRW
9.chmod -R 777 all file and folder
10.docker-compose up --build
การ deploy ตัว code มาทำงาน<br />
1.สร้างเว็บและ sql ให้เรียบร้อย พร้อมทั้ง dockerfile และ docker-compose.yaml<br />
2.เตรียม git ให้พร้อม<br />
3.สร้าง repositories ct519-JRW<br />
4.อัพโหลด 1 ขึ้น repositories ct519-JRW<br />
5.ใน Aws install docker engine ให้เรียบร้อย<br />
6.ใน Aws install docker compose ให้เรียบร้อย<br />
7.ใน command line git clone (https://github.com/JP-jirawat/CT519-JRW.git)<br />
8.cd ct519-JRW<br />
9.chmod -R 777 all file and folder<br />
10.docker-compose up --build <br />
