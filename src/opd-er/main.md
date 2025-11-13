# แฟ้มผู้ป่วย ER

## ข้อมูลแฟ้มผู้ป่วย
![OPD-ER Order Top](images/opd-er-main-top.webp)

ท่านสามารถแก้ไข `Visit`, `เตียง`, `สถานะ` และ `Note` ได้ตามต้องการ

กรณี Discharge แล้ว
<!-- ANCHOR: opd-er-discharge -->
![OPD-ER Order Top Discharged](images/opd-er-main-top-discharged.webp)

ให้บันทึก `ประเภทการ Discharge` และ `วันที่จำหน่าย` เพิ่มเติม

เมื่อแก้ไขเรียบร้อยแล้ว กดปุ่ม `บันทึก`
<div class="warning">

ท่านสามารถคลิกที่ <i class="fa fa-clock-o" style="color:orange;"></i>  
เพื่อเลือกวันที่และเวลาปัจจุบัน
</div>

<!-- ANCHOR_END: opd-er-discharge -->

## สถานะผู้ป่วย
![OPD-ER Status](images/opd-er-status.webp)

เมื่อแก้ไขเรียบร้อยแล้ว กดปุ่ม `บันทึก`

## ระบบงานย่อยในแฟ้มผู้ป่วย
![OPD-ER Order Tab](images/opd-er-main-tab.webp)
* [ประวัติผู้ป่วย](medical-history.md) : แสดงประวัติใน HOSxP, บันทึก Trauma care (ABCDE)
* [Med Reconciliation](../shared/med-reconciliation.md) : ทบทวนยาเดิมผู้ป่วย ทั้งจากข้อมูล HOSxP และบันทึกเพิ่มเองได้
* [Order](../shared/order.md) : บันทึก Order และ Progress Note
* [Vital Sign](../shared/vital-sign.md) : บันทึก Vital Sign, แสดงกราฟสัญญาณชีพ
* [I/O](../shared/io.md) : บันทึกสมดุลน้ำ
* [Nursing Progress Note](../shared/focus-note.md) : แสดงความก้าวหน้าทางการพยาบาล, [บันทึกปัญหาทางการพยาบาล (Focus List)](../shared/focus-list.md), [บันทึกความก้าวหน้าทางการพยาบาล (Nurse Note)](..shared/focus-note.md) และ  [บันทึกแผนการจำหน่าย (Discharge Plan)](../shared/discharge-plan.md)
* [Nurse Planning](../shared/index-plan.md) : บันทึกแผนและกิจกรรมทางการพยาบาล (Index Plan/Action)
* [Lab](../shared/lab.md) : แสดงผลการตรวจทางห้องปฏิบัติการ จาก HOSxP
* [X-Ray <i class="fa fa-external-link"></i>](../shared/out-source.md) : ไปสู่ระบบ PACs (โปรแกรมภายนอก, ถ้ามี)
* [EKG <i class="fa fa-external-link"></i>](../shared/out-source.md) : ไปสู่ระบบบันทึก EKG (โปรแกรมภายนอก, ถ้ามี)
* [Scan <i class="fa fa-external-link"></i>](../shared/out-source.md) : ไปสู่ระบบภาพ Scan (โปรแกรมภายนอก, ถ้ามี)
* [ประวัติการสั่งยา](../shared/prescription-screen.md) : ระบบ Screen ใบสั่งยา (ประวัติการสั่งยาใน HOSxP)
* [EMR](../shared/emr.md) : แสดงประวัติการรักษา (Electronic Medical Record: EMR)
* [เอกสาร](document.md) : แสดงและจัดพิมพ์เอกสารทางการแพทย์
* [ขอเปล <i class="fa fa-external-link"></i>](../shared/out-source.md) : ไปสู่ระบบขอเปล (โปรแกรมภายนอก, ถ้ามี)
* [Antibiogram <i class="fa fa-file-pdf-o"></i>](../shared/antibiogram.md) : แสดงข้อมูลการดื้อยา (Antibiogram)