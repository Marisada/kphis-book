# Order ล่วงหน้า

![Pre Order List](images/pre-order-list.webp)

## การสร้าง Order ล่วงหน้า ใหม่
ด้วยการกดปุ่ม `+ เพิ่มใบ Order ใหม่` แล้วเลือกประเภทใบ Order ที่ต้องการ

1. `Admit ล่วงหน้า` : คือใบ Order ที่สร้างไว้ล่วงหน้า เฉพาะสำหรับผู้ป่วยที่ระบุไว้ เพื่อ `Admit` ใน `วันที่นัดหมาย`
1. `Admit ในวัน` : คือใบ Order ที่สร้างไว้ล่วงหน้า เฉพาะสำหรับผู้ป่วยที่ระบุไว้ เพื่อ `Admit` ใน `วันนี้`

    ![Pre Order New](images/pre-order-new.webp)

    * กดปุ่ม <i class="fa fa-search"></i> เพื่อค้นหาผู้ป่วยที่ต้องการ
    * เลือกวันนัด `Admit` (ประเภท `Admit ในวัน` จะระบุเป็น `วันนี้` โดยอัตโนมัติ)
    * กดปุ่ม `บันทึก`

1. `Template` : คือ Standing Order ที่กำหนด Order และ Progress Note ไว้ล่วงหน้า ผู้ใช้งานสามารถนำไปวางใน Order ได้ตามต้องการ

    ![Pre Order New Template](images/pre-order-new-template.webp)

    * ตั้งชื่อ `Template` ตามต้องการ 
    * กดปุ่ม `บันทึก`

    <div class="warning">
    
    ชื่อ `Template` ควรเป็นชื่อที่สั้นและเข้าใจง่าย เช่น `แก้ HyperK ชุดใหญ่`  
    หรือกำหนดโครงสร้างของชื่อ เพื่อใช้ร่วมกันในโรงพยาบาล  
    เช่น `[PED] Septic work-up`, `[MED] Septic work-up` เป็นต้น
    </div>

<div class="warning">

`Order ล่วงหน้า` โดยทั่วไป จะสามารถใช้ได้เฉพาะผู้ที่สร้างเท่านั้น  
มีเฉพาะ `Template` ที่กำหนดเป็น `Shared Template` เท่านั้น  
ที่เจ้าหน้าที่ท่านอื่นจะสามารถนำไปใช้ได้
</div>