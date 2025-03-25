# ระบบงานผู้ป่วยใน (IPD)

## ขั้นตอนเตรียมความพร้อม
- กำหนด [Template การบันทึกทางการพยาบาล (Focus Charting)](../other/template-nurse.md) ในรูปแบบ Assessment Intervention Evaluation (AIE) ให้ครอบคลุมทุกกลุ่มโรค
- กำหนด [Order ล่วงหน้า](pre-order.md) ประเภท `Shared Template` เป็น Standing Order ตามแนวทางเวชปฏิบัติ

## กระบวนการบริการ
### แรกรับ
1. ใช้ระบบ `รอ Admit`
    * เปิดเมนู `รอ Admit`
    * กดปุ่ม `เพิ่มใบ Order ใหม่`
    * กดปุ่ม <i class="fa fa-search"></i> เพื่อค้นหา Visit ที่ต้องการ แล้วกดปุ่ม `บันทึก`
    * เลือกผู้ป่วยที่ต้องการ เพื่อ [บันทึกประวัติและตรวจร่างกายแรกรับ](admission-note-dr.md) และ [บันทึกคำสั่งแพทย์](order.md) ต่อไป
    * บันทึก `Admit` ใน HOSxP

    <div class="warning">

    ในระบบ `รอ Admit` แพทย์สามารถเลือกผู้ป่วยที่เปิด Visit แล้ว เพื่อบันทึกประวัติ และคำสั่งแพทย์ได้โดยไม่ต้อง `Admit` ใน HOSxP ก่อน
    
    หลังจากเจ้าหน้าที่ `Admit` ใน HOSxP แล้ว ระบบจะย้ายข้อมูลผู้ป่วย จากประเภท `รอ Admit` เป็นประเภท `Admit แล้ว`
    </div>

1. ใช้ระบบ KPHIS ดั้งเดิม
    * บันทึก `Admit` ใน HOSxP
    * เปิดเมนู `รายการผู้ป่วยใน` และค้นหาผู้ป่วยที่ต้องการ เพื่อ [บันทึกประวัติและตรวจร่างกายแรกรับ](admission-note-dr.md) และ [บันทึกคำสั่งแพทย์](order.md) ต่อไป

    <div class="warning">

    ในระบบ KPHIS ดั้งเดิม เมนู `รายการผู้ป่วยใน` จะแสดงเฉพาะผู้ป่วยที่ `Admit` ใน HOSxP เรียบร้อยแล้ว และยังไม่จำหน่ายเท่านั้น

    แพทย์จะต้องรอให้เจ้าหน้าที่ ทำการ `Admit` ใน HOSxP ก่อน ถึงจะบันทึกประวัติ และคำสั่งแพทย์ได้  
    </div>

* แพทย์
    - [บันทึกประวัติและตรวจร่างกายแรกรับ](admission-note-dr.md)
    - [บันทึกคำสั่งแพทย์](order.md)
* เภสัชกร/แพทย์
    - [บันทึกการทบทวนยา (Medical Reconciliation)](med-reconciliation.md) 
* พยาบาล
    - [ประเมินสภาพผู้ป่วยแรกรับและแบบแผนสุขภาพ](admission-note-nurse.md)
    - [ระบุแพทย์เจ้าของไข้](doctor-in-charge.md)

### การบันทึกประจำวัน/เวร
* พยาบาล
    - [บันทึกปัญหาทางการพยาบาล (Focus List)](../shared/focus-list.md)
    - [บันทึกความก้าวหน้าทางการพยาบาล (Nurse Note)](../shared/focus-note.md)
* เจ้าหน้าที่
    - [บันทึกสัญญาณชีพ](../shared/vital-sign.md)
    - [บันทึกสมดุลน้ำ (Intake-Output: I/O)](../shared/io.md)

### การรักษาพยาบาล
* แพทย์
    - [บันทึกคำสั่งแพทย์](order.md)
    - [ขอคำปรึกษา (Consult)](consult.md)
* พยาบาล
    - รับ Order ตาม [บันทึกคำสั่งแพทย์](order.md)
    - [บันทึกแผนและกิจกรรมทางการพยาบาล (Index Plan/Action)](../shared/index-plan.md)
* เภสัชกร
    - [รอรับใบสั่งยา](order-pharmacy.md)
    - บันทึกจ่ายยา ใน HOSxP
    - จ่ายยา ใน [บันทึกคำสั่งแพทย์](order.md)
    - ยืนยันการจ่ายยา ใน [บันทึกคำสั่งแพทย์](order.md)

### เครื่องมือทำงาน
- [แสดงผลการตรวจทางห้องปฏิบัติการ จาก HOSxP](shared/lab.md)
- [เวชระเบียนอิเล็กทรอนิกส์ (Electronic Medical Record:EMR)](shared/emr.md)
- [ระบบ Screen ใบสั่งยา และค้นประวัติการสั่งยาใน HOSxP](shared/prescription-screen.md)
- [เอกสาร Antibiogram](shared/antibiogram.md)
- [ทางลัดสู่ระบบภายนอก](shared/out-source.md)

### หลังจำหน่าย
- [สรุป Chart](post-admit.md)
- [บันทึกการสรุปเวชระเบียน (In-Patient Summary)](summary.md)
- [จัดทำเอกสาร](document.md)

## การสร้างใบ Order ไว้ล่วงหน้า เพื่อ Admit ใน Visit อื่น
- สร้าง [Order ล่วงหน้า](pre-order.md) ประเภท `Admit ล่วงหน้า`
- เมื่อถึงวันนัด ให้เปิด `Visit` ตามปกติ
- ดำเนินการในระบบ [แรกรับ](#แรกรับ)
- เลือกผู้ป่วย <i class="fa fa-arrow-circle-right"></i> กดปุ่ม [Order](order.md) <i class="fa fa-arrow-circle-right"></i> กดปุ่ม `เลือกใบ Order` <i class="fa fa-arrow-circle-right"></i> กดปุ่ม `ใช้งาน`
