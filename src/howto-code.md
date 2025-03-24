# เตรียมพร้อมเขียนหนังสือ
ไฟล์เอกสารต้นฉบับ `kphis-book` อยู่บนระบบ [GitHub](https://github.com) ที่เป็นระบบสำหรับนักพัฒนาโปรแกรมคอมพิวเตอร์ ในการเก็บไฟล์ต้นฉบับ การจัดทำ version และมีเครื่องมือสำหรับทีมงานพัฒนา เช่น กระดานรับปัญหา (Issues), การทบทวนและตรวจสอบ รวมถึงการสร้างเวปเพจฟรีให้ท่าน โดยไม่มีค่าใช้จ่าย ซึ่งท่านสามารถอ่านวิธีการพัฒนาโปรแกรมบน GitHub ได้ที่ [Contributing to a project on GitHub](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project)

สิ่งที่ควรมี ได้แก่
* คอมพิวเตอร์สักเครื่อง
* ความรู้เกี่ยวกับคอมพิวเตอร์เบื้องต้น เช่น การค้นหาไฟล์, การเปิดและแก้ไขไฟล์, การค้นหาโปรแกรม, การติดตั้งและถอนการติดตั้งโปรแกรม เป็นต้น
* ความรู้เกี่ยวกับ Terminal เบื้องต้น (`Command Prompt` บน Windows หรือ `Terminal` บน Linux และ MacOS) เช่น คำสั่ง `cd`, `dir` เป็นต้น

## การแก้ไขบนเวปไซต์ [GitHub](https://github.com)
* หากยังไม่มี GitHub account ท่านสามารถสมัครได้ฟรี ที่ <https://github.com/signup>
* สร้างสำเนา(Fork) ของท่านเอง ด้วยการกดปุ่ม `Fork` แล้วกดปุ่ม `Create fork`
* ไปที่สำเนาของท่าน เช่น `https://github.com/<ชื่อ GitHub ของท่าน>/kphis-book`
* สร้างสาขา(ฺฺBranch) ใหม่ เพื่อแก้ไขเอกสาร ด้วยการกดที่ `Branches` แล้วกดปุ่ม `New branch`
* แก้ไขไฟล์ที่ต้องการ ใน Branch ของท่าน ด้วยการเลือกไฟล์ที่ต้องการ และแก้ไขใน Web Browser
* ส่งการแก้ไขของท่าน เพื่อมารวม (Merge) กับข้อมูลหลัก ด้วยการกดที่ปุ่ม `Contribute` แล้วกดปุ่ม `Open pull request`
* กรอกรายละเอียดการแก้ไข เพื่อให้เราสามารถมองเห็นความสำคัญของการแก้ไขนี้ได้ หากเรียบร้อยแล้ว กดปุ่ม `Create pull request`
* รอทีมงานของเรา ในการดำเนินการรวม (Merge) การแก้ไขของท่านต่อไป

## การแก้ไขบนเครื่องตนเอง
* เปิดโปรแกรมป้อนคำสั่ง ด้วยการค้นหาในระบบปฏิบัติการด้วยคำว่า `terminal` เพื่อเปิดโปรแกรม `Command Prompt` ใน Windows, `Terminal` ใน Linux หรือ MacOS
* ติดตั้ง [Git](https://git-scm.com/) หากต้องการใช้คำสั่ง `git` บน `terminal` หรือติดตั้ง [GitHub Desktop](https://github.com/apps/desktop) สำหรับการใช้งานบน Application (ใช้คำสั่ง `git` บน `terminal` ไม่ได้) หรือเลือกติดตั้งทั้ง 2 อย่างก็ได้
* หากยังไม่มี GitHub account ท่านสามารถสมัครได้ฟรี ที่ <https://github.com/signup>
* สร้างสำเนาของท่านเอง ด้วยการกดปุ่ม `Fork` แล้วกดปุ่ม `Create fork`
* สำเนา (Clone) ไฟล์ทั้งหมดมาที่เครื่องของท่าน ทำได้ 3 วิธี ได้แก่
    1. เพจ GitHub ของท่าน: คลิกที่ปุ่ม `Code` แล้วเลือก `Download ZIP` แตกไฟล์แล้ววางในที่ที่ต้องการ
    1. git shell ใน `terminal`
        ```bash
        git clone https://github.com/<ชื่อ GitHub ของท่าน>/kphis-book
        ```
    1. GitHub Desktop
        * กดปุ่ม `Add` และเลือก `Clone repository...`  
        * ในหัวข้อ `GitHub.com` เลือก `<ชื่อ GitHub ของท่าน>/kphis-book` แล้วกดปุ่ม `Clone`
* สร้างสาขา (Branch) ทำได้ 3 วิธี
    1. เพจ GitHub ของท่าน: คลิกที่ปุ่ม `Branch` แล้วเลือก `New branch` เพื่อสร้าง `New branch name` จาก `main` Source
    1. git shell ใน `terminal`
        ```bash
        git branch BRANCH-NAME
        git checkout BRANCH-NAME
        ```
    1. GitHub Desktop
        * คลิกที่ `Current branch` กรอกชื่อสาขาใหม่ แล้วกดปุ่ม `New branch`
* เปิด Hot Reload ด้วย `mdbook watch`  
    ท่านสามารถสร้างหน้าเพจอัตโนมัติทุกครั้งที่บันทึกการแก้ไขไฟล์ต้นฉบับได้ ด้วยคำสั่ง `mdbook watch` ดังนี้
    1. เปิด `terminal` และใช้คำสั่ง `cd` เพื่อไปยัง folder ของ `kphis-book` ที่ได้ clone ไว้
        * Windows
            ```bat
            c:
            cd %UserProfile%\Documents\GitHub\kphis-book
            ```
        * Linux
            ```bash
            cd $HOME/github/kphis-book
            ```
    1. ใช้คำสั่ง `watch` ของ mdBook 
        ```bash
        mdbook watch -o
        ```
        โปรแกรมจะเปิด Web Browser ให้ท่านพร้อมแสดงตัวอย่างเพจจากไฟล์บนเครื่องของท่านให้  
        และทุกครั้งที่ท่านบันทึกการแก้ไขไฟล์ใน `/kphis-book/src` ตัว Web Browser จะโหลดหน้าเพจให้ท่านใหม่อัตโนมัติ
* แก้ไขไฟล์ที่ต้องการ ด้วย code editor ที่รองรับการเขียนภาษา Markdown เช่น [Visual Studio Code](https://code.visualstudio.com/), [NotePad++](https://notepad-plus-plus.org/), [Zed](https://zed.dev/), [Helix](https://helix-editor.vercel.app/), [Vim](https://www.vim.org/) หรือ [NeoVim](https://neovim.io/) เป็นต้น
* ส่งการแก้ไข ไปยัง GitHub ของท่าน ทำได้ 2 วิธี ได้แก่
    1. git shell ใน `terminal`
        ```bash
        git add .
        git commit -m "ประเด็นแก้ไขของคุณ"
        git push
        ```
    1. GitHub Desktop
        * พิมพ์ `Summary (required)` และ `Description` (ถ้ามี) แล้วกดปุ่ม `Commit to main`
* ไปที่ `https://github.com/<ชื่อ GitHub ของท่าน>/kphis-book`
* ส่งการแก้ไขใน GitHub เพื่อมารวม (Merge) กับ GitHub หลัก ด้วยการกดที่ปุ่ม `Contribute` แล้วกดปุ่ม `Open pull request`
* กรอกรายละเอียดการแก้ไข เพื่อให้เราทราบความสำคัญของการแก้ไขในครั้งนี้ แล้วกดปุ่ม `Create pull request`
* รอทีมงานดำเนินการรวม (Merge) การแก้ไขของท่านต่อไป

## Continuous Integration (CI) and Continuous Delivery/Deployment (CD)
ทาง GitHub มีระบบ CI/CD ที่เรียกว่า GitHub Action ที่จะทำการแปลงไฟล์ต้นฉบับ ให้เป็นเพจให้ท่านโดยอัตโนมัติ ทุกครั้งที่ท่าน `Commit to main`  
โดยขั้นตอนที่ GitHub Action ทำให้ท่าน ประกอบด้วย
* สร้างเครื่อง Builder พร้อมติดตั้ง `mdBook` และสำเนาไฟล์ต้นฉบับ `kphis-book` ของท่าน
* เรียกคำสั่ง `mdbook build`
* ส่งไฟล์ Web Page ที่สร้างสำเร็จ ขึ้นสู่ `https://<ชื่อ GitHub ของท่าน>.github.io/kphis-book/`

## ชื่นชมผลงานของท่าน
* บนเครื่องของท่าน ด้วยการติดตั้ง [mdBook](https://rust-lang.github.io/mdBook/guide/installation.html), เปิด `terminal` แล้วไปที่ folder `kphis-book` และใช้คำสั่ง 
    ```bash
    mdbook build --open
    ``` 
* `https://<ชื่อ GitHub ของท่าน>.github.io/kphis-book/` เช่น https://marisada.github.io/kphis-book/