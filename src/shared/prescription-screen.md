# ระบบ Screen ใบสั่งยา และค้นประวัติการสั่งยาใน HOSxP

![PS Top](images/prescription-screen-top.webp)

ท่านสามารถค้นหาใบสั่งยาใน HOSxP ด้วยการระบุ QN, HN, VN หรือ เลขประจำตัวประชาชน (CID) แล้วคลิก `ค้นหา` หรือกดปุ่ม Enter

![PS Hx](images/prescription-screen-hx.webp)

หลังจากค้นหา จะได้รายการใบสั่งยา เรียงตามวันที่และเวลา จากใหม่ ลงไปหาเก่า

ระบบจะนำใบสั่งยาล่าสุด มาแสดงรายละเอียดให้อัตโนมัติ ซึ่งท่านสามารถเลือกดูใบสั่งยาอื่นได้เช่นกัน

<div class="warning">

ในหัวข้อ `นัดหมาย` ท่านสามารถคลิกที่ <i class="fa-solid fa-reply" style="color:orange;"></i>

เพื่อไปยังวันที่รับบริการได้ (เฉพาะกรณีที่ผู้ป่วยมาตรงกับวันนัดเท่านั้น)

</div>

### รายการยา
![PS Drug Alert](images/prescription-screen-drug-alert.webp)

แสดงรายการยาในใบสั่งยา โดยหากเป็นยาใหม่ หรือเปลี่ยนวิธีใช้ ระบบจะแสดงด้วยพื้นหลังสีฟ้า

![PS Drug Modal](images/prescription-screen-drug-modal.webp)

เมื่อคลิกที่รายการยา จะเปิดหน้าต่างแสดงรายการยาทุกตัว พร้อมข้อมูลการจ่ายยาชนิดเดียวกันครั้งล่าสุด เพื่อตรวจสอบและให้คำแนะนำได้ถูกต้อง

### Drug Interaction
![PS Drug Interaction](images/prescription-screen-drug-interaction.webp)

หากมีคู่ยา ที่มีอันตรกิริยาระหว่างกัน (drug interaction) ตรงตามที่บันทึกคู่ยาไว้ใน HOSxP ระบบจะนำมาแสดงไว้ที่นี้

### LAB
![PS Lab](images/prescription-screen-lab.webp)

แสดงรายการ `LAB ล่าสุด` และ `LAB ของ Visit` ตามรายการที่เลือกไว้ในระบบ (กรุณาติดต่อผู้ดูแลระบบ หากต้องการเพิ่ม/ลดรายการ) 

<div class="warning">

ท่านสามารถคลิกที่ ค่าผลตรวจ (ตัวเลขสีน้ำเงิน)

เพื่อแสดงค่าผลตรวจดังกล่าวในอดีต ในรูปแบบกราฟเส้นได้ ดังรูป

![PS Lab Graph](images/prescription-screen-lab-graph.webp)

</div>

### ข้อความเตือนการใช้ยา
![PS Notice](images/prescription-screen-notice.webp)

แสดงคำเตือนตามเงื่อนไข เช่น การใช้ยา NSAIDs, ACEIs, CCBs มากกว่า 1 ตัวยาในกลุุ่มเดียวกัน เป็นต้น (กรุณาติดต่อผู้ดูแลระบบ หากต้องการเพิ่ม/ลดเงื่อนไข) 

### บันทึกเวลาดำเนินการ
![PS Act Accept](images/prescription-screen-act-accept.webp)

รองรับการบันทึกเวลาในการ รับรายการ ตรวจสอบ และจ่ายยา ของเจ้าหน้าที่ห้องยา (หากคลิกที่ ปุ่มอักษรสีแดง จะบันทึกเวลาของขั้นตอนนั้นๆ ใหม่ด้วยเวลาปัจจุบัน)

![PS Act Check](images/prescription-screen-act-check.webp)

![PS Act Done](images/prescription-screen-act-done.webp)

![PS Act End](images/prescription-screen-act-end.webp)

### บันทึกการส่งยาทางไปรษณีย์
![PS Postal](images/prescription-screen-postal.webp)

รองรับการบันทึก การส่งยาทางไปรษณีย์ (ส่ง/ไม่ส่ง) พร้อมเวลาและผู้บันทึก

![PS Postal Send](images/prescription-screen-postal-send.webp)

![PS Postal Resend](images/prescription-screen-postal-resend.webp)

### อื่นๆ
![PS Gadget](images/prescription-screen-gadget.webp)

เช่น การบันทึกการปรับยา ระหว่างให้บริการ Telemed, การบันทึกการให้บริการทางเภสัชกรรม เป็นต้น