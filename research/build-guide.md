# JoJo Golden Spirit — คู่มือบิลด์ตัวละคร (Build Guide) v2

> รวบรวมเมื่อ: **20 พฤศจิกายน 2026** · เกมอัปเดตบ่อย ตรวจวันที่ของ tier list ทุกครั้ง
> ระดับความน่าเชื่อถือ: 📖 = อ่านหน้าต้นฉบับเต็ม · 🔎 = สรุปจากผลค้นหา · ⚠️ = แหล่งขัดกัน
> **YouTube:** ดึง transcript ไม่ได้ (YouTube ตอบ HTTP 429 ต่อการขอซับไตเติลจากเครื่องนี้ แม้อัปเดต yt-dlp และเว้นจังหวะแล้ว) — ได้เฉพาะ **ชื่อ/ช่อง/วันที่/ยอดวิว/บท (chapters)/description** ดู [youtube/index.md](youtube/index.md) → **บิลด์ในไฟล์นี้ไม่ได้มาจากเนื้อหาในคลิป** ห้ามอ้างว่าเป็นของคลิป
> **บิลด์ละเอียดรายตัว:** [builds/jotaro.md](builds/jotaro.md) (มี transcript YouTube ที่อ่านผ่าน Chrome)
> ไฟล์คู่กัน: [golden-spirit.md](golden-spirit.md) · [characters.md](characters.md) (สกิล+บิลด์ละเอียดทุกตัว) · [badges.md](badges.md)

---

## 0. TL;DR — ทำอะไรก่อนหลัง (สรุป 7 ข้อ)

1. **อย่ากระจายทรัพยากร** — เลือก **ทีมหลัก 5 ตัว** แล้วดัน Character Level + Ability Level ให้ชนเพดาน (เพดานผูกกับ Account Level เลื่อนตามการเล่น)
2. **ทีมต้องมี ≥3 สไตล์ต่างกัน** เพื่อเปิด Rush (+25% Final DMG 10 วิ) — อย่าใส่สไตล์เดียวกันหมด
3. **Star-up ตัวแครี่หลัก + ซัพพอร์ตหลักก่อน** เมื่อได้ตัวซ้ำ (★2 ปลดสกิล 3, ★3 ปลดสกิล 4, ★5 ปลดสกิล 5; ★4 เป็นแค่จุดสถานะ)
4. **เมตาตอนนี้ (Hideout 20 พ.ย.)**: Jotaro, Prosciutto, Bucciarati, Caesar, F.F., Kakyoin, Koichi, Giorno, Iggy, Ermes อยู่ Tier S — แกนกลางที่ใช้บ่อยใน team comp = **Giorno + Jotaro + Bucciarati + Caesar**
5. **Dramatic Scenes**: ฟาร์มจาก Extreme Trial; เซตตามบทบาท — melee = *The Greatest High Known to Man!*, ranged = *Stone Ocean*, แท็งก์ = *I Decline*, ฮีลเลอร์ = *The Final Hamon*; ดัน 4 ชิ้นให้ได้เซต 4-pc ก่อน
6. **Badge**: ตรวจเงื่อนไขสกิล (Melee/Ranged only) ก่อนใส่; อัปทั้ง 4 ชิ้นให้ได้เซต; Badge ที่ไม่ใช้ → dismantle เป็น Gem (Gem ย้ายใช้ใหม่ได้ ไม่เสียของ)
7. **ที่ Account Lv.13 เริ่ม Spirit Board** (วัสดุมาจาก Double Clash) และหยุดสุ่มแบบเปลืองเปล่า: ออมไป **60 (การันตี) / 180 (selector)** ไม่ต้อง reroll

---

## 1. ระบบพัฒนาตัวละคร (ตัวเลขจริง) 📖

| ลำดับ | ระบบ | ใช้อะไร | สาระ |
|---|---|---|---|
| 1 | **Character Level** | Courage Essence/Crystal + Coin | 100 ขั้น; เพดานตาม Account/Quest Level (เช่น Lv.12 → ตัวละครสูงสุด Lv.40) |
| 2 | **Ability Level** | Ability Essence/Crystal + Coin | แยกเส้น 100 ขั้น; เพิ่มพลัง Ability ที่ใส่ (สำหรับส่วนใหญ่ = Stand); ตู้ Ability ถาวร selector ที่ 150 ครั้ง; Ability เลื่อนได้ถึง **S11** แล้ว Ability Boost ด้วย Stone of Destiny |
| 3 | **Star Rank** | ตัวซ้ำ/shard | ★1–★5 แล้วต่อเป็นรวม **16 ขั้น**; ที่ 4 ดาวได้ภาพ Rank II; แต่ละขั้นให้ HP/ATK/DEF ถาวร + ปลดสกิล (3rd=★2, 4th=★3, 5th=★5) |
| 4 | **Star Tree** | Stone of Destiny + Coin | 132 โหนด / 6 ต้นไม้ร่วม; ครบทั้งหมดต้องใช้ Stone หลักพัน + Coin >1 ล้าน → ป้อนทีละน้อยให้ตัวที่จะเก็บยาว |
| 5 | **Dramatic Scenes** (ปลดหลังด่าน N3-10) | ฟาร์ม Extreme Trial | 4 ช่อง/ตัว; 5 เกรด (Minion/Rare/Superior/**Excellent**/Outstanding); ต้อง Excellent+ ชื่อเดียวกัน 2/4 ชิ้นจึงได้โบนัสเซต; อัปที่ **+4/+8/+12** สุ่มค่ารอง; Outstanding Lv.100 ตั้งเป็น "Favorite" ด้วย Camrecorder เพื่อปลด +16/+20; ย้ายของเก่าไปชิ้นใหม่ **ไม่เสียค่าอัป 100%** |
| 6 | **Badge + Gem** (ปลดหลังด่าน N4-10) | Forge (Refined Iron/Gold Ingot/Rawstone/Blueprint) | ดูข้อ 3 |
| 7 | **Spirit Realm / Spirit Board** | Spirit Power | ⚠️ ปลดที่ **Account Lv.13** (jojogs.dev/PUG) และตามเลเวลตัวละคร: **9 ช่องที่ Lv.45, ครบ 18 ช่องที่ Lv.80**; ใส่ได้พร้อมกัน **3 อัน**; รวม Spirit Power ระดับเดียวกันถึง 6 ช่อง (3→5 ช่องอาจปลด attribute/talent ใหม่, 5→6 ช่องอัป talent หนึ่งช่อง); talent มี 6 ระดับ (Uncommon→Exalted); ถึง 3 ช่องแล้ว master/reshape ด้วย shard; มี Realm Bonus เมื่อใส่ระดับเดียวกันครบ |
| 8 | **Gallery** (Quest Lv.4) | Gallery XP/Chapter | โบนัสสถานะทุกตัว + รายตัว; v1.0.10 ลดต้นทุนแล้ว |
| 9 | **Collectibles** | Intel จาก SPW Request | โบนัสสถานะทั้งโรสเตอร์ |
| 10 | **Guild Training** | Training Voucher/Combat Recording | โบนัสแยกตามสไตล์ (ใช้เฉพาะสไตล์นั้น) |

**หลักการลงทรัพยากร** (PUG 19 ส.ค. 🔎→📖 อ่านเต็ม + jojogs.dev 📖): Character/Ability Level เลื่อนตามบัญชีเอง ต้องวางแผนจริงจังเฉพาะ Star Rank, Star Tree, Badge promote, Scene
**ลำดับ**: (1) ดันเนื้อเรื่อง/Account Level → (2) ทีมหลัก 5 ตัวขึ้นเพดาน Character+Ability → (3) Star-up แครี่/ซัพพอร์ตหลัก → (4) เช็กลิสต์รายวัน → (5) Lv.13 เริ่ม Spirit Board + Badge เซตพื้นฐาน → (6) Star Tree + Badge โปรโมตสูง เฉพาะตัวที่จะเก็บยาว

## 2. Dramatic Scenes (9 เซต) 📖

| เซต | 2-pc | 4-pc | เหมาะกับ |
|---|---|---|---|
| **The Greatest High Known to Man!** | ATK +5% | ATK +5%; Ultimate มี 50% เจาะ DEF เป้า 20% | Melee DPS (Diavolo, Bucciarati, Akira) |
| **Stone Ocean** | ATK +5% | ATK +5%; ดาเมจโจมตีปกติ +4%/ช่องระยะ สูงสุด +20% | Ranged DPS (Caesar, F.F.) |
| **I Decline** (But I Decline) | DEF +5% | DEF +5%; ใช้สกิลตอน HP <50% ได้ Defense Up ×2 | แท็งก์ (Ermes, Jonathan, Iggy) |
| **The Final Hamon** | HP +5% | HP +5%; ฮีลเป้า HP <50% ฟื้นเพิ่ม 20% | ฮีลเลอร์ (Giorno, Tonio) |
| **Do Something** (Think of Something) | ATK +5% | ATK +5%; โจมตีปกติ 30% ทำให้สกิลถัดไปแรงขึ้น 20% (ไม่ซ้อน) | DPS สายสกิล (Caesar endgame, Diavolo) |
| **Gang-Star** | — | เปิดการต่อสู้ด้วยบัฟ ATK/DEF | (ดูที่ Extreme Trial Lv.80+) |
| **I Cast Aside My Humanness** | HP +5% | ATK +5%; สกิล/โจมตีปกติลด DEF เป้า 6% นาน 6 วิ (ไม่ซ้อนกันทั้งทีม) — 📖 Hideout, สอดคล้อง Codex | Jotaro ต้นเกม, Secco |
| **The Hymn of Bravery** | — | บัฟที่ให้มีโอกาสกระจายไปพันธมิตรใกล้ | Giorno |
| **The Taste of a Lie** | — | debuff ที่ใส่มีโอกาสซ้ำ | Bucciarati, Joseph, Chaka |

แหล่งฟาร์ม: Extreme Trial Lv.20 (4 เซตแรก) → Lv.40 (+Humanness, Do Something) → Lv.60 (+Hymn, Taste of a Lie) → Lv.80 (+Gang-Star) → ทีม Lv.100 I/II/III (ดรอป Camrecorder ด้วย)
เลือกชิ้นที่ **base attribute ตรงบทบาท** (ดาเมจ=ATK / แท็งก์=DEF/HP / ฮีล=HP — ฮีลสเกลกับ HP ของผู้ฮีลเอง)

## 3. Badge และ Gem 📖 (เต็ม 69 แบบใน [badges.md](badges.md))

**กติกา**
- Badge **ไม่ผูกกับตัวละคร** — ใครใส่ก็ได้ แต่บางสกิลทำงานเฉพาะ **Melee/Ranged** (อ่านเงื่อนไขทุกครั้ง)
- เกรด Rare → Epic → Legendary → Mythic; โปรโมตได้จนเพดานตามเกรดเริ่มต้น (Rare★1→Epic★2, Epic★1→Legendary★2, Legendary★1→Mythic★1); ถึง **3 ดาวปลดช่อง Gem**
- ใส่ Badge ชื่อ **สกิลเดียวกันหลายชิ้น = เลเวลรวมกัน**; ทั้ง 4 ชิ้นต้องถึงจุดเปิดเซตก่อนดันสูง
- คราฟต์: Regular (Refined Iron → 95% Rare/5% Epic) · Set (50 Refined Iron + 10 Gold Ingot → Epic ครบ 4 ชิ้นรับประกัน) · Blueprint (Legendary ตามแบบ; ได้จากร้าน Monthly Pass/Boss Store/กล่องเลือกแบบ + Rawstone)
- Gem: dismantle Badge ได้สกิลเป็น Gem ย้ายไปใส่ที่อื่น — เสี่ยงต่ำ ใช้ Badge ที่ไม่ใช้ให้เกิดค่า
- สถิติ: DPS เน้น ATK, แท็งก์ เน้น DEF, ซัพพอร์ต เน้น HP

**Badge เด่น (Legendary/Mythic สูงสุด 4/4) 📖**
| Badge | สกิลเด่น (ค่าสูงสุด) | ใช้กับ |
|---|---|---|
| **Caesar** | Penetration: โจมตีปกติเจาะ DEF 32% (Ranged เท่านั้น) + Adv. Attack ฐาน ATK +20% | Ranged DPS |
| **Jotaro** | Star: โจมตีปกติ 20% Stun 1 วิ + ดาเมจเพิ่ม 160% ATK (Melee, CD 4 วิ) + ATK/HP +10% | Melee DPS |
| **Kakyoin** | Hawk-Eye: Crit Boost +3,250 + โอกาสคริ +16% (Ranged) | Ranged |
| **Iggy** | Protection: ทุก 3 วิ โล่ 160% DEF ให้พันธมิตร HP ต่ำสุด; ตายแล้วโล่ทั้งทีม | แท็งก์/ซัพพอร์ต |
| **Avdol** | Assault: เข้าสนาม/กดอัลติ → โจมตีปกติ 3 ครั้งถัดไป +40% Crit Rate | DPS |
| **Koichi** | Onslaught: ใช้สกิล/อัลติ ได้สแตก +12% ดาเมจสกิล ×3 (Ranged) | Ranged สายสกิล |
| **Giorno / Ermes / Jonathan / Joseph II** | โล่ทีม / ฮีล-โล่ / ลดดาเมจพันธมิตร 2 ช่อง 10% (HP>50%) / บัฟดาเมจ 40% ต้นสนาม (Ranged) | ซัพพอร์ต/แท็งก์ |
| **Akira Otoishi** | Impulse: Crit Boost +3,250 แต่ **รับดาเมจ +20%** (Melee) + Lethality: คริ ดาเมจ +180% ATK (CD 4 วิ) | Melee DPS ที่อึดพอ |
| **Mariah / Leaky-Eye Luca / Shigekiyo / Gwess / Bruford / Straizo** | Rare/Epic ราคาถูก: ฐาน ATK/DEF/HP เพิ่ม | ต้นเกม/F2P |

(Boss Store ขาย Speedwagon/Santviento/Joseph/Stroheim/Lisa Lisa Badge I–IV ชิ้นละ 800 Challenge Coin; Blueprint Giorno 6,000; Monthly Pass Store ขาย Koichi/Jotaro/Giorno Blueprint ชิ้นละ 200 token ซื้อได้ 4 ครั้ง)

## 4. ทีมแนะนำ 📖 (Hideout Team Compositions, อ่านเต็มหน้า — ชุดชุมชน + แกนที่ซ้ำ)

**โหมด PvE รายวัน — World Boss ตามวัน (ทีมชุมชน)**
| วัน | บอส | ทีม (ซ้าย→ขวา) | ตัวสำรอง |
|---|---|---|---|
| จ | Akira Otoishi | Caesar · Prosciutto · Giorno · Bucciarati · Jotaro | F.F. แทน Caesar |
| อ | Notorious Chase | Bucciarati · Caesar · Giorno · Jotaro · Speedwagon | |
| พ | Risotto Nero | Bucciarati · Giorno · Hol Horse · Jotaro · Speedwagon | Caesar/F.F. แทน Hol Horse |
| พฤ | F.F. | Jotaro · Caesar · Tonio · Giorno · Bucciarati | |
| ศ | Tarukus | Jotaro · Speedwagon · Caesar · Giorno · Bucciarati | |
| ส | Wamuu | Bucciarati · F.F. · Koichi · Jotaro · Giorno | |
| อา | Cool Ice | Caesar · Jotaro · Bucciarati · Giorno · Koichi | |

**Co-op Raid** (ยืมตัวละครผู้เล่นอื่นได้): Raid 1 (Johngalli A.) / Raid 2 (Rubber Soul) / Raid 3 (Pesci & Prosciutto) — ชุดแกน Giorno + Jotaro + Caesar + Bucciarati (+Prosciutto/F.F./Speedwagon); เซต/Badge ที่ชุมชนใช้: Giorno = *The Hymn of Bravery* + Giorno Badge; Jotaro = *The Greatest High Known to Man!* + Kenzou Badge; Caesar = *Stone Ocean* + Caesar Badge; Bucciarati = *The Taste of a Lie* + Ermes Badge

**PvP (Arena/Ranked) ชุมชน 4 ทีม**: ① Giorno · Diavolo · Ermes · Jotaro · Koichi ② Ermes · Leone Abbacchio · Jotaro · F.F. · Giorno ③ Jotaro · Koichi · Ermes · Giorno · Bucciarati ④ Jotaro · Giorno · Ermes · Prosciutto · F.F.
**PvE ทั่วไป 3 ทีม**: ① Tonio · Giorno · Koichi · Jotaro · Ermes ② Giorno · Caesar · Koichi · Jotaro · Ermes ③ Tonio · Joseph(SR) · Jotaro · Prosciutto · Santana

**ทีม F2P / ประหยัด (PUG 17 ส.ค. 📖)**
- **Budget Bullet Train**: Santviento (แท็งก์หน้ากลาง) + Hol Horse (DPS หลัก ยืนหลังสุด; อัลติแบบ channel โดน CC ขัดได้) + Lisa Lisa (ส่ง Energy ให้ผู้มี ATK สูงสุด → ปรับให้เป็น Hol Horse) + Lang Rangler (บัฟดาเมจ/ความเร็วสายไกล) + Tonio (ฮีล/ล้าง debuff) — แทน Lang ด้วย Will A. Zeppeli, แทนแท็งก์ด้วย Leone Abbacchio ได้
- **Bubble Beatdown** (ราคาถูก ไม่เป๊ะ F2P): Jonathan (แท็งก์) + Caesar (DPS) + Koichi (คุม) + Joseph (ซัพพอร์ต/ดึง-สตัน) + Giorno (ฮีล) — สำรอง: Ermes แทน Jonathan, Tonio แทน Joseph เมื่อต้องล้าง debuff หนัก
- Joseph SR เป็นตัวแจกฟรี (รางวัลลงทะเบียน 2M), Giorno แจกฟรีช่วงต้น ⚠️ (ตามไกด์ PUG; ยืนยันในเกม)

**หลักการทีม**: แนวหน้า 1 (Defense/Assault) · DPS 2–3 · Special 1 (ปั่น energy) · Support 1 (ฮีล) · ≥3 สไตล์เพื่อ Rush · ตัวสายไกลยืนหลังสุด ตัวแท็งก์กลางหน้า · พิจารณา **สภาพอากาศ** (หมอกลดสายไกล, พายุฟ้าผ่า ฯลฯ) และ **ศัตรูพิเศษ** (Hamon ได้เปรียบ Vampire/Zombie)

## 5. Tier list ล่าสุด + ตารางบิลด์รายตัว

### 5.1 Tier ล่าสุด (Hideout Gacha — โหวตชุมชน อ่านเต็มหน้า 20 พ.ย. 2026) 📖
- **S**: Prosciutto, Jotaro · Iggy, Ermes · Bucciarati · Kakyoin, Caesar, F.F. · Koichi · Giorno
- **A**: Lisa Lisa · Diavolo · Hol Horse · Avdol · Joseph(SR), Kenzou, Speedwagon, Tonio
- **B**: Rubber Soul · Mista, Keicho · Tennille · Pesci · **C**: Cioccolata, Narancia · ที่เหลือ **D**
- ⚠️ PvE tier ต่างจาก Overall (เช่น Ermes S→PvE A, Prosciutto S→PvE A, Diavolo A→PvE B, Avdol A→PvE C) ดูคอลัมน์ PvE ด้านล่าง
- ⚠️ Closed-Beta (Tychara 11 ส.ค.) จัด Jonathan SS, Cioccolata/Diavolo/Avdol A+ — **ล้าสมัยแล้ว**

### 5.2 ตารางบิลด์ทุกตัว (จาก Hideout; ค่าดาว/Gems/Spirit Power รายตัวไม่มีแหล่งให้ — ดูหมายเหตุ)
| ตัวละคร | Rarity | สไตล์ | Tier | PvE | ต้นเกม (Scene / Badge) | กลางเกม | ปลายเกม |
|---|---|---|---|---|---|---|---|
| Akira Otoishi | SR | Agility | Tier D | Tier D | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) | Do Something / Avdol Badge (Mythic ★1×4+10) |
| Anjuro Katagiri | R | Special | Tier D | Tier D | Stone Ocean / Leaky Eye Luca Badge (Epic ★2×4+5) | Stone Ocean / Johngalli A. Badge (Legendary ★2×4+8) | Stone Ocean / Caesar Badge (Mythic ★1×4+10) |
| Bruford | R | Assault | Tier D | Tier D | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | – | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) |
| Bruno Bucciarati | SSR | Agility | Tier S | Tier S | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) | The Greatest High Known to Man! / Avdol Badge (Mythic ★1×4+10) |
| Caesar Anthonio Zeppeli | SSR | Ranged | Tier S | Tier S | Stone Ocean / Shigekiyo Yangu Badge (Epic ★2×4+5) | Stone Ocean / Johngalli A. Badge (Legendary ★2×4+8) | Do Something / Caesar Badge (Mythic ★1×4+10) |
| Chaka | SR | Assault | Tier D | Tier D | The Taste of a Lie / Leaky Eye Luca Badge (Epic ★2×4+5) | The Taste of a Lie / Kenzou Badge (Legendary ★2×4+8) | The Taste of a Lie / Akira Otoishi Badge (Legendary ★2×4+8) |
| Cioccolata | SSR | Special | Tier C | Tier C | Do Something / Leaky Eye Luca Badge (Epic ★2×4+5) | – | Do Something / Johngalli A. Badge (Legendary ★2×4+8) |
| Diavolo | SSR | Agility | Tier A | Tier B | The Greatest High Known to Man! / Mariah Badge (Epic ★2×4+5) | Do Something / Akira Otoishi Badge (Legendary ★2×4+8) | Do Something / Avdol Badge (Mythic ★1×4+10) |
| Ermes Costello | SSR | Defense | Tier S | Tier A | – | – | I Decline / Secco Badge (Epic ★3×4+6) |
| F.F. | SSR | Ranged | Tier S | Tier S | Stone Ocean / Shigekiyo Yangu Badge (Epic ★2×4+5) | Stone Ocean / Keicho Nijimura Badge (Legendary ★2×4+8) | Do Something / Caesar Badge (Mythic ★1×4+10) |
| Formaggio | SR | Agility | Tier D | Tier D | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) | The Greatest High Known to Man! / Avdol Badge (Mythic ★1×4+10) |
| Ghiaccio | SR | Defense | Tier D | Tier D | – | – | I Decline / Secco Badge (Epic ★3×4+6) |
| Giorno Giovanna | SSR | Support | Tier S | Tier S | – | Do Something / Johngalli A. Badge (Epic ★1×4+4) | – |
| Guido Mista | SR | Ranged | Tier B | Tier C | Stone Ocean / Leaky Eye Luca Badge (Epic ★2×4+5) | Stone Ocean / Johngalli A. Badge (Legendary ★2×4+8) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Gwess | R | Agility | Tier D | Tier D | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) | The Greatest High Known to Man! / Avdol Badge (Mythic ★1×4+10) |
| Hol Horse | SR | Ranged | Tier A | Tier A | – | Do Something / Johngalli A. Badge (Epic ★1×4+4) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Iggy | SSR | Defense | Tier S | Tier A | – | – | I Decline / Iggy Badge (Protection Every 3 seconds in battle, grants a shield equal to 20% of the equipper's Defense to the ally with the lowest HP percentage, lasting 5 seconds. When the equipper is defeated, grants this shield to all surviving allies.) |
| Imposter Captain Tennille | SR | Special | Tier B | Tier B | – | Do Something / Johngalli A. Badge (Epic ★1×4+4) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Johngalli A. | SR | Ranged | Tier D | Tier D | – | Do Something / Johngalli A. Badge (Epic ★1×4+4) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Jonathan Joestar | SSR | Defense | Tier D | Tier D | – | – | I Decline / Secco Badge (Epic ★3×4+6) |
| Joseph Joestar | SR | Support | Tier A | Tier A | The Taste of a Lie / Bucciarati Badge (Epic ★1×4+4) | – | The Taste of a Lie / Kenzou Badge (Legendary ★2×4+8) |
| Jotaro Kujo | SSR | Assault | Tier S | Tier S | I Cast Aside My Humanness / Kenzou Badge (Flurry Only activates when equipped by a Melee character. Basic attacks deal additional damage equal to 10% of the equipper's Attack and increase the equipper's Crit Rate by 2% for 10 seconds. Cooldown: 10 seconds.) | – | The Greatest High Known to Man! / Jotaro Badge (Star Only activates when equipped by a Melee character. Basic attacks have a 20% chance to Stun the target for 1 second and deal additional damage equal to 20% of Attack. Cooldown: 4 seconds.) |
| Keicho Nijimura | SR | Ranged | Tier B | Tier D | Stone Ocean / Shigekiyo Yangu Badge (Epic ★2×4+5) | Stone Ocean / Hol Horse Badge (Legendary ★2×4+8) | Stone Ocean / Caesar Badge (Mythic ★1×4+10) |
| Kenzou | SR | Support | Tier A | Tier A | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) | – |
| Koichi Hirose | SSR | Special | Tier S | Tier S | – | Do Something / Johngalli A. Badge (Epic ★1×4+4) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Lang Rangler | SR | Support | Tier D | Tier D | Stone Ocean / Leaky Eye Luca Badge (Epic ★2×4+5) | Stone Ocean / Johngalli A. Badge (Legendary ★2×4+8) | Stone Ocean / Caesar Badge (Mythic ★1×4+10) |
| Leaky-Eye Luca | R | Assault | Tier D | Tier D | The Greatest High Known to Man! / Mariah Badge (Epic ★2×4+5) | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) | The Greatest High Known to Man! / Avdol Badge (Mythic ★1×4+10) |
| Leone Abbacchio | SR | Defense | Tier D | Tier D | – | – | I Decline / Secco Badge (Epic ★3×4+6) |
| Lisa Lisa | SR | Assault | Tier A | Tier D | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | – | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) |
| Mariah | R | Support | Tier D | Tier D | Stone Ocean / Leaky Eye Luca Badge (Epic ★2×4+5) | Stone Ocean / Johngalli A. Badge (Legendary ★2×4+8) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Mario Zucchero | SR | Agility | Tier D | Tier D | Do Something / Leaky Eye Luca Badge (Epic ★2×4+5) | – | Do Something / Akira Otoishi Badge (Legendary ★2×4+8) |
| Melone | SR | Agility | Tier D | Tier D | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | – | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) |
| Muhammad Avdol | SSR | Special | Tier A | Tier C | – | Stone Ocean / Johngalli A. Badge (Epic ★1×4+4) | Stone Ocean / Caesar Badge (Mythic ★1×4+10) |
| Narancia Ghirga | SR | Special | Tier C | Tier D | – | Do Something / Johngalli A. Badge (Epic ★1×4+4) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| N'Doul | SR | Agility | Tier D | Tier D | – | Do Something / Johngalli A. Badge (Epic ★1×4+4) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Noriaki Kakyoin | SSR | Ranged | Tier S | Tier S | – | – | Stone Ocean / Kakyoin Badge (Hawk-Eye Only activates when equipped by a Ranged character. The equipper gains 3,250 Crit Boost Up and their basic attacks have a 2% better chance to land critical hits.) |
| Pesci | R | Support | Tier B | Tier D | – | Do Something / Johngalli A. Badge (Epic ★1×4+4) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Pet Shop | SR | Special | Tier D | Tier D | Do Something / Johngalli A. Badge (Epic ★1×4+4) | – | Stone Ocean / Johngalli A. Badge (Legendary ★2×4+8) |
| Prosciutto | SSR | Assault | Tier S | Tier A | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) | The Greatest High Known to Man! / Avdol Badge (Mythic ★1×4+10) |
| Robert E. O. Speedwagon | SR | Support | Tier A | Tier A | Stone Ocean / Leaky Eye Luca Badge (Epic ★2×4+5) | Stone Ocean / Johngalli A. Badge (Legendary ★2×4+8) | The Hymn of Bravery / Blueford Badge (Epic ★2×4+5) |
| Rubber Soul | R | Defense | Tier B | Tier D | – | – | I Decline / Secco Badge (Epic ★3×4+6) |
| Rudol von Stroheim | SR | Defense | Tier D | Tier D | The Hymn of Bravery / Speedwagon Badge (Epic ★3×4+6) | I Decline / Stroheim Badge (Legendary ★2×4+8) | I Decline / Jonathan Badge (Mythic ★1×4+10) |
| Sale | R | Ranged | Tier D | Tier D | – | Do Something / Johngalli A. Badge (Epic ★1×4+4) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Santana | SR | Defense | Tier D | Tier D | – | – | I Decline / Secco Badge (Epic ★3×4+6) |
| Secco | SR | Assault | Tier D | Tier D | The Taste of a Lie / Bucciarati Badge (Epic ★1×4+4) | The Greatest High Known to Man! / Akira Otoishi Badge (Legendary ★2×4+8) | The Greatest High Known to Man! / Avdol Badge (Mythic ★1×4+10) |
| Shigekiyo Yangu | R | Special | Tier D | Tier D | Do Something / Leaky Eye Luca Badge (Epic ★2×4+5) | Do Something / Johngalli A. Badge (Legendary ★2×4+8) | The Taste of a Lie / Koichi Hirose Badge (Mythic ★1×4+10) |
| Sports Maxx | SR | Assault | Tier D | Tier D | The Taste of a Lie / Leaky Eye Luca Badge (Epic ★2×4+5) | The Taste of a Lie / Anubis Badge (Legendary ★2×4+8) | The Taste of a Lie / Ermes Badge (Mythic ★1×4+10) |
| Squalo | R | Agility | Tier D | Tier D | Stone Ocean / Leaky Eye Luca Badge (Epic ★2×4+5) | Do Something / Johngalli A. Badge (Legendary ★2×4+8) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Straizo | R | Agility | Tier D | Tier D | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | Do Something / Akira Otoishi Badge (Legendary ★2×4+8) | Do Something / Avdol Badge (Mythic ★1×4+10) |
| Tarkus | SR | Assault | Tier D | Tier D | – | Do Something / Johngalli A. Badge (Epic ★1×4+4) | Do Something / Koichi Hirose Badge (Mythic ★1×4+10) |
| Tonio Trussardi | SR | Support | Tier A | Tier A | – | – | The Final Hamon / Giorno Badge (Inspiration Upon entering battle and casting the Ultimate, grants all allies a Shield equal to 2% of the equipper's Max HP and 2 stacks of Attack Up for 10 seconds.) |
| Viviano Westwood | SR | Assault | Tier D | Tier D | The Greatest High Known to Man! / Mariah Badge (Epic ★2×4+5) | The Taste of a Lie / Akira Otoishi Badge (Legendary ★2×4+8) | The Taste of a Lie / Ermes Badge (Mythic ★1×4+10) |
| Will A. Zeppeli | SR | Support | Tier D | Tier D | The Greatest High Known to Man! / Leaky Eye Luca Badge (Epic ★2×4+5) | The Greatest High Known to Man! / Anubis Badge (Legendary ★2×4+8) | The Hymn of Bravery / Giorno Badge (Mythic ★1×4+10) |


**หมายเหตุสำคัญ**
- Badge ในตารางเป็นรูป "ชื่อ Badge (เกรด ★×4 + ระดับยกขั้น)" ตามต้นฉบับ; ค่าตัวเลขสกิลดู [badges.md](badges.md); ต้นเกมมัก = Epic ★2, กลาง = Legendary ★2, ปลาย = Mythic ★1
- ต้นฉบับ Hideout **ไม่ระบุ**: ดาวขั้นต่ำ/เป้าหมายรายตัว, Gems ที่แนะนำ, Spirit Power — **ไม่พบข้อมูลจากแหล่งที่อ่าน** (ข้อมูลที่ไกด์อื่นให้: Diavolo อย่างน้อย 3★ + Gem of Fury 🔎 ไกด์ allthings.how; ที่เหลือไม่ยืนยัน)
- บิลด์ R/SR ระดับล่างจำนวนมากเป็นแม่แบบซ้ำของ Hideout → ใช้เป็นแนวทางหยาบ
- ทีมที่เข้ากันรายตัวอยู่ใน [characters.md](characters.md) (หัวข้อ "ทีมที่เข้ากัน")

### 5.3 บิลด์ตัวเด่นแบบอ่านง่าย (อ้างจาก Hideout/Codex/ไกด์ก่อนหน้า)
| ตัวละคร | บทบาท | เซต Scene | Badge | จุดเด่น |
|---|---|---|---|---|
| **Jotaro** (S) | Assault DPS | *Greatest High* 4 ชิ้น (ATK) | Jotaro/Kenzou Badge | Ultimate หยุดเวลา; เริ่ม 700/1,000 energy; ลด DEF เป้า 6% 6 วิ |
| **Caesar** (S) | Ranged AoE/คุม | *Stone Ocean* → endgame *Do Something* | ต้นเกม Shigekiyo → Johngalli → **Caesar Badge** (Mythic); หรือ Hol Horse (บอส)/Keicho (คลื่น) | Bubble Barrier ตรึง, Ripple ได้เปรียบ Vampire/Zombie, สเกล AS |
| **Giorno** (S) | Support ฮีล+Energy | *Hymn of Bravery*/*Final Hamon* | **Giorno Badge** | ฮีลเป้า HP ต่ำสุด + โล่สะท้อน + พลังงานทั้งทีมต้นสนาม — กาวทุกทีม |
| **Bucciarati** (S) | Agility เปิดเกม/คุม | *Greatest High* หรือ *Taste of a Lie* | Leaky-Eye→Akira→**Avdol** | Unzip/Zipper Space สตัน/ลบเป้าออกจากสนาม |
| **F.F.** (S) | Ranged summoner | *Stone Ocean* → *Do Something* | Shigekiyo→Keicho→**Caesar** | Plankton Colony carry; +ดาเมจต่อ Damp |
| **Koichi** (S) | Special คุม/แท็งก์ | เซต Attack 4 ชิ้นตามไกด์ (⚠️ ขัดกับบทบาทแท็งก์ — ตรวจในเกม) | Koichi Badge (Ranged only) | คุม+ปั่น energy, ยุคแรกมองว่าเป็นแท็งก์ที่ดีที่สุด |
| **Ermes** (S/PvE A) | Defense | *I Decline* | Secco Badge (Epic ★3×4+6) | โล่แชร์พันธมิตร, ทนสุด |
| **Iggy** (S) | Defense | — | Iggy Badge | HP/ATK ต่ำสุดในเกม แต่ซัพพอร์ตเกราะแรง (โล่ 160% DEF) |
| **Prosciutto** (S/PvE A) | Assault | — | — | ถูกกดตอน Blizzard แรงขึ้นตอนร้อนจัด |
| **Diavolo** (A/PvE B) | Agility assassin | *Greatest High* → *Do Something* | Mariah → Akira → **Avdol** | Stealth ต้นสนาม; Isolation; ดาเมจ +30–50% ของ HP ที่ขาด (cap 500% ATK) |
| **Hol Horse** (A) | Ranged DPS | — | Hol Horse Badge | อัลติ 10 นัดแบบ channel (ถูก CC ขัดได้) |
| **Joseph (SR)** (A) | Support | — | Joseph Badge | ฟรี; ดึง/สตัน เข้าชุดกับ Caesar+Koichi |

## 6. ลำดับการลงทรัพยากรตามช่วงเกม 📖/🔎

**มือใหม่ (Account Lv.1–12)**: เล่นเนื้อเรื่อง Golden Wind (ปลดโหมด + แจกตั๋วสุ่ม) → ใช้ Astrogem ตู้ Standard Character ก่อน → ทำเควสรายวัน (Adventure Progress ให้ XP มากสุด) → ส่ง SPW Request ทุกเช้า → ทีม 4–5 ตัวสมดุล (ดาเมจ/แท็งก์/ฮีล) → Badge เซต Rare/Epic ราคาถูก (Mariah/Bruford/Straizo/Gwess)
**กลางเกม (Lv.13–60)**: เปิด Spirit Board ผ่าน Double Clash; ทำ Extreme Trial ไล่ Lv.20→60 เก็บเซต; Star-up แครี่; ออมเข้า 180 selector (เลือก Caesar/Koichi/Ermes ถ้ายังไม่มี); ประจำวัน = World Boss (10 รอบ/วัน), Interview Trial, SPW, Extreme Trial, Arena, Double Clash, Guild Training
**ปลายเกม (Lv.60+/Lv.100)**: Extreme Trial Team Lv.100 → Outstanding Scene + Camrecorder → Favorite (+16/+20); Badge โปรโมตสู่ Legendary/Mythic (Blueprint จาก Monthly Pass/Boss Store); Star Tree เฉพาะตัวที่เก็บยาว; Ranked/Arena ดัน Apex; ปลายเกม World Boss ล็อก Lv.100 ทุกตัว → ผลขึ้นกับบิลด์และการวางทีม ไม่ใช่เลเวล

**เงินเติม/F2P**: คุ้มสุดที่ Monthly Pass (Premium) — ได้ Token ซื้อ Blueprint Jotaro/Koichi/Giorno (ตัวละ 200, ซื้อได้ 4), Uncharted Fate ×5 (30 token), Stone of Destiny; Voyager Pack I–VI (ชุดเติมตามขั้น). F2P: ได้ Joseph SR ฟรี, ตู้ Novice เลือก SSR, selector 180/300, Selection Shard 60 ชิ้น

## 7. สรุปจาก YouTube — **ไม่สามารถทำได้ในรอบนี้**
- ที่ทำได้: เก็บ metadata + chapters + description ของคลิป (ดู [youtube/index.md](youtube/index.md)) ซึ่งช่วยหา "หัวข้อที่ต้องดูต่อ" ได้ เช่น คลิป WG:B "How to Build EVERY SSR" ยาว 44 นาที มี 11 บท
- ที่ทำไม่ได้: transcript → สกัดบิลด์รายตัว — เพราะ YouTube ตอบ 429 ต่อ endpoint ซับไตเติลจาก IP เครื่องนี้ (ตั้ง sleep 5–20 วิ, อัปเดต yt-dlp 2026.10.26 แล้ว ยังเกิด) ห้ามใช้วิธีหลบการตรวจจับ → **แนะนำ**: ลองรันซ้ำภายหลัง/จากเครือข่ายอื่นด้วย `yt-dlp --skip-download --write-auto-subs --sub-langs "en.*" <url>` หรือเปิดคลิปที่ลิงก์ในตารางแล้วอ่าน transcript จากหน้าเว็บเอง

## 8. แหล่งอ้างอิง
ดู [sources.md](sources.md)
