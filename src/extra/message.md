# ระบบข้อความ
แสดงจำนวนข้อความใหม่ที่ยังไม่ได้อ่าน เหนือรูปจดหมาย <i class="fa-regular fa-envelope"></i> ที่เมนูด้านขวา ใกล้กับชื่อผู้ใช้

![Message Badge](images/message-badge.webp)

เมื่อคลิกที่เมนูรูปจดหมาย <i class="fa-regular fa-envelope"></i> จะมีเมนูย่อย ได้แก่

![Message Menu](images/message-menu.webp)

* `ประกาศ` : กล่องจดหมาย ประกาศจากระบบ
* `หอผู้ป่วย` : กล่องจดหมาย ถึงหอผู้ป่วยที่ท่านลงทะเบียนไว้
* `แผนก` : กล่องจดหมาย ถึงแผนกที่ท่านลงทะเบียนไว้
* `ส่วนตัว` : กล่องจดหมาย ถึงท่านโดยเฉพาะ
* <i class="fa-regular fa-pen-to-square" style="color:orange;"></i> : เขียนข้อความใหม่
* <i class="fas fa-gear" style="color:orange;"></i> : ตั้งค่าการรับข่าวสาร

## การตั้งค่า
![Message Gear](images/message-gear.webp)

* เลือกหอผู้ป่วย และแผนก ที่ท่านต้องการรับข่าวสาร (เลือกได้หลายหอผู้ป่วย/แผนก)
* กดปุ่ม <i class="fa-regular fa-floppy-disk" style="color:orange;"></i> `บันทึก`

<div class="warning">

การตั้งค่านี้ ผูกพันกับผู้ใช้งาน  
ไม่ได้จดจำไว้ในเครื่อง
</div>

## การเขียนข้อความ
![Message Compose](images/message-compose.webp)

* `ข้อความ` : เนื้อหาข้อความที่ต้องการส่ง
* `ถึงเจ้าหน้าที่` : ระบุเจ้าหน้าที่ปลายทาง
* `ถึงหอผู้ป่วย` : ระบุหอผู้ป่วยปลายทาง
* `ถึงแผนก` : ระบุแผนกปลายทาง
* `แนบ URL` : ระบุ ที่ตั้งเวปไซต์ (URL) ที่ต้องการแนบพร้อมข้อความ รองรับที่ตั้งภายในและภายนอกโปรแกรม

<div class="warning">

ท่านสามารถส่งข้อความเดียว ไปถึงเจ้าหน้าที่ ถึงหอผู้ป่วย และแผนก ได้ในคราวเดียวกัน    
หากท่านไม่ระบุเจ้าหน้าที่, หอผู้ป่วย, แผนก ระบบจะส่งเป็นประกาศ ถึงผู้ใช้งานทุกคนในระบบ
</div>

<div class="warning">

การแนบ URL มี 2 รูปแบบ ได้แก่
1. `ภายใน` จะต้องมีเครื่องหมาย `#` นำหน้า เช่น `#/info`
1. `ภายนอก`  จะต้องเป็น URL ที่ถูกต้องตามมาตรฐาน นำหน้าด้วย `http://` หรือ `https://`
</div>

<div class="warning">

ปุ่ม <i class="fas fa-wand-magic-sparkles" style="color:orange;"></i> ในการแนบ URL  
จะสำเนาที่ตั้ง (URL) ปัจจุบันของโปรแกรม ให้โดยอัตโนมัติ
</div>

## การจัดการข้อความ
![Message Messages](images/message-messages.webp)

* <i class="fa-regular fa-envelope" style="color:red;"></i> : ข้อความที่ `ยังไม่ได้อ่าน`
* <i class="fa-regular fa-envelope" style="color:orange;"></i> : ข้อความที่ `อ่านแล้ว`
* `GO` : ไปยัง URL ที่แนบ
* <i class="fas fa-reply" style="color:orange;"></i> : ตอบกลับ
* <i class="fa-regular fa-circle-check" style="color:orange;"></i> : กำหนดว่า `อ่านแล้ว`

ปุ่มด้านล่าง
* <i class="fa-regular fa-circle-check" style="color:orange;"></i> `ทั้งหมด` : กำหนดว่า `อ่านแล้ว` ทั้งหมดทุกหัวข้อ
* <i class="fa-regular fa-circle-check" style="color:orange;"></i> `ประกาศ` : กำหนดว่า `อ่านแล้ว` ทั้งหมดในหัวข้อ `ประกาศ`
* <i class="fas fa-arrows-rotate" style="color:orange;"></i> `ย้อนหลัง..` : โหลดข้อความเก่า

<div class="warning">

การกดปุ่ม `GO` หรือ ตอบกลับด้วยปุ่ม <i class="fas fa-reply" style="color:orange;"></i>  
จะถือว่า `อ่านแล้ว` โดยอัตโนมัติ
</div>

## การตอบกลับ
การตอบกลับ สามารถอ้างอิงข้อความได้เพียง 1 ชั้น เช่น User อ้างอิงข้อความของ Test User ในการตอบกลับ  
ส่งไปหา TEST DOCTOR ดังรูป

![Message Compose Ref](images/message-compose-ref.webp)

TEST DOCTOR จะได้รับข้อความ ดังรูป

![Message Ref](images/message-ref.webp)