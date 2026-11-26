# LearnLab — ห้องเรียนออนไลน์วิทยาศาสตร์และคณิตศาสตร์ ม.4–ม.6

เว็บไซต์เรียนรู้ภาษาไทยสำหรับทบทวนวิทยาศาสตร์และคณิตศาสตร์ระดับมัธยมศึกษาตอนปลาย สร้างด้วย HTML, CSS และ JavaScript โดยไม่ต้องติดตั้งระบบหลังบ้าน

## ไฟล์ในโปรเจกต์
- `index.html` โครงสร้างหน้าเว็บและหน้าต่าง ๆ
- `style.css` ธีมสีชมพูพาสเทล ตัดด้วยลาเวนเดอร์ มิ้นต์ และครีม พร้อมรองรับมือถือ
- `data.js` บทเรียน สูตร แบบทดสอบ และข้อมูลธาตุ
- `app.js` ระบบนำทาง ค้นหา กรองระดับชั้น เปิดบทเรียน ตารางธาตุ คลังสูตร แบบทดสอบ และพิมพ์เอกสาร

## สิ่งที่มีในรุ่นนี้
- บทเรียน 23 บท แยกตามวิชาและระดับ ม.4, ม.5 และ ม.6
- บทเรียนมีจุดประสงค์ หัวข้อย่อย คำอธิบาย รายการสำคัญ สูตร ตัวอย่าง เทคนิคจำ สรุปท้ายบท และจุดที่มักพลาด
- แบบทดสอบแยกก่อนเรียน 10 ข้อและหลังเรียน 10 ข้อต่อบท รวม 20 ข้อต่อบท พร้อมเฉลยอธิบาย
- ตัวกรองระดับชั้นแยกในหน้าวิทยาศาสตร์และคณิตศาสตร์
- คลังสูตร ตารางธาตุ 118 ธาตุ และระบบแบบทดสอบพร้อมเฉลยอธิบาย
- พิมพ์บทเรียนหรือบันทึกเป็น PDF ผ่านเมนู Print ของเบราว์เซอร์
- เพิ่มเนื้อหาต่อยอดในบทเรียนทุกบท พร้อมทางลัดติดต่อ/รีวิวที่เห็นได้ทุกหน้า และแบบฟอร์มให้คะแนน/ส่งข้อเสนอแนะ
- เพิ่มตัวอย่างการประยุกต์ใช้และคำถามฝึกคิดที่แตกต่างกันตามแต่ละบทเรียน และแสดงหัวข้อย่อยที่เคยไม่ถูกนำมาแสดง

## เปิดดูในเครื่อง
แตกไฟล์ ZIP แล้วเปิด `index.html` ด้วยเบราว์เซอร์ หรือใช้ Live Server ใน VS Code

## เผยแพร่ด้วย GitHub Pages
1. อัปโหลดไฟล์ทั้งหมดในโฟลเดอร์นี้ไว้ที่ root ของ branch `main` ใน repository `panida-6-6/LearnLabscimch`
2. ไปที่ Settings → Pages
3. ใน Build and deployment เลือก Deploy from a branch
4. เลือก branch `main` และ folder `/ (root)` แล้วกด Save
5. GitHub Pages จะแสดง URL ของเว็บไซต์ในหน้า Pages เมื่อ deploy สำเร็จ

## รีวิวและช่องทางติดต่อ
- รีวิวที่ส่งจากฟอร์มจะเก็บใน `localStorage` ของเบราว์เซอร์ผู้ส่งเท่านั้น และจะแสดงในเครื่องนั้น ไม่ได้รวมเป็นรีวิวสาธารณะสำหรับผู้เข้าชมทุกคน
- หากต้องการรับความคิดเห็นจากผู้ใช้ทุกคนจริง ๆ ให้เชื่อมแบบฟอร์มกับบริการจัดเก็บ/รับฟอร์ม เช่น Formspree หรือฐานข้อมูลก่อนเผยแพร่
- เปลี่ยนอีเมล `learnlab@example.com` ใน `index.html` เป็นอีเมลติดต่อจริง และเปลี่ยนลิงก์ GitHub placeholder เป็น URL repository หรือ Issues ของโครงการ

## เพิ่มบทเรียน
เพิ่ม object ใน array `LESSONS` ภายใน `data.js` โดยกำหนด `id`, `subject`, `category`, `level`, `title`, `desc`, `goals`, `sections`, `memory`, `summary` และ `mistakes`

## หมายเหตุเรื่องหลักสูตรและข้อสอบ
บทเรียนเป็นสื่อทบทวนที่เรียบเรียงเพื่อช่วยทำความเข้าใจ ไม่ใช่เอกสารหลักสูตรทางการ ควรตรวจสอบหัวข้อและตัวชี้วัดกับหลักสูตรสถานศึกษาและหนังสือเรียนที่ใช้จริงก่อนสอบ เนื้อหาและข้อสอบในรุ่นนี้ยังเป็นฉบับขยายระยะแรก และยังไม่ใช่คลังข้อสอบ 20 ข้อครบทุกบท

