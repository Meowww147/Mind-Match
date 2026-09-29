Mind Match — วิธีใช้งาน

เปิด index.html ในเบราว์เซอร์เพื่อเล่น หรืออัปโหลดทั้งโฟลเดอร์ขึ้นโฮสต์เว็บ (เช่น GitHub Pages) โดยคงโครงสร้าง images/ ไว้

รูปสัตว์อยู่ที่ images/animals/ รูปอาหารอยู่ที่ images/food/ และรูปผลไม้อยู่ที่ images/fruits/ เป็น PNG พื้นหลังโปร่งใสทั้งหมด
หากต้องการเปลี่ยนรูปเดิม ให้นำ PNG ใหม่มาแทนที่ไฟล์ชื่อเดิมในโฟลเดอร์นั้น

หากจะเพิ่มหมวดใหม่:
1. สร้างโฟลเดอร์ images/fruits/ แล้วใส่ภาพ PNG 10 ภาพ เช่น apple.png, banana.png ฯลฯ
2. เปิด index.html และเพิ่มบรรทัดใน CATEGORIES ดังตัวอย่าง:
   Fruits: ['apple','banana','grape','orange','mango','pineapple','watermelon','durian','longan','mangosteen'].map(name => `images/fruits/${name}.png`),
3. ตรวจว่าชื่อทุกไฟล์ตรงกับรายการในโค้ด และมีรูปไม่ซ้ำกัน 10 รูป

โลโก้เปลี่ยนได้โดยแทนที่ images/logo.png
เกมจะสุ่มเฉพาะหมวดที่มีรายการอยู่ใน CATEGORIES จึงเล่นได้ทันทีด้วยหมวด Animals, Food และ Fruits
