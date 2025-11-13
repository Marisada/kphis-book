# รายการผู้ป่วยใน

ตัวกรองในการค้นหา `ผู้ป่วยใน` ที่มีในระบบ KPHIS ได้แก่
* `แผนก`
* [Passcode](#ward-passcode) (เฉพาะเปิดด้วยเมนู `แพทย์`, `พยาบาล`, และ `อื่นๆ`)
* `แพทย์เจ้าของไข้`
* `แพทย์ผู้ตอบ Consult` (เฉพาะเปิดด้วยเมนู `แพทย์`)
* `การประเมินข้อมูลแพ้ยาใบแรกรับ` (เฉพาะเปิดด้วยเมนู `เภสัชกร`)
* `HN, AN, ชื่อ-สกุล` : กรอก HN, AN หรือชื่อ-สกุล ผู้ป่วย อย่างใดอย่างหนึ่ง

เปิดจากเมนู `แพทย์`
![IPD Search Patient Doctor](images/ipd-search-patient-doctor.webp)

ผลการค้นหา จะแสดงทางลัดไป..
* [แฟ้มผู้ป่วย IPD](main.md)
* [บันทึกประวัติและตรวจร่างกายแรกรับ](admission-note-dr.md)
* [บันทึกการสรุปเวชระเบียน (In-Patient Summary)](summary.md)

เปิดจากเมนู `พยาบาล`
![IPD Search Patient Nurse](images/ipd-search-patient-nurse.webp)

ผลการค้นหา จะแสดงทางลัดไป..
* [แฟ้มผู้ป่วย IPD](main.md)
* [บันทึกประวัติและตรวจร่างกายแรกรับ](admission-note-dr.md)
* [ประเมินสภาพผู้ป่วยแรกรับและแบบแผนสุขภาพ](admission-note-nurse.md)

เปิดจากเมนู `เภสัชกร`
![IPD Search Patient Pharmacist](images/ipd-search-patient-pharmacist.webp)

ผลการค้นหา จะแสดงทางลัดไป..
* [แฟ้มผู้ป่วย IPD](main.md)

เปิดจากเมนู `อื่นๆ`
![IPD Search Patient Other](images/ipd-search-patient-other.webp)

ผลการค้นหา จะแสดงทางลัดไป..
* [แฟ้มผู้ป่วย IPD](main.md)

## Ward Passcode
ระบบ `Passcode` ใช้สำหรับปกปิดการแสดง `แผนก` ที่ต้องการ (`แผนก` ที่มี `Passcode` กำหนดไว้ จะไม่ปรากฏในกล่องตัวเลือก `แผนก`)

หากใส่รหัส `Passcode` ของ `แผนก` นั้นๆ ได้ถูกต้อง ระบบจะแสดงข้อมูลของ `แผนก` ที่ปกปิดนั้นให้  

![Passcode](images/passcode.webp)

การสร้าง `Passcode` สามารถทำได้ ด้วยการเลือก `สำหรับ ward` เป็น `แผนก` ที่ต้องการปกปิด  
หลังจากยืนยันรหัสผ่านของท่าน และกดปุ่ม `สร้าง Passcode ใหม่` ระบบจะส่ง `Passcode` ให้ท่าน
<div class="warning">

* ปุ่ม <i class="fa fa-cog" style="color:orange;"></i> สำหรับเปลี่ยน `Passcode` จะปรากฏเฉพาะผู้ได้รับสิทธิจากผู้ดูแลระบบเท่านั้น
* `Passcode` ของแต่ละ `แผนก` จะมีเพียงรหัสเดียว, หากสร้างใหม่ จะยกเลิก `Passcode` เก่าทันที
</div>