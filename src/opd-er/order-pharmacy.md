# ระบบรอรับใบสั่งยา (เภสัชกรรม)

![OPD-ER Order Pharmacy Head](images/opd-er-order-pharmacy-head.webp)

การตั้งค่า ระบบรอรับใบสั่งยาผู้ป่วยนอก ประกอบด้วย
* `วันที่ Order ตั้งแต่ .. ถึงวันที่ ..` : แสดงเฉพาะ Order ในช่วงวันที่กำหนด
* `รอบการ Update` : กำหนดเวลา ที่ระบบจะค้นหาซ้ำ เช่น ค้นหาทุก 1 นาที เป็นต้น
* `ยา/สารน้ำ/Nurse's Order ที่ยังไม่ได้ตรวจสอบ` : แสดงเฉพาะ Order ที่เป็น ยา หรือสารน้ำ หรือสั่งโดยพยาบาล ที่เภสัชกรยังไม่ได้รับรายการ
* `HN, VN, ชื่อ-สกุล` : แสดงเฉพาะผู้ป่วยที่กำหนด ด้วยการกรอก HN, VN หรือชื่อ-สกุล ผู้ป่วย อย่างใดอย่างหนึ่ง
* <i class="fas fa-magnifying-glass" style="color:orange;"></i> `ค้นหา` : สั่งการค้นหา
* <i class="fas fa-volume-xmark" style="color:orange;"></i>`x` : เสียงเรียกถูกปิดไว้
* <i class="fas fa-volume-high" style="color:orange;"></i> : เสียงเรียกพร้อมใช้งาน
* <i class="fas fa-play" style="color:orange;"></i> `Test` : ทดสอบเสียงเรียก

![OPD-ER Order Pharmacy Data](images/opd-er-order-pharmacy-data.webp)

ผลจากการค้นหา ประกอบด้วย 2 ส่วน ได้แก่
* `รายการ Order ใหม่` : แสดงข้อมูลผู้ป่วยที่มี Order ใหม่ ร่วมกับข้อมูล
    1. `เวลา Order` น้อยที่สุด - มากที่สุด ในช่วง `วันที่ Order ตั้งแต่ .. ถึงวันที่ ..` ที่กำหนด
    2. เป็นรายการยา/สารน้ำ หรือไม่
    3. `Priority` : แสดงสถานะ และหมายเหตุ ยา Stat หรือ Home-Med (ถ้ามี)
        - <i class="fa-regular fa-envelope" style="color:orange;"></i> : จำนวน Order ที่เภสัชกรยังไม่รับรายการ
        - <i class="fa-regular fa-pen-to-square" style="color:orange;"></i> : จำนวน Order ที่เภสัชกรรับรายการแล้ว
        - <i class="fa-regular fa-circle-check" style="color:orange;"></i> : จำนวน Order ที่เภสัชกรตรวจสอบแล้ว

    <div class="warning">

    Stat Order ที่เภสัชกรยังไม่รับรายการ จะแสดงแถบสี`ชมพู` เพื่อเตือนเภสัชกร  
    Order อื่น ที่เภสัชกรยังไม่รับรายการ จะแสดงแถบสี`เหลือง`  
    Order ที่เภสัชกรรับรายการแล้ว (รอตรวจสอบ) จะแสดงแถบสี`ฟ้า`  
    Order ที่เภสัชกรตรวจสอบแล้ว จะไม่มีแถบสี 
    </div>

* `ผู้ป่วยที่อยู่ที่ ER แต่ไม่มี Order ใหม่ในช่วงเวลาที่เลือก` : แสดงรายการผู้ป่วยที่ไม่มี Order ใหม่ ในช่วง `วันที่ Order ตั้งแต่ .. ถึงวันที่ ..` ที่กำหนด ท่านสามารถคลิกที่รายการ เพื่อไปดูใบ Order ของผู้ป่วยได้