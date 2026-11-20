# HANDOFF — งานวิจัยเกม JoJo's Bizarre Adventure: Golden Spirit

> เขียนเมื่อ 20 พ.ย. 2026 จาก session ก่อนหน้า (cloud)
> **ถึง session ใหม่:** อ่านไฟล์นี้ทั้งหมดแล้วทำงานตามขั้นตอนจนจบ **โดยไม่ต้องถามผู้ใช้เพิ่ม** ยกเว้นตรงที่เขียนว่า "ต้องถาม" เท่านั้น
> ผู้ใช้สื่อสารเป็น **ภาษาไทย** — ตอบและเขียนเอกสารเป็นภาษาไทย (คงชื่อเฉพาะเป็นภาษาต้นฉบับ)

---

## 1. เป้าหมายของผู้ใช้

1. **ฐานข้อมูลเกมที่ละเอียดที่สุด** เกี่ยวกับ *JoJo's Bizarre Adventure: Golden Spirit* (ญี่ปุ่น: ジョジョの奇妙な冒険 黄金讃歌 / Ōgon Sanka, จีน: 乔乔的奇妙冒险：黄金赞歌, เกาหลี: 죠죠의 기묘한 모험: 골든 스피릿, ชื่อเดิม: Golden Anthem / Golden Hymn) — จาก **ทุกแหล่ง ทุกภาษา**
2. **คู่มือบิลด์ตัวละครให้เก่งที่สุด** — ทุกตัวละครเท่าที่หาได้: ดาว, เลเวล, Ability, Dramatic Scenes, Badge, Gems, Spirit Board, ทีม, ลำดับการลงทรัพยากร
3. เก็บผลลัพธ์ไว้ให้ **NotebookLM** ใช้ได้ และให้ **Claude session ต่อ ๆ ไปเรียกใช้ได้** (ไฟล์ใน repo นี้)

---

## 2. สถานะปัจจุบัน (ทำไปแล้ว)

