โปรเจคนี้เป็นเกม **2D Escape** ที่เขียนด้วย **JavaScript + HTML5 Canvas + css**  
ผู้เล่นต้องบังคับตัวละคร (Player) หลบหนี Killer พร้อมหาทางออก (Exit) โดยไม่ถูกฆ่า หรือเหยียบกับดัก (Trap)

---

## 🎮 วิธีการเล่น
- ใช้ปุ่ม **W A S D** เพื่อบังคับตัวละคร
  - `W` = ขึ้น
  - `S` = ลง
  - `A` = ซ้าย
  - `D` = ขวา
- เป้าหมายคือไปถึง **Exit (รูทางออก)** โดยไม่ให้ Killer ตามจับได้
- ถ้า Player เหยียบ **Trap** → Killer จะได้เทิร์นเดินทันที
- Killer ใช้ **A* Pathfinding Algorithm** ไล่ล่า Player
- หาก Player เดินไปชน Killer → **Game Over!**
- หาก Player เดินถึง Exit → **You Win!**

---

## 🧩 ฟีเจอร์
- **Random Spawn System** → Player, Killer, Exit จะสุ่มเกิดในตำแหน่งที่ไม่ชนกัน
- **A* Pathfinding** → Killer คำนวณเส้นทางสั้นที่สุดเพื่อตาม Player
- **Trap System** → ถ้า Player เหยียบกับดักจะเสียเทิร์นทันที
- **Footstep Trail** → แสดงรอยการเคลื่อนที่ของ Killer
- **Reset Game** → สามารถรีเซ็ตตำแหน่งใหม่ได้

---

## 🛠️ เทคโนโลยีที่ใช้
- **HTML5 Canvas** สำหรับการวาดเกม
- **Vanilla JavaScript** ควบคุมการเล่น, Logic ของเกม
- **A* Algorithm** ระบบ AI ของ Killer
- **css** ตกแต่งหน้า UI