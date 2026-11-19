# Cassette player

A cassette-style music player for iPhone that plays your own music files.
Each set of songs you pick is one tape. Eject changes the tape, and forward/back skip songs.

The whole app is a single file, `index.html`. It needs no server, and songs are stored on the phone (IndexedDB).

## วิธีใช้บน iPhone
1. เปิดลิงก์ของแอปใน Safari แล้วกด Share > **Add to Home Screen**
2. แตะที่ม้วนเทป ตั้งชื่อเทป แล้วกด **Choose songs** เลือกได้ทีละหลายไฟล์ (MP3, M4A, AAC, WAV) จากแอป Files หรือ iCloud Drive
3. เลือกไฟล์ 1 ครั้งได้เทป 1 ม้วน เพลงเรียงตามชื่อไฟล์ ถ้าอยากกำหนดลำดับ ให้ตั้งชื่อไฟล์ขึ้นต้นด้วย `01`, `02`, ...
4. ปุ่ม ▶︎ เล่น/หยุด, ⏩ เพลงถัดไป, ⏪ เพลงก่อนหน้า และปุ่มส้ม ⏏ เปลี่ยนเทป
5. ถ้าจะลบเทป ให้แตะที่ม้วนเทป กด Remove แล้วกดอีกครั้งเพื่อยืนยัน

## เพิ่ม playlist จาก YouTube / YouTube Music
1. เปิด playlist ในแอป YouTube Music หรือ YouTube แล้วกด Share > **Copy link**
2. playlist ต้องตั้งค่าเป็น **Public** หรือ **Unlisted** ถ้าเป็น Private จะเล่นไม่ได้
3. ในแอป Cassette แตะที่ม้วนเทป พิมพ์ชื่อเทป แล้ววางลิงก์ในช่อง YouTube กด **Add**
4. วิดีโอจะขึ้นในจอเล็กใต้ม้วนเทป เพราะเงื่อนไขของ YouTube กำหนดให้ต้องเห็น player ส่วนเพลงจาก YouTube จะหยุดเมื่อล็อกจอ

## เผยแพร่ด้วย GitHub Pages (ฟรี)
1. ใส่ไฟล์ `index.html` ไว้ที่ root ของ repo
2. ไปที่ Settings > Pages > Source แล้วเลือก **Deploy from a branch** > `main` / `(root)`
3. รอสักครู่ จะได้ลิงก์ `https://je11ybeam.github.io/cassette_player/`

## ข้อจำกัด
- เพลงจะเก็บไว้เฉพาะในเครื่องนั้น และแยกตามวิธีเปิด แอปที่ Add to Home Screen ไว้กับ Safari จะเก็บเพลงคนละที่กัน
- ถ้าเครื่องพื้นที่ใกล้เต็ม iOS อาจลบข้อมูลของเว็บแอปที่ไม่ได้เปิดใช้นานๆ เก็บไฟล์ต้นฉบับไว้ใน Files ด้วยเสมอ
- เพลงจาก Apple Music ที่ดาวน์โหลดไว้ใช้ไม่ได้ เพราะมีการป้องกันลิขสิทธิ์ ต้องเป็นไฟล์เพลงที่คุณมีเอง
