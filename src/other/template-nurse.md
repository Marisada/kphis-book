# Template การบันทึกทางการพยาบาล (Focus Charting)
ในระบบ FAIE (Focus Assessment Intervention Evaluation) ประกอบด้วย
* ประเด็นสำคัญ หรือ ปัญหา (Focus)
* การประเมินผู้ป่วยแรกรับ (Assessment)
* การบันทึกกิจกรรมการพยาบาล (Intervention)
* การประเมินผลการพยาบาล (Evaluation)

ใน KPHIS จัดระบบการบันทึกทางการพยาบาล โดยเพิ่ม
* กลุ่มอาการ (Group)
* กลุ่มอาการ กลุ่มย่อย (Subgroup)
* เป้าหมาย (Goal)
* Daily Care 

![Template Nurse Start](images/template-nurse-start.webp)

1. `กลุ่มอาการ (Group)` ประกอบด้วย หลาย `กลุ่มอาการ กลุ่มย่อย (Subgroup)`

1. `กลุ่มอาการ กลุ่มย่อย (Subgroup)` มี 2 ประเภท ได้แก่
    * `ไม่ระบุ(แสดงเสมอ)` : เมื่อเลือก `กลุ่มอาการ (Group)` ของกลุ่มย่อยนี้ จะแสดง `ปัญหา (Focus)` + `เป้าหมาย (Goal)` + `Intervention` ของกลุ่มย่อยนี้โดยอัตโนมัติ
    * `ระบุชื่อ` : เพื่อแบ่งกลุ่มอาการ เป็นกลุ่มย่อย (Subgroup)

    ![Template Nurse Subgroup](images/template-nurse-subgroup-start.webp)
    ![Template Nurse Subgroup Always](images/template-nurse-subgroup-always.webp)
    <div class="warning">

    ประเภท `ไม่ระบุ(แสดงเสมอ)` ช่วยให้ท่านสามารถเลือก `ปัญหา (Focus)` + `เป้าหมาย (Goal)` + `Intervention` ได้โดยอัตโนมัติ ในทุกๆ `ปัญหา (Focus)` ที่ตรงกับ `กลุ่มอาการ (Group)` 

    เช่น  `กลุ่มอาการ (Group)` ไข้ มี
    - `ไม่ระบุ(แสดงเสมอ)` ที่มี `ปัญหา (Focus)` F-A, `เป้าหมาย (Goal)` G-A และ `Intervention` I-A
    - `ระบุชื่อ` <u>หนาวสั่น</u> ทีมี `ปัญหา (Focus)` F-X, `เป้าหมาย (Goal)` G-X และ `Intervention` I-X
    - `ระบุชื่อ` <u>ซึม</u> ทีมี `ปัญหา (Focus)` F-Y, `เป้าหมาย (Goal)` G-Y และ `Intervention` I-Y
    หากเลือก `ปัญหา (Focus)` F-X จะแสดง `เป้าหมาย (Goal)` G-X และ G-A  
    หากเลือก `ปัญหา (Focus)` F-Y จะแสดง `เป้าหมาย (Goal)` G-Y และ G-A 
    </div>

1. ในแต่ละ `กลุ่มอาการ กลุ่มย่อย (Subgroup)` จะประกอบไปด้วย `ปัญหา (Focus)` + `เป้าหมาย (Goal)` + `Intervention` ประจำกลุ่มย่อย

    ![Template Nurse Focus](images/template-nurse-focus.webp)
    ![Template Nurse Goal](images/template-nurse-goal.webp)
    ![Template Nurse Intvt](images/template-nurse-intvt.webp)
1. `Daily Care` จะแสดงตลอดเวลา ไม่เกี่ยวข้องกับ `กลุ่มอาการ (Group)`, `กลุ่มอาการ กลุ่มย่อย (Subgroup)`, `ปัญหา (Focus)`, `เป้าหมาย (Goal)` หรือ `Intervention`

## การเพิ่ม หรือแก้ไข
ด้วยการกดปุ่ม `+ เพิ่ม` เพื่อสร้างรายการใหม่ หรือกดปุ่ม <i class="fa fa-pencil-square-o"></i> เพื่อแก้ไข
* `ยกเลิกการใช้งาน` ทำไม่ไม่สามารถใช้รายการนี้ได้ จนกว่าจะเปลี่ยนเป็น `ยังใช้งานอยู่`
* `Delete` ลบรายการ (หากถูกใช้งานแล้ว จะไม่สามารถลบได้)

    ![Template Nurse Group Edit](images/template-nurse-group-edit.webp)
    ![Template Nurse Subgroup Edit](images/template-nurse-subgroup-edit.webp)
    ![Template Nurse Focus Edit](images/template-nurse-focus-edit.webp)
    ![Template Nurse Goal Edit](images/template-nurse-goal-edit.webp)
    ![Template Nurse Intvt Edit](images/template-nurse-intvt-edit.webp)
    ![Template Nurse Dlc Edit](images/template-nurse-dlc-edit.webp)