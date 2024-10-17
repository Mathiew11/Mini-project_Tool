# DADS5001 Miniproject - 18/10/2024
 
## TOPIC: วิเคราห์พฤติกรรมผู้เล่น League of Legends เพื่อหากลยุทธ์สำหรับการเล่นให้ชนะ
 
### BY:

- Pakawat Naktubtee (STD ID: 6620422021)

- Kittitat Wattanasuntikul (STD ID: 6620422025)
 
### DATASET:[League of Legends Dataset](https://www.kaggle.com/datasets/delfinaoliva/league-of-legends-champspopularity-winrate-kda/data)
 
---

![League of Legends Logo](https://github.com/user-attachments/assets/9eb4573e-0e91-4c84-8dbb-dfe8fdde681b)
 
**League of Legends (LoL)** เป็นเกมแนว **MOBA (Multiplayer Online Battle Arena)** ที่ได้รับความนิยมเป็นอย่างมากและติดอันดับ **Top 2** ของโลก โดยมีผู้เล่นนับล้านคนจากทุกมุมโลก ทั้งนี้ความนิยมของ LoL เกิดจากองค์ประกอบหลายอย่าง เช่น:
 
- **การแข่งขันที่เข้มข้น**: ด้วยความเป็นเกมที่ต้องใช้ทักษะการเล่นสูง ผสมผสานกับกลยุทธ์ที่หลากหลาย LoL กลายเป็นเกมที่ถูกใช้ในการแข่งขันระดับโลกอย่างต่อเนื่อง

- **eSports ระดับโลก**: การแข่งขัน **LoL World Championship** และทัวร์นาเมนต์ระดับประเทศต่าง ๆ ทำให้ LoL มีบทบาทสำคัญในวงการ **eSports** และมีผู้ชมทั่วโลกติดตามเป็นจำนวนมาก

- **แชมเปี้ยนที่หลากหลาย**: ด้วยการออกแบบแชมเปี้ยนที่หลากหลาย ทำให้ผู้เล่นสามารถเลือกใช้ตัวละครที่ตรงกับสไตล์การเล่นของตัวเอง ซึ่งสร้างความสนุกและความท้าทายใหม่ ๆ ในแต่ละเกม

- **การอัปเดตและการปรับปรุงอย่างต่อเนื่อง**: Riot Games, ผู้พัฒนาเกม LoL, ให้ความสำคัญกับการปรับปรุงและพัฒนาเกมอย่างต่อเนื่อง ไม่ว่าจะเป็นการเพิ่มแชมเปี้ยนใหม่ หรือปรับสมดุลของเกมเพื่อให้เกมยังคงน่าตื่นเต้นและสนุกสนานอยู่เสมอ

- **ชุมชนผู้เล่นที่แข็งแกร่ง**: LoL มีฐานผู้เล่นที่กว้างขวางและชุมชนผู้เล่นที่คอยแบ่งปันความรู้ เทคนิค และกลยุทธ์ในการเล่น
 
ด้วยปัจจัยเหล่านี้ ทำให้ LoL ยังคงเป็นเกมที่อยู่ในใจของผู้เล่นหลายคนและเป็นหนึ่งในเกมที่ได้รับความนิยมสูงสุดในโลก MOBA
 
---
 
### Quest and Answer:

1. **คำถาม**: จำนวนการเปิดตัวแชมเปียนมีการเปลี่ยนแปลงอย่างไรในแต่ละปี?
 
   ![image](https://github.com/user-attachments/assets/12f2118f-57a3-4c4f-b07f-fe2ee496b48b)
 
   - **คำตอบ**: จากกราฟแสดงให้เห็นเทนด์ของการปล่อยตัว Champion ใหม่ๆของ LoL โดยในช่วงปี 2009-2012 มีการเพิ่มจำนวน Champion ที่มากกว่า 10 ตัว แต่หลังจากปี 2013 ทางผู้พัฒนาก็ได้ลดจำนวน Champion ใหม่ๆลง เหลือปีละไม่เกิน 10 ตัว เพื่อเอาเวลาไปพัฒนาในส่วนอื่นๆเพิ่มเติม คิดว่ามีส่วนสำคัญอย่างมากเนื่องจากการเพิ่ม Champion ตัวใหม่ๆขึ้นมาทำให้มีความแปลกใหม่ทำให้เป็นที่สนใจของผู้เล่นใหม่ และทำให้ผู้เล่นเก่ามีแผนการเล่นเพิ่มเติม โดยในช่วงที่มีฐานผู้เล่นเริ่มเยอะขึ้นแล้วก็ได้ลดจำนวนการปล่อย Champion ใหม่ๆลงแต่หันไปเพิ่มคุณภาพ ในส่วนอื่นๆแทน
 
2. **คำถาม**: ตำแหน่งใดมีจำนวน Champion มากที่สุดและมีจำนวนเท่าไหร่?

![image](https://github.com/user-attachments/assets/be498181-8343-4de6-bb4f-510bf218efac)

   - **คำตอบ**: จำนวน Champion ทั้งหมดของ LoL มี 168 ตัว
Barchart แสดงให้เห็นถึงจำนวน Champions ที่ถูกเลือกในแต่ละ Role โดย Top-lane มีจำนวน Champion เยอะที่สุดใกล้เคียงกับ Mid-lane ที่เหลือรองลงมาส่วน Bottom-lane หรือ Carry มีน้อยที่สุด

  Key takeaway:

  - มี Champions หลายตัวที่สามารถเล่นได้มากกว่า 1 ตำแหน่ง

  - Champions ที่ถูกเลือกในตำแหน่ง Bottomlane มี spec unflexible จึงมีจำนวนน้อยที่สุด

  - Champions ที่ถูกเลือกในตำแหน่ง Toplane และ Midlane มีความ flexible สูงเห็นได้จากมี Champions หลากหลายตัวถูกเลือกในตำแหน่งนี้
 

3.**คำถาม**: Champion ที่มี win-rate สูง มักจะมี ban-rate และ popularity สูงด้วย?

   - **คำตอบ**
     
![image](https://github.com/user-attachments/assets/45bc0f58-99ec-4d9c-8e76-6fd129c66b31)

กราฟนี้แสดงให้เห็นถึงการกระจายตัวของ win-rate, ban-rate และ popularity ของ Champion ทุกตัวในเกม

![image](https://github.com/user-attachments/assets/c7be60c0-e531-430d-a62e-776f33cf2273)     

   จาก Graph Correlation Heatmap แสดงให้เห็นว่า win-rate กับ ban-rate มีความสัมพันธ์เชิงลบ ซึ่งหมายถึง อัตราการชนะไม่มีความเกี่ยวข้องกับการถูกแบน 
   นอกจากนี้กราฟยังแสดงให้เห็นถึง ค่าความสัมพันธ์เชิงบวกระหว่าง ban-rate กับ popularity ซึ่งหมายถึง Champion ที่มีความนิยมสูงมักจะมีอัตราการถูกแบนสูงด้วย

![image](https://github.com/user-attachments/assets/719c5678-94eb-443e-9a0e-b19ae4cf2d3c)

จากค่าในตารางแสดงให้เห็นว่าใน Champion 10 อันดับแรกที่มีอัตราการชนะสูงสุด  มี Champion 9 อันดับที่มีอัตราการชนะสูง แต่มีอัตราการถูกแบนต่ำ

จากสมมติฐาน: Champion ที่มี win-rate สูง น่าจะมี ban-rate สูงตามไปด้วย ไม่ถูกต้อง ทำให้เราสงสัยว่า Champion ประเภทไหนที่ผู้เล่นเกมส์ LoL มักจะแบน?

![image](https://github.com/user-attachments/assets/be9e4303-0c3f-42f9-80da-0a29a534012f)

จากกราฟ Average Banrate by Champion Tag แสดงให้เห็นว่าผู้เล่นมักจะเลือกแบน Champion ประเภท Artillery มากที่สุด Diver และ Assasin รองลงมาตามลำดับ ซึ่งหมายถึงผู้เล่นไม่ชอบ Champion ที่โจมตีได้รุนแรงในระยะไกล และ Champion ที่มีความคล่องแคล่ว สามารถเข้าประชิดตัว ทำดาเมจได้รุนแรงและรวดเร็ว

เช่นเดียวกัน จากสมมติฐาน: Champion ที่มี win-rate สูง น่าจะมี popularity สูงตามไปด้วย ไม่ถูกต้อง ทำให้เราสงสัยว่า Champion ประเภทไหนที่ผู้เล่นเกมส์ LoL มักนิยมเล่นมากที่สุด?

![image](https://github.com/user-attachments/assets/9a2fae71-6ca8-45fc-ac8d-2393b380fa46)

จากกราฟ Average Popularity by Champion Tag แสดงให้เห็นว่าผู้เล่นมักจะเลือกเล่น Champion ประเภท Artillery, Marksman, Skirmisher และ Assassin ตามลำดับ ซึ่งจากทั้ง 4 ประเภทของ Champion แสดงให้เห็นว่า ผู้เล่นเกมนี้มักจะชอบเล่น Champion ที่ทำดาเมจได้รุนแรง

---
**สรุป**
จาก story telling ทั้งหมดที่กล่าวมาจะพบว่าพฤติกรรมของผู้เล่นเกมนี้ มักจะชอบแบนและเลือกเล่น Champion ทีเป็นเอกลักษณ์โดยไม่สนใจความเก่ง(win-rate)ของ Champion ตัวนั้นๆ ทำให้เราได้กลยุทธ์การเล่นเพื่อให้ได้รับชัยชนะดังนี้

- ต้องฝึกฝนการเล่น Champion ประเภท Artillery, Diver และ Assasin ซึ่งเป็น Champion ที่ผู้เล่นส่วนมากไม่ชอบแต่ก็มีโอกาสสูงที่จะถูกแบน หรือถูกแย่งเลือกโดยผู้เล่นอีกฝั่ง

- ต้องฝึกฝน Champion ที่มีอัตราการชนะสูงๆ เนื่องจากเป็น Champion ที่มีอัตราการแบนต่ำ และมีความนิยมน้อย ทำให้มีโอกาสที่จะเลือกนำมาเล่นได้สูง

---
**Challenge and Improvement**

- dataset มีจำนวน column เยอะ ทำให้ต้องใช้เวลาในการเลือก scope ว่าจะนำ dimention ไหนมาเพื่อทำ story telling บ้าง

- ต้องมีการทำ data cleansing บาง column เช่น การแปลง str ให้เป็น float และมีประเภทของ Champion บางตัวที่เขียนไม่เหมือนกัน เช่น Assasin กับ Assassin

- การเติมรายละเอียดในกราฟ ทำให้ต้องศึกษา library เพิ่มเติม เพื่อนำมาเติมรายละเอียดลงในกราฟให้ครบถ้วน

- หากมีข้อมูลเพิ่มเติมจะสามารถวิเคราะห์หา insight ออกมาได้มีประสิทธิภาพมากกว่านี้ เช่น ข้อมูลเฉพาะกลุ่มผู้เล่น SEA หรือข้อมูลเฉพาะกลุ่มของผู้เล่นมืออาชีพ
