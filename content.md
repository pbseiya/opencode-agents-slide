# OpenCode + Oh My OpenAgent
## คู่มือเลือกใช้ Agent ให้ถูกต้อง

---

## สไลด์ 1: ทำไมต้องรู้จัก Agent?

OpenCode มี AI Agents หลายตัวช่วยเขียนโค้ด
- ถ้าเลือกถูก = งานเสร็จเร็ว ไม่เปลืองเครดิต
- ถ้าเลือกผิด = agent ทำงานซ้ำ เสียเวลา ตอบคำถามวนไปมา

---

## สไลด์ 2: Agent มีกี่ตัว?

ระบบแบ่งเป็น 3 ระดับ:

1. Agents (สั่งการระดับสูง)
   - Sisyphus - ตัวเริ่มต้น
   - Prometheus - วางแผน
   - Atlas - ลงมือทำ
   - Hephaestus - คิดลึก

2. Core Agents (แบ่งประเภทงาน)
   - core_research, core_explore, core_development

3. Tools (ลงมือทำจริง)
   - terminal, file, code_execution

---

## สไลด์ 3: กฎทอง

ลำดับความสำคัญ: Agents > Core > Tools

อย่าเลือก Tools เอง
ให้ Agents ตัดสินใจสั่งการอัตโนมัติ

---

## สไลด์ 4: Sisyphus — ตัวเริ่มต้น

ใช้เมื่อ: งานง่าย แก้ไฟล์เดียว รู้ว่าต้องทำอะไร

วิธีใช้:
- เปิด OpenCode TUI คือ Sisyphus อยู่แล้ว
- พิมพ์คำสั่งตรงๆ ได้เลย

ทางลัด:
- พิมพ์ ultrawork หรือ ulw
- ให้ agent ทำงานอัตโนมัติจนเสร็จ

---

## สไลด์ 5: Prometheus — ผู้วางแผน

ใช้เมื่อ: งานใหญ่ ไม่แน่ใจ scope

ขั้นตอน:
1. กด Tab ที่ prompt เลือก Prometheus
2. ตอบคำถาม Interview กำหนดขอบเขต
3. อนุมัติแผนที่ agent สร้างให้
4. พิมพ์ /start-work

Prometheus จะส่งต่อให้ Atlas ลงมือทำ

---

## สไลด์ 6: Hephaestus — ผู้คิดลึก

ใช้เมื่อ: Debug ลึก หรือ Research ข้ามหลายไฟล์

สัญญาณที่ต้องเรียก:
- Agent ตัวอื่น ติดปัญหาไม่รู้สาเหตุ
- ต้องค้นคว้า domain ที่ไม่คุ้นเคย
- ต้อง redesign กระทบหลายส่วน

วิธีเรียก: กด Tab ที่ prompt เลือก Hephaestus

---

## สไลด์ 7: ตารางตัดสินใจ

| งาน | Agent |
|-----|-------|
| แก้ typo | Sisyphus |
| ทำ feature ใหม่ | Prometheus -> Atlas |
| Refactor ใหญ่ | Prometheus -> Atlas -> Hephaestus |
| ไม่รู้ต้องทำอะไร | Prometheus (interview) |
| Debug ลึก | Hephaestus |
| ขี้เกียจอธิบาย | ultrawork |

---

## สไลด์ 8: สิ่งไม่ควรทำ

- อย่าเริ่มที่ Atlas โดยตรง ถ้าไม่มีแผน
- ไม่ต้องเรียก Oracle เอง Sisyphus จะเรียกให้อัตโนมัติ
- อย่าพยายามเลือก Core/Tools เอง

---

## สไลด์ 9: สรุปง่ายๆ

งานเล็ก -> Sisyphus ตรงๆ
งานกลาง -> Sisyphus + ultrawork
งานใหญ่ -> Prometheus -> Atlas

คิดลึก -> เพิ่ม Hephaestus

เลือกให้ถูก งานเสร็จไว ไม่เสียเวลา
