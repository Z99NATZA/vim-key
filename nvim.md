# Neovim keymaps

## Leader `\`

| Key | การทำงาน | ใช้ได้ใน |
| --- | --- | --- |
| `\w` | บันทึกไฟล์ปัจจุบัน | Normal |
| `\e` | เปิด prompt `:e ` | Normal |
| `\ff` | ค้นหาไฟล์ด้วย Telescope รวม hidden files | Normal |
| `\cp` | Copy path ลง system clipboard | Normal / Telescope |
| `\mk` | เปิด prompt `:make ` | Normal |
| `\rr` | เปิด prompt shell command `:!` | Normal |
| `\rs` | บันทึกทั้งหมด ปิด Sidebar แล้ว restart และเปิด Sidebar กลับ | Normal |
| `\qq` | บันทึกทั้งหมดแล้วปิดหน้าต่างปัจจุบัน | Normal |
| `\tt` | เปิด prompt `:Terminal ` | Normal |
| `\ts` | เปิด prompt `:Sidebar ` | Normal |
| `\n` | เปิด/ปิด Sidebar | Normal |
| `\s` | สลับ focus ระหว่าง Sidebar กับไฟล์ | Normal |
| `\gs` | เปิด Sidebar และหาไฟล์ปัจจุบัน | Normal |
| `\=` | ขยาย Sidebar 5 ช่อง | Normal |
| `\-` | ย่อ Sidebar 5 ช่อง | Normal |
| `\0` | คืนความกว้าง Sidebar | Normal |
| `\gp` | Preview Git change | ไฟล์ที่มี Gitsigns |
| `\gb` | แสดง Git blame ของบรรทัด | ไฟล์ที่มี Gitsigns |
| `\gd` | แสดง Git diff ของไฟล์ | ไฟล์ที่มี Gitsigns |
| `\db` | เปิด/ปิด Database UI | Normal |

## Custom key

| Key | การทำงาน | Mode / ขอบเขต |
| --- | --- | --- |
| `Ctrl + backtick` | เปิด/ซ่อน bottom terminal | Normal / Insert / Terminal |
| `Ctrl+b` | เปิด/ปิด Sidebar | Normal |
| `Ctrl+j` | ลง 5 บรรทัด | Normal / Visual |
| `Ctrl+k` | ขึ้น 5 บรรทัด | Normal / Visual |
| `Alt+j` | ย้ายบรรทัดลง | Normal / Insert / Visual |
| `Alt+k` | ย้ายบรรทัดขึ้น | Normal / Insert / Visual |
| `kj` | ออกจาก Insert mode | Insert |
| `Ctrl+Backspace` | ลบคำก่อนหน้า | Insert / Command-line |
| `Ctrl+h` | ลบคำก่อนหน้า | Insert / Command-line |
| `K` | doc hint | Normal |
| `gd` | ไปยัง definition | Buffer ที่ LSP attach |
| `gr` | แสดง references | Buffer ที่ LSP attach |
| `]c` | ไปยัง Git change ถัดไป | ไฟล์ที่มี Gitsigns |
| `[c` | ไปยัง Git change ก่อนหน้า | ไฟล์ที่มี Gitsigns |
| `Backspace` | ปิดการใช้งาน | Normal |

## `\cp`

| ตำแหน่ง | Path ที่ copy |
| --- | --- |
| ไฟล์ทั่วไป | Path ของไฟล์ที่เปิดอยู่ |
| Sidebar | Path ของไฟล์หรือโฟลเดอร์ใต้ cursor |
| Telescope (`\ff`) | Path ของรายการที่เลือกอยู่ ใช้ได้ทั้ง Insert และ Normal mode |

## Sidebar

| Key | สถานะ |
| --- | --- |
| `Space` | ปิด |
| `Backspace` | ปิด |
| `-` | ปิด |
| `Ctrl+]` | ปิด |
| `s` | ปิด |
| `S` | ปิด |

## Custom commands

| Command | การทำงาน |
| --- | --- |
| `:Terminal -h {number}` | ความสูง bottom terminal |
| `:Sidebar -w {number}` | ความกว้าง Sidebar (20–80) |
