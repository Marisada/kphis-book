# การปรับปรุงต้นฉบับ

## ภาษาที่เกี่ยวข้อง
หนังสือเล่มนี้ ใช้ภาษา [Markdown](https://en.wikipedia.org/wiki/Markdown) ในการเขียน และแปลงเป็น Web Page ด้วย [mdBook](https://rust-lang.github.io/mdBook) ซึ่งภาษา Markdown ที่ mdBook ใช้นั้น อ้างอิงตาม [CommonMark](https://commonmark.org/) ซึ่งท่านสามารถศึกษาเพิ่มเติมได้ที่ [tutorial](https://commonmark.org/help/tutorial/) หรือทดลองได้ที่ [dingus](https://spec.commonmark.org/dingus/) หรือศึกษารายละเอียดได้ที่ [Markdown Guide](https://www.markdownguide.org/)

การแสดง Web page ของหนังสือเล่มนี้ ทาง mdBook มีคู่มือการใช้งานที่เกี่ยวข้อง ได้แก่
* สร้างเมนูด้านซ้าย ด้วย [SUMMARY.md](https://rust-lang.github.io/mdBook/format/summary.html)
* สร้างสูตรคณิตศาสตร์ ด้วย [MathJax](https://rust-lang.github.io/mdBook/format/mathjax.html)
* ความสามารถพิเศษ ของ mdBook ([mdBook-specific features](https://rust-lang.github.io/mdBook/format/mdbook.html))

บทความภาษาไทย อ่านได้ที่ [วิธีการเขียนภาษา Markdown บน mdBook](markdown.md)

---

## การแก้ไขเอกสารต้นฉบับ
ไฟล์เอกสารต้นฉบับ อยู่ใน [GitHub](https://github.com) ซึ่งท่านสามารถอ่านวิธีการส่งเอกสารต้นฉบับได้ที่ [Contributing to a project on GitHub](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project)

### แก้ไขบนเวปไซต์ [GitHub](https://github.com)
* หากยังไม่มี GitHub account ท่านสามารถสมัครได้ฟรี ที่ <https://github.com/signup>
* สร้างสำเนา(Fork) ของท่านเอง ด้วยการกดปุ่ม `Fork` แล้วกดปุ่ม `Create fork`
* ไปที่สำเนาของท่าน เช่น `https://github.com/<ชื่อ GitHub ของท่าน>/kphis-book`
* สร้างสาขา(ฺฺBranch) ใหม่ เพื่อแก้ไขเอกสาร ด้วยการกดที่ `Branches` แล้วกดปุ่ม `New branch`
* แก้ไขไฟล์ที่ต้องการ ใน Branch ของท่าน ด้วยการเลือกไฟล์ที่ต้องการ และแก้ไขใน Web Browser
* ส่งการแก้ไขของท่าน เพื่อมารวม (Merge) กับข้อมูลหลัก ด้วยการกดที่ปุ่ม `Contribute` แล้วกดปุ่ม `Open pull request`
* กรอกรายละเอียดการแก้ไข เพื่อให้เราสามารถมองเห็นความสำคัญของการแก้ไขนี้ได้ หากเรียบร้อยแล้ว กดปุ่ม `Create pull request`
* รอทีมงานของเรา ในการดำเนินการรวม (Merge) การแก้ไขของท่านต่อไป

### แก้ไขบนเครื่องตนเอง
* ติดตั้ง [Git](https://git-scm.com/) หากต้องการใช้คำสั่ง `git` บน `cmd` หรือติดตั้ง [GitHub Desktop](https://github.com/apps/desktop) สำหรับการใช้งานบน Application (ใช้คำสั่ง `git` บน `cmd` ไม่ได้) หรือเลือกติดตั้งทั้ง 2 อย่างก็ได้
* หากยังไม่มี GitHub account ท่านสามารถสมัครได้ฟรี ที่ <https://github.com/signup>
* สร้างสำเนาของท่านเอง ด้วยการกดปุ่ม `Fork` แล้วกดปุ่ม `Create fork`
* สำเนา (Clone) ไฟล์ทั้งหมดมาที่เครื่องของท่าน ได้ 3 วิธี ได้แก่
    1. GitHub : คลิกที่ปุ่ม `Code` แล้วเลือก `Download ZIP` แตกไฟล์แล้ววางในที่ที่ต้องการ
    1. git shell 
        ```bash
        git clone https://github.com/<ชื่อ GitHub ของท่าน>/kphis-book
        ```
    1. GitHub Desktop
        * กดปุ่ม `Add` และเลือก `Clone repository...`  
        * ในส่วน `Github.com` เลือก `<ชื่อ GitHub ของท่าน>/kphis-book` แล้วกดปุ่ม `Clone`
* สร้างสาขา (Branch) ทำได้ 2 วิธี
    1. git shell
        ```bash
        git branch BRANCH-NAME
        git checkout BRANCH-NAME
        ```
    1. GitHub Desktop
        * คลิกที่ `Current branch` กรอกชื่อสาขาใหม่ แล้วกดปุ่ม `New branch`
* แก้ไขไฟล์ที่ต้องการ ด้วย code editor ที่ท่านชื่นชอบ เช่น [Visual Studio Code](https://code.visualstudio.com/), [NotePad++](https://notepad-plus-plus.org/), [Zed](https://zed.dev/), [Helix](https://helix-editor.vercel.app/), [Vim](https://www.vim.org/) และ [NeoVim](https://neovim.io/) เป็นต้น
* บันทึกการแก้ไข ไปยัง GitHub ของท่าน ทำได้ 2 วิธี ได้แก่
    1. git shell 
        ```bash
        git add .
        git commit -m "ประเด็นแก้ไขของคุณ"
        git push
        ```
    1. GitHub Desktop
        * พิมพ์ `Summary (required)` และ `Description` (ถ้ามี) แล้วกดปุ่ม `Commit to main`
* ไปที่ `https://github.com/<ชื่อ GitHub ของท่าน>/kphis-book`
* ส่งการแก้ไขของท่าน เพื่อมารวม (Merge) กับข้อมูลหลัก ด้วยการกดที่ปุ่ม `Contribute` แล้วกดปุ่ม `Open pull request`
* กรอกรายละเอียดการแก้ไข เพื่อให้เราสามารถมองเห็นความสำคัญของการแก้ไขนี้ได้ หากเรียบร้อยแล้ว กดปุ่ม `Create pull request`
* รอทีมงานของเรา ในการดำเนินการรวม (Merge) การแก้ไขของท่านต่อไป

### ชื่นชมผลงานของท่าน
* ติดตั้ง [mdBook](https://rust-lang.github.io/mdBook/guide/installation.html), เปิด terminal แล้วไปที่ `../kphis-book/` และใช้คำสั่ง 
    ```bash
    mdbook build --open
    ``` 
* <https://marisada.github.io/kphis-book/>
* `https://<ชื่อ GitHub ของท่าน>.github.io/kphis-book/`