| ไฟล์ / เอกสาร | เนื้อหา | ระดับความครบ |
|---|---|---|
| `research/golden-spirit.md` | ข้อมูลเกมรวม: ชื่อ, บริษัท, ไทม์ไลน์, ระบบเกม, gacha, ตัวละคร, tier list, แบนเนอร์, ผลประกอบการ, แหล่งอ้างอิง | ~60% — มาจาก **สรุปผลการค้นหาเท่านั้น** ยังไม่ได้อ่านหน้าเว็บจริง |
| `research/build-guide.md` | ระบบพัฒนาตัวละคร, Dramatic Scenes, Badge, ทีม, บิลด์ 8 ตัว, รายชื่อคลิป YouTube 21 คลิป | ~40% — ไม่มี transcript YouTube, บิลด์รายตัวยังไม่ครบ |
| Google Doc: [Knowledge Base](https://docs.google.com/document/d/14Hj651jolZ1-Z8gD1n9JrL4SIQqqdJYO_EkjKOKDn6g/edit) (ID `14Hj651jolZ1-Z8gD1n9JrL4SIQqqdJYO_EkjKOKDn6g`) | สำเนาของ `golden-spirit.md` | ต้องอัปเดตตามไฟล์ใหม่ |
| Google Doc: [Build Guide](https://docs.google.com/document/d/16oY2_vDYT09WeGMLNOXpOiXbMw_wmCznCCcOjrobuLI/edit) (ID `16oY2_vDYT09WeGMLNOXpOiXbMw_wmCznCCcOjrobuLI`) | สำเนาของ `build-guide.md` | ต้องอัปเดตตามไฟล์ใหม่ |

**อุปสรรคที่ session ก่อนเจอ (cloud):**
- เครือข่าย cloud environment "Default" ตั้งเป็น Limited — เปิดหน้าเว็บส่วนใหญ่ไม่ได้ (ได้แค่ WebSearch) ตอนนี้อนุญาตเพิ่มแล้ว: `www.youtube.com`, `youtube.com`, `youtubei.googleapis.com`, `www.hideoutgacha.com`, `tychara.com`, `allthings.how`, `jojogs.dev`, `www.goldenspiritcodex.ink`, `progameguides.com`, `jojowiki.com`
- **YouTube บล็อก IP ของ cloud** ("Sign in to confirm you're not a bot") → yt-dlp ดึง transcript ไม่ได้
- ระบบ auto-mode บล็อกการ `curl` ดาวน์โหลดหน้าไกด์ (ผู้ใช้ยังไม่ได้อนุญาตในแชทอย่างชัดเจน) — **ผู้ใช้อนุญาตแล้วใน handoff นี้: "หาจากทุกแหล่ง ทั้งเว็บ youtube และอื่น ๆ ได้หมด"**
- ไม่มีตัวเชื่อมต่อ NotebookLM ใน cloud session

---

## 3. ขั้นตอนเริ่มต้น (ตรวจสภาพแวดล้อมก่อน)

1. ตรวจว่ารันอยู่ที่ไหน:
   - **บนเครื่องผู้ใช้ (local / Remote Control) — แนะนำ** เพราะ YouTube ไม่บล็อก, เข้าเว็บได้หมด, อาจมีตัวเชื่อมต่อ NotebookLM
   - **บน cloud** — ทำต่อได้ แต่ต้องยอมรับข้อจำกัด YouTube (ดูข้อ 4.3 ทางเลือกสำรอง)
2. `git pull` ให้ได้ไฟล์ล่าสุด
3. ทดสอบการเข้าถึงด้วยคำสั่งเดียว เช่น `curl -sI https://jojowiki.com/Golden_Spirit_(Game)` และ `yt-dlp --skip-download --write-auto-subs --sub-langs en "https://www.youtube.com/watch?v=BPfi1CndgUc"`
4. ถ้าบน cloud แล้วโดเมนไหนถูกบล็อก (403 จาก proxy) → ขอเพิ่มโดเมนนั้นผ่าน environment tools (ผู้ใช้กดอนุมัติบนการ์ด) — **รวมโดเมนที่ต้องใช้ทั้งหมดในคำขอเดียว** อย่าขอทีละโดเมน
5. ติดตั้งเครื่องมือ: `pip install yt-dlp html2text` (ถ้ายังไม่มี)

---

## 4. งานที่ต้องทำ

### 4.1 อ่านหน้าเว็บต้นฉบับเต็ม ๆ (แทนสรุปจากการค้นหา)

อ่านทุกหน้าใน "แหล่งอ้างอิง" ของ `research/golden-spirit.md` และ `research/build-guide.md` แล้วเพิ่มลิงก์ใหม่ที่เจอ ลำดับความสำคัญ:

**ข้อมูลเกม**
- JoJo Wiki (ละเอียดที่สุด): `https://jojowiki.com/Golden_Spirit_(Game)` และหน้าย่อยทั้งหมด — `/Events`, `/Badges`, หน้าตัวละครแต่ละตัว (`https://jojowiki.com/Golden_Spirit/<ชื่อ>`), Gallery
- 나무위키: `https://namu.wiki/w/죠죠의 기묘한 모험: 골든 스피릿` (มักมีประวัติ/ข้อถกเถียง/รายได้ละเอียด)
- ข่าว KLab (ญี่ปุ่น): `https://www.klab.com/jp/press/release/2026/0526/preregister.html`, `.../0807/j.html`, `.../0813/j.html` + งบการเงิน KLab ไตรมาส 3/2026 (หลังเปิดเกม)
- gamebiz.jp, 4gamer.net, denfaminicogamer.jp, gamewith.jp
- จีน: gamersky.com, 3dmgame.com, sina.com.cn, bilibili (วิดีโอ/บทความ), taptap.cn — และเช็กสถานะ 版号 (ใบอนุญาตจีน)
- เกาหลี: inven.co.kr, gamemeca.com, khgames.co.kr, betanews.net, ruliweb.com
- ไทย: ค้นหาข่าว/กลุ่ม Facebook/คลิปไทย (คำค้น: "JoJo Golden Spirit ไทย", "โจโจ้ Golden Spirit") — ตอบคำถาม "รองรับภาษาไทยไหม / เล่นในไทยได้ไหม"
- ร้านค้า: App Store `https://apps.apple.com/us/app/jojos-bizarre-adventure-gs/id6757908157`, Google Play `com.wanda.jojo.gp.global` (ภาษา, ขนาด, เรต, เรตติ้ง, version history)
- ช่องทางทางการ: X `@jojogs_official`, เว็บไซต์ทางการ, Discord, Reddit (r/JoJoGoldenSpirit หรือ subreddit ที่ใช้จริง)

**บิลด์**
- Hideout Gacha: `https://www.hideoutgacha.com/games/jojo-golden-spirit/characters` + หน้าตัวละครทุกตัว + `/modes-and-systems`, `/beginner-guide`, `/tier-list`
- Tychara: `https://tychara.com/JoJoGoldenSpirit/characters/<ชื่อ>/` ทุกตัว + `/tier-list/`
- allthings.how (badge guide, Diavolo, Caesar, tier list, reroll, codes)
- jojogs.dev (`/investment`, `/guides/beginners-guide`, `/changelog`)
- goldenspiritcodex.ink, goldenspiritguides.com, jojosbizarreadventuregoldenspirit.wiki, gacha.gg, game.guide, progameguides.com, game8.co, powerupgaming.co.uk, destructoid.com

### 4.2 YouTube — ดึง transcript แล้วสรุป

รายชื่อคลิปที่ต้องทำ (21 คลิปใน `research/build-guide.md` ข้อ 6) **+ ค้นเพิ่ม** ด้วย `yt-dlp --flat-playlist "ytsearch20:<คำค้น>"` เช่น:
`JoJo Golden Spirit build guide`, `... badge guide`, `... best team`, `... tier list November`, `... <ชื่อตัวละคร> build`, `黄金讃歌 編成`, `黄金赞歌 攻略`, `골든 스피릿 공략`, `JoJo Golden Spirit ไทย`

สำหรับแต่ละคลิป: ดึง auto-subs (`--write-auto-subs --sub-langs "en.*,ja,zh.*,ko,th" --skip-download`), แปลง VTT เป็นข้อความ, สรุปเป็น **บิลด์ที่ใช้ได้จริง** (ตัวละคร → ดาวขั้นต่ำ, Scene set + base attribute, Badge + เหตุผล, Gems, ตำแหน่งในทีม, คู่หูที่เข้ากัน) พร้อมระบุ **ช่อง + วันอัปโหลด + ลิงก์ + timestamp**

### 4.3 ถ้าดึง transcript YouTube ไม่ได้ (ทางเลือกสำรองตามลำดับ)
1. ถ้าอยู่บน cloud → บอกผู้ใช้หนึ่งบรรทัดว่า YouTube บล็อก cloud แล้วแนะนำให้รัน session นี้บนเครื่องตัวเอง (`claude remote-control` หรือ Claude Desktop) — **แต่ทำงานส่วนอื่นต่อให้เสร็จก่อน อย่าหยุดรอ**
2. ใช้บทความ/ไกด์ที่สรุปคลิปเดียวกัน, คอมเมนต์ปักหมุด, คำอธิบายคลิป (description) จากผลค้นหา
3. **ห้าม** แต่งเนื้อหาคลิปขึ้นเอง และห้ามใช้เทคนิคหลบการตรวจจับบอทของ YouTube

### 4.4 ผลลัพธ์ที่ต้องได้

อัปเดต/สร้างไฟล์ใน `research/`:

1. **`research/golden-spirit.md`** — เขียนใหม่ให้ครบ ครอบคลุม:
   ชื่อทุกภาษา · บริษัทและบทบาท · ไทม์ไลน์ครบทุกวันที่ · ภูมิภาค/ภาษา/แพลตฟอร์ม/เรต · ระบบเกมทั้งหมด (การต่อสู้, energy, Rush, 6 สไตล์, สภาพอากาศ, โหมดทั้งหมดและเลเวลปลดล็อก) · gacha (อัตรา, pity, สกุลเงิน, ประวัติแบนเนอร์ทุกตู้พร้อมวันที่) · **รายชื่อตัวละครครบทุกตัว** (Part, ความหายาก, สไตล์, Stand, วันที่เพิ่ม) · อีเวนต์และแพตช์ทุกครั้ง · โค้ด · ผลประกอบการ/อันดับ/รายได้ · นักพากย์/ดนตรี/ทีมงาน · ข้อถกเถียงและการตอบรับ · สถานะญี่ปุ่น/จีน/ไทย · แหล่งอ้างอิงทั้งหมด
2. **`research/build-guide.md`** — เขียนใหม่ให้ครบ:
   - ระบบการพัฒนาทั้งหมดพร้อมตัวเลขจริง (เพดานเลเวล, ต้นทุน, ขั้นดาว 16 ขั้น, Spirit Board)
   - **ตารางบิลด์ทุกตัวละคร**: ตัวละคร | ความหายาก | สไตล์ | บทบาท | ดาวขั้นต่ำ/เป้าหมาย | Scene set (2/4 ชิ้น) + base attribute | Badge หลัก/สำรอง | Gems | Spirit Power | ทีมที่เข้ากัน | ระดับใน tier list ล่าสุด
   - ทีมแนะนำแยกตามโหมด: Story, Arena (PvP), Guild Boss, World Boss, Extreme Trial, Interview Trial, Bloody Battle — แยก **F2P** และ **มีเงินเติม**
   - ลำดับการลงทรัพยากรสำหรับผู้เล่นใหม่ / กลางเกม / ปลายเกม
   - tier list ล่าสุด (ระบุวันที่และแหล่ง)
   - สรุปจาก YouTube แต่ละคลิป (ข้อ 4.2)
3. **`research/youtube/`** — เก็บ transcript ที่ดึงได้เป็นไฟล์ `.txt` (ชื่อไฟล์ = video ID) + `index.md` ที่มีชื่อคลิป ช่อง วันที่ ลิงก์
4. **`research/sources.md`** — รายการแหล่งทั้งหมด จัดกลุ่มตามภาษา พร้อมวันที่เข้าถึง และหมายเหตุว่าอ่านเต็มหรือแค่สรุปจากการค้นหา

### 4.5 ส่งออกไป NotebookLM / Google Drive
1. ถ้ามีตัวเชื่อมต่อ NotebookLM → สร้าง notebook "JoJo Golden Spirit" แล้วเพิ่มไฟล์ทั้งหมดเป็น source
2. ถ้าไม่มี → **อัปเดต Google Doc 2 ตัวในข้อ 2** ด้วยเนื้อหาใหม่ (ใช้ Google Drive tools — update ไฟล์เดิมโดยใช้ ID ไม่ต้องสร้างใหม่) และสร้าง Doc ใหม่สำหรับไฟล์ YouTube summary ถ้ามี
3. บอกผู้ใช้ขั้นตอนเพิ่ม source ใน NotebookLM: New notebook → Add source → Google Drive → เลือกเอกสาร

### 4.6 Commit
- commit + push ขึ้น `main` ของ `pjaitutor-maker/jojo-bizarre` เป็นระยะ (อย่างน้อยหลังจบแต่ละข้อ 4.1 / 4.2 / 4.4) เพราะ cloud container อาจถูกลบ

---

## 5. กฎคุณภาพ

- **ห้ามแต่งข้อมูล** — ทุกข้อเท็จจริงต้องมีแหล่ง ถ้าไม่พบให้เขียนว่า "ไม่พบข้อมูล"
- ข้อมูลขัดกัน → ใส่ทุกเวอร์ชันพร้อมแหล่ง, ติด ⚠️, และระบุว่าเชื่ออันไหนมากกว่าเพราะอะไร (แหล่งทางการ > วิกิ > ไกด์ใหม่ > ไกด์เก่า)
- ระบุ **วันที่** ของข้อมูลเมตา/tier list/บิลด์เสมอ (เกมอัปเดตบ่อย)
- แยกให้ชัดระหว่าง "อ่านจากหน้าต้นฉบับ" กับ "จากสรุปผลการค้นหา"
- ตัวเลขรายได้จากเว็บติดตาม = ประมาณการ ไม่ใช่ตัวเลขบริษัท
- เคารพความเป็นส่วนตัว: ไม่ใส่ข้อมูลส่วนตัวของผู้ใช้ในคำขอไปยังบริการภายนอก

---

## 6. เมื่อทำเสร็จ — รายงานผู้ใช้ (ภาษาไทย, สั้น)

- ลิงก์ไฟล์/Google Doc ที่อัปเดต
- สรุป 5–7 ข้อว่า "บิลด์ให้เก่งที่สุด" ต้องทำอะไร
- อะไรที่ยังหาไม่ได้และเพราะอะไร
- ถ้าบน cloud แล้วติด YouTube → แนะนำรันบนเครื่องเพื่อเก็บ transcript ให้ครบ