## เพิ่มเติมในเวอร์ชันนี้
- เพิ่มหน้า **คลังวิดีโอ** แยกตามวิชา พร้อมตัวกรองและค้นหาบทเรียน
- เพิ่มลิงก์ค้นหา YouTube ตามหัวข้อย่อยในแต่ละบทเรียน
- ขยายคลังสูตรจาก 32 รายการเป็น 100 รายการ ครอบคลุมฟิสิกส์ เคมี และคณิตศาสตร์
- หมายเหตุ: ลิงก์วิดีโอเป็นการค้นหา YouTube ตามหัวข้อ ยังไม่ได้ตรวจสอบคลิปเฉพาะรายคลิปหรือฝังตัวเล่นวิดีโอโดยตรง



## LearnLab update
- เพิ่มหน้าบัตรคำทบทวนที่สร้างจากเนื้อหาบทเรียนจริง
- เพิ่มเครื่องคำนวณอัตราเร็ว กฎนิวตัน โมล และโมลาร์
- เพิ่มการบันทึกความคืบหน้าการอ่านบทเรียนไว้ในเบราว์เซอร์
- ปรับข้อความจำนวนข้อสอบให้ตรงกับชุดคำถามของแต่ละบทและช่วงก่อน/หลังเรียน
- ปรับคำค้นหาวิดีโอให้ระบุระดับชั้นและภาษาไทยชัดเจนขึ้น (ยังเป็นลิงก์ค้นหา ไม่ใช่วิดีโอที่คัดเลือก/ฝังไว้)

## การปรับปรุงเนื้อหาและคลิปวิดีโอ (รอบเพิ่มเติม)
- เพิ่มหัวข้ออธิบายเชิงลึกแบบเฉพาะเรื่องให้ครบทั้ง 48 บท พร้อมตัวอย่าง วิธีคิด สูตร หรือประเด็นเชื่อมโยงตามความเหมาะสม
- เนื้อหาส่วนเพิ่มเติมจะแสดงต่อจากเนื้อหาเดิม และถูกรวมในระบบบัตรคำทบทวนด้วย
- เปลี่ยนวิดีโอจากลิงก์ค้นหา YouTube เป็นลิงก์ไปยังคลิปเฉพาะที่ตรวจสอบหัวข้อและ URL แล้ว
- ขณะนี้มีคลิปที่คัดเลือกและตรวจสอบแล้วในบางบทเท่านั้น บทอื่นจะแสดงข้อความแจ้งว่ายังไม่มีคลิปที่ตรวจสอบแล้ว แทนการส่งผู้ใช้ไปหน้าค้นหา
- รายการวิดีโอสามารถเพิ่มได้ภายหลังในตัวแปร `LESSON_VIDEOS` ท้ายไฟล์ `data.js` โดยใช้รูปแบบ `{title, url, source}`

หมายเหตุ: ควรตรวจสอบความถูกต้องของเนื้อหาและความพร้อมใช้งานของวิดีโออีกครั้งก่อนนำไปใช้เป็นเอกสารการเรียนการสอนอย่างเป็นทางการ ลิงก์ YouTube เป็นของเจ้าของช่องและอาจเปลี่ยนแปลงได้

## Update 26 November 2026 – interactive study tools

- All 48 lessons now include an additional subject-specific section: **แนวทางคิดและตรวจคำตอบ**.
- The quiz bank is expanded at runtime to **20 questions per lesson for the pre-test and 20 for the post-test** (1,920 questions across 48 lessons). Existing authored questions are retained; new review questions are built from the lesson goals, explanations, examples, formulas, summaries, and common mistakes. Treat these as practice questions and review the explanations after submitting.
- Flashcards now build a deck from lesson headings, explanations, key points, formulas, examples, and summaries. Subject, level, and lesson filters work; cards flip and the previous/next controls move through the deck.
- The four calculators (average speed, Newton's second law, amount of substance, and molarity) now validate input and show the formula and calculation steps.
- Video cards use direct YouTube watch links, not YouTube search queries. There are direct links for 28 of the 48 lessons; lessons without a verified direct clip are labelled as not yet available rather than being sent to a search page.
- GitHub Pages is static hosting. Review submissions and learning progress are stored in the visitor's own browser unless a backend or external form service is connected.

A number of direct video URLs were selected from OnDemand's public high-school free-trial video library: https://www.ondemand.in.th/free-trial-%E0%B8%A1-%E0%B8%9B%E0%B8%A5%E0%B8%B2%E0%B8%A2/
