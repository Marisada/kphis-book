# ระบบงานผู้ป่วยใน (IPD)

## ขั้นตอนเตรียมความพร้อม
- กำหนด [ชุดข้อมูลทางการพยาบาล (Template Nurse)](../other/template-nurse.md)
- กำหนด [Order ล่วงหน้า](pre-order.md) ประเภท `Shared Template`

## กระบวนการบริการ
### แรกรับ
* บันทึก `Admit` ใน HOSxP
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
- [บันทึกการสรุปเวชระเบียน (In-Patient Summary)](summary.md)
- [จัดทำเอกสาร](ipd/document.md)

## การนัดเพื่อ Admit
- กำหนด [Order ล่วงหน้า](ipd/pre-order.md) ประเภท `Admit ล่วงหน้า`
- เมื่อถึงวันนัด ให้เปิด `Visit` และ `Admit` ใน HOSxP
- เปิดเมนู [รายการผู้ป่วยใน](search-patient.md) <i class="fa fa-arrow-circle-right"></i> เลือกผู้ป่วย <i class="fa fa-arrow-circle-right"></i> กดปุ่ม [Order](order.md) <i class="fa fa-arrow-circle-right"></i> กดปุ่ม `เลือกใบ Order`
