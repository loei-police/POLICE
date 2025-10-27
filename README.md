# POLICEPOLICE
```
OLICEายชื่อแหล่งข้อมูลหล่งรวมข้อมูล
แหล่งรวมข้อมูล
รายชื่อแหล่งข้อมูล ยชื่อแหล่งข้อมูล LLM/VLM/VLA ที่ยอดเยี่ยมสำหรับการขับขี่อัตโนมัติ (LLM4AD) ที่คัดสรรมาอย่างดี (อัปเดตอย่างต่อเนื่อง)

ใบอนุญาต
 ใบอนุญาต Apache-2.0
 1.5k ดาว
 85 ส้อม
 50 คน กำลังดู
 1 สาขา
 0 แท็ก
 กิจกรรม
 คุณสมบัติที่กำหนดเอง
คลังเก็บข้อมูลสาธารณะ
Thinklab-SJTU/สุดยอด-LLM4AD
ชื่อ	
เจย์ยัง0802
เจย์ยัง0802
3 months ago
สินทรัพย์
2 years ago
ใบอนุญาต
2 years ago
README.md
3 months ago
การนำทางไฟล์ที่เก็บข้อมูล
อ่านฉัน
ใบอนุญาต Apache-2.0
สุดยอด LLM สำหรับแหล่งข้อมูลการขับขี่อัตโนมัติ
สุดยอดดาวเด่นของ GitHub GitHub ฟอร์ก ใบอนุญาต GitHub

นี่คือชุดบทความวิจัยเกี่ยวกับหลักสูตร LLM-for-Autonomous-Driving (LLM4AD)คลังข้อมูลนี้จะได้รับการอัปเดตอย่างต่อเนื่องเพื่อติดตามความก้าวหน้าของหลักสูตร LLM4AD (Large Language Models for Autonomous Driving) ซึ่งครอบคลุม VLM4AD (Vision-Language Models for AD) และ VLA4AD (Vision-Language Models for AD) ซึ่งเป็นองค์ประกอบสำคัญของกระบวนทัศน์แบบบูรณาการนี้ จัดทำโดย SJTU-ReThinklab

ยินดีต้อนรับกดติดตามและติดดาว! หากพบว่าเนื้อหาใด ๆ ที่เกี่ยวข้องอาจเป็นประโยชน์ โปรดติดต่อเรา ( yangzhenjie@sjtu.edu.cnหรือjiaxiaosong@sjtu.edu.cn ) หรือฝากประชาสัมพันธ์

การอ้างอิง
เอกสารการสำรวจของเราอยู่ที่https://arxiv.org/abs/2311.01043ซึ่งรวมถึงการอภิปรายโดยละเอียดเพิ่มเติมและจะได้รับการอัปเดตอย่างต่อเนื่อง

GitHub Pages ได้รับการอัปเดตเมื่อวันที่ 3 กรกฎาคม 2025

แบบสำรวจฉบับล่าสุดได้รับการอัปเดตเมื่อวันที่ 12 สิงหาคม 2024

หากคุณพบว่าที่เก็บข้อมูลของเรามีประโยชน์ โปรดพิจารณาอ้างอิง

@misc{yang2023survey,
      title={LLM4Drive: A Survey of Large Language Models for Autonomous Driving}, 
      author={Zhenjie Yang and Xiaosong Jia and Hongyang Li and Junchi Yan},
      year={2023},
      eprint={2311.01043},
      archivePrefix={arXiv},
      primaryClass={cs.AI}
}
สารบัญ
หลักสูตร LLM ที่ยอดเยี่ยมสำหรับการขับขี่อัตโนมัติ (LLM4AD)
สารบัญ
ภาพรวมของ LLM4AD
เอกสาร
ชุดข้อมูล
การอ้างอิง
ใบอนุญาต
ภาพรวมของ LLM4AD
LLM-for-Autonomous-Driving (LLM4AD) หมายถึงการประยุกต์ใช้ Large Language Models (LLMs) ในการขับขี่อัตโนมัติ เราแบ่งงานที่มีอยู่ตามมุมมองของการประยุกต์ใช้ LLM ได้แก่ การวางแผน การรับรู้ การตอบคำถาม และการสร้าง

ข้อมูลรูปภาพ

แรงบันดาลใจของ LLM4AD
วงกลมสีส้มแสดงถึงระดับความสามารถในการขับขี่ที่เหมาะสม ซึ่งเทียบเท่ากับความสามารถของผู้ขับขี่ที่มีประสบการณ์ มีสองวิธีหลักในการบรรลุความเชี่ยวชาญดังกล่าว วิธีแรกคือการเรียนรู้จากเทคนิคในสภาพแวดล้อมจำลอง และวิธีที่สองคือการเรียนรู้จากข้อมูลออฟไลน์ผ่านวิธีการที่คล้ายคลึงกัน สิ่งสำคัญที่ต้องทราบคือ เนื่องจากความคลาดเคลื่อนระหว่างการจำลองและโลกแห่งความเป็นจริง โดเมนทั้งสองนี้จึงไม่เหมือนกันโดยสิ้นเชิง นั่นคือช่องว่างระหว่างการจำลองกับโลกแห่งความเป็นจริง ในขณะเดียวกัน ข้อมูลออฟไลน์ก็ทำหน้าที่เป็นส่วนย่อยของข้อมูลโลกแห่งความเป็นจริง เนื่องจากรวบรวมโดยตรงจากสภาพแวดล้อมจริง อย่างไรก็ตาม การกระจายตัวของข้อมูลทั้งหมดนั้นทำได้ยาก เนื่องจากลักษณะหางยาวของงานขับขี่อัตโนมัติที่ขึ้นชื่อเรื่องการขับเคลื่อนแบบอัตโนมัติ เป้าหมายสุดท้ายของการขับขี่อัตโนมัติคือการยกระดับความสามารถในการขับขี่จากระดับพื้นฐานสีเขียวไปสู่ระดับสีน้ำเงินขั้นสูง ผ่านการรวบรวมข้อมูลอย่างละเอียดและการเรียนรู้เชิงลึก

ข้อมูลรูปภาพ

เอกสาร
สลับ
format:
- [title](paper link) [links]
  - author1, author2, and author3...
  - publisher
  - task
  - keyword
  - code or project page
  - datasets or environment or simulator
  - publish date
  - summary
  - metrics
แพลตฟอร์มการทดสอบแบบลำดับชั้นสำหรับโมเดลภาษาการมองเห็น (VLM) - การขับขี่อัตโนมัติในโลกแห่งความเป็นจริง

หยูเผิง โจว, คาน ชุย, จุนทง เผิง, จิจง หยาง, ฮวนหวู่ ลู่, จิเตช เอช. ปานชาล, ปิน เหยา, ซีราน หวาง
สำนักพิมพ์: มหาวิทยาลัยเพอร์ดู
วันที่เผยแพร่: 2025.06.17
งาน: การประเมินผล
สรุป:
เอกสารนี้จะแนะนำไปป์ไลน์มิดเดิลแวร์ที่มีน้ำหนักเบา มีโครงสร้าง และความหน่วงต่ำบนยานพาหนะ และพัฒนารูปแบบของสถานการณ์การจราจรในโลกแห่งความเป็นจริงที่ปรับแต่งได้บนแทร็กทดสอบแบบปิด
AutoVLA: โมเดลวิสัยทัศน์-ภาษา-การกระทำสำหรับการขับขี่อัตโนมัติแบบครบวงจรพร้อมการใช้เหตุผลเชิงปรับตัวและการปรับแต่งการเสริมแรง

Zewei Zhou, Tianhui Cai, Seth Z. Zhao, Yun Zhang, Zhiyu Huang, Bolei Zhou, Jiaqi Ma
สำนักพิมพ์: มหาวิทยาลัยแคลิฟอร์เนีย ลอสแองเจลิส
วันที่เผยแพร่: 2025.06.16
หน้าโครงการ: AutoVLA
รหัส: AutoVLA
ภารกิจ: การวางแผน
ชุดข้อมูล: nuPlan, nuScenes , Waymo, Bench2Drive (การใช้ชุดข้อมูล CARLA-Garageสำหรับการฝึกอบรม)
สรุป:
AutoVLA คือเฟรมเวิร์กการขับขี่อัตโนมัติแบบครบวงจรที่ใช้ประโยชน์จากโครงกระดูกสันหลัง VLM ที่ได้รับการฝึกอบรมไว้ล่วงหน้าซึ่งรวมเข้ากับโทเค็นการดำเนินการทางกายภาพที่แยกจากกัน
ใช้ GRPO เพื่อเปิดใช้งานการใช้เหตุผลเชิงปรับตัวและปรับปรุงประสิทธิภาพของโมเดลให้ดียิ่งขึ้นในภารกิจการขับขี่แบบครบวงจร
เกี่ยวกับความแข็งแกร่งตามธรรมชาติของโมเดลการมองเห็นและภาษาในการต่อต้านการโจมตีการรับรู้ภาพในการขับขี่อัตโนมัติ

เปดราม โมฮาเยร์อันซารี, อาเมียร์ ซาลาร์ปูร์, ไมเคิล คูห์ร, ซิยู หวง, โมฮัมหมัด ฮาหมัด, เซบาสเตียน สไตน์ฮอร์สต์, ฮาบีบ โอลูโฟบี, แมร์ต ดี. เปเซ่
ผู้จัดพิมพ์: มหาวิทยาลัย Clemson, มหาวิทยาลัยเทคนิคมิวนิก, มหาวิทยาลัยเท็กซัสที่อาร์ลิงตัน
วันที่เผยแพร่: 2025.06.13
ภารกิจ: การรับรู้
รหัส: V2LM
สรุป:
เอกสารนี้จะแนะนำ Vehicle Vision Language Models (V2LM) ซึ่งเป็น VLM ที่ได้รับการปรับแต่งโดยเฉพาะสำหรับงานการรับรู้ AV
ReCogDrive: กรอบความคิดที่เสริมความแข็งแกร่งสำหรับการขับขี่อัตโนมัติแบบครบวงจร

หยงคัง ลี, ไคซิน สยง, เซียงหยู่ กั๋ว, ฟาง ลี, ซิ่วซู่ หยาน, กังเว่ย ซู, ลี่จุน โจว, หลง เฉิน, ไห่หยาง ซุน, ปิง หวาง, กวง เฉิน, หางจุน เย่, เหวินหยู่ หลิว, ซิงกัง หวาง
ผู้จัดพิมพ์: มหาวิทยาลัยวิทยาศาสตร์และเทคโนโลยีหัวจง, Xiaomi EV
วันที่เผยแพร่: 2025.06.09
หน้าโครงการ: ReCogDrive
รหัส: ReCogDrive
ภารกิจ: การวางแผน
ชุดข้อมูล: NAVSIM
สรุป:
ReCogDrive กรอบการทำงานทางปัญญาเสริมแรงแบบใหม่สำหรับการขับขี่อัตโนมัติแบบ End-to-End พร้อมด้วย Vision-Language Model (VLM) และ Diffusion-based Planner ที่ได้รับการปรับปรุงด้วย Reinforcement Learning
ReCogDrive ใช้รูปแบบการฝึกอบรมสามขั้นตอน เริ่มตั้งแต่การฝึกอบรมก่อนการขับขี่ ตามด้วยการเรียนรู้เลียนแบบและการเรียนรู้เสริมแรง GRPO เพื่อเพิ่มความสามารถในการวางแผนของระบบวิสัยทัศน์-ภาษา-การกระทำ (VLA)
STSBench: เกณฑ์มาตรฐานสถานการณ์เชิงพื้นที่และเวลาสำหรับโมเดลภาษาขนาดใหญ่แบบหลายโหมดในการขับขี่อัตโนมัติ

คริสเตียน ฟรูห์เวิร์ธ-ไรซิงเกอร์, ดูซาน มาลิช, เว่ย ลิน, เดวิด ชินาเกิล, ซามูเอล ชูลเตอร์, ฮอร์สต์ พอสเซกเกอร์
ผู้จัดพิมพ์: มหาวิทยาลัยเทคโนโลยีกราซ, ห้องปฏิบัติการคริสเตียนดอปเปลอร์สำหรับการเรียนรู้ของเครื่องฝังตัว, มหาวิทยาลัยโยฮันเนสเคปเลอร์ ลินซ์, Amazon
วันที่เผยแพร่: 2025.06.06
งาน : QA
รหัส: STSBench
ชุดข้อมูล: STSBench
สรุป:
STSBench กรอบงานสำหรับการขุดข้อมูลสถานการณ์อัตโนมัติจากชุดข้อมูลการขับขี่อัตโนมัติขนาดใหญ่พร้อมคำอธิบายพื้นฐานที่สมบูรณ์
เมื่อนำไปใช้กับชุดข้อมูล NuScenes จะนำเสนอ STSnu ซึ่งเป็นเกณฑ์มาตรฐานแรกที่ประเมินความสามารถในการใช้เหตุผลเชิงพื้นที่และเวลาของ VLM โดยอิงจากการรับรู้ภาพสามมิติที่ครอบคลุม
การติดฉลากแบบมีโครงสร้างช่วยให้สามารถสร้างโมเดลภาษาภาพได้เร็วขึ้นสำหรับการขับขี่อัตโนมัติแบบครบวงจร

ห่าวเจียง, ชวนหู, หยูคังชิ, หยวนเหอ, เค่อหวาง, ซีจาง, จือเผิงจาง
ผู้จัดพิมพ์: มหาวิทยาลัยเซี่ยงไฮ้เจียวทง, KargoBot
วันที่เผยแพร่: 2025.06.05
งาน: VQA
ชุดข้อมูล: nuScenes
สรุป:
เอกสารนี้แนะนำชุดข้อมูลเกณฑ์มาตรฐานที่มีโครงสร้างและกระชับที่เรียกว่า NuScenes-S ซึ่งได้มาจากชุดข้อมูล NuScenes และประกอบด้วยการแสดงโครงสร้างที่เป็นมิตรกับเครื่อง
AD-EE: การออกจากระบบก่อนกำหนดเพื่อโมเดลภาษาภาพที่รวดเร็วและเชื่อถือได้ในการขับขี่อัตโนมัติ

เหลียนหมิง หวง, ไห่ป๋อ หู, หยูเฟย ชุย, เจียเฉิง ซูโอ, ซางหยู่ วู่, หนานกวน, ชุน เจสัน เสวี่ย
สำนักพิมพ์: มหาวิทยาลัยซิตี้แห่งฮ่องกง, มหาวิทยาลัยแมคกิลล์, MBZUAI, มหาวิทยาลัยซูโจว
วันที่เผยแพร่: 2025.06.04
งาน: การรับรู้, VQA
ชุดข้อมูล: Waymo , CODA ที่เน้นเฉพาะกรณีพิเศษ
สรุป:
AD-EE ซึ่งเป็นกรอบการทำงาน Early Exit ผสมผสานลักษณะเฉพาะของโดเมนการขับขี่อัตโนมัติและใช้ประโยชน์จากการอนุมานเชิงสาเหตุเพื่อระบุเลเยอร์ทางออกที่เหมาะสมที่สุด
AD-EE เสนอแนวทางตามการอนุมานเชิงสาเหตุเพื่อระบุและวิเคราะห์เลเยอร์ทางออกเบื้องต้นที่เหมาะสมที่สุดสำหรับการอนุมาน VLM ที่ได้รับการปรับปรุง
DriveRX: โมเดลการใช้เหตุผลด้านวิสัยทัศน์และภาษาสำหรับการขับขี่อัตโนมัติแบบข้ามงาน

มูซี เตียว, เล่อเล่ หยาง, หงป๋อ หยิน, เจ็กซู หวาง, เย่เจี๋ย หวาง, ต้าซิน เทียน, คงหมิง เหลียง, จ้านหยูหม่า
สำนักพิมพ์: มหาวิทยาลัยไปรษณีย์และโทรคมนาคมปักกิ่ง วิทยาลัยจงกวนชุน มหาวิทยาลัยเป่ยหาง
วันที่เผยแพร่: 27.05.2025
หน้าโครงการ: DriveRX
งาน: VQA
สรุป:
AutoDriveRL กรอบการฝึกอบรมแบบครบวงจรที่พัฒนาระบบขับขี่อัตโนมัติให้เป็นกระบวนการคิดเชิงเหตุผลที่มีโครงสร้างครอบคลุมงานหลักสี่งาน แต่ละงานมีการจำลองปัญหา QA เชิงภาษาภาพและวิสัยทัศน์อย่างอิสระ และได้รับการปรับแต่งโดยใช้แบบจำลองรางวัลเฉพาะงาน ช่วยให้สามารถส่งสัญญาณเสริมแรงที่ละเอียดในขั้นตอนการใช้เหตุผลที่แตกต่างกัน
ภายในกรอบงานนี้ ให้ฝึก DriveRX ซึ่งเป็น VLM ที่ใช้การใช้เหตุผลแบบข้ามงานที่ออกแบบมาสำหรับการตัดสินใจแบบเรียลไทม์
การใช้เหตุผลแบบ WOMD: ชุดข้อมูลขนาดใหญ่สำหรับการใช้เหตุผลแบบโต้ตอบในการขับขี่

ยี่เหิง ลี, คุนซิน ฟาน, ชงเจียน เกอ, จี้หาว จ้าว, เฉินหราน ลี, เฉินเฟิง ซู, ฮวาซิ่ว เหยา, มาซาโยชิ โทมิซึกะ, โบเล่ โจว, เฉิน ถัง, หมิงหยู่ติง, เว่ย จ้านICML 2025
ผู้จัดพิมพ์: UC Berkeley, UCLA, UNC-Chapel Hill, UT Austin
วันที่เผยแพร่: 25.05.2568
รหัส: WOMD-การใช้เหตุผล
ชุดข้อมูล: ชุดข้อมูล Waymo Open Motion
งาน: VQA
สรุป:
WOMD-Reasoning คือชุดข้อมูลคำอธิบายภาษาที่สร้างขึ้นจากชุดข้อมูล Waymo Open Motion (WOMD) โดยเน้นที่การอธิบายและการใช้เหตุผลในการโต้ตอบและความตั้งใจในสถานการณ์การขับขี่
FutureSightDrive: การคิดเชิงภาพด้วย CoT เชิงพื้นที่และเวลาสำหรับการขับขี่อัตโนมัติ

ชวงเซง, ซินหยวน ชาง, เมิ่งเหว่ย เซี่ย, ซินหราน หลิว, ยี่ฟาน ไป่, เจิ้งปัน, มู่ ซู, ซิง เว่ย
สำนักพิมพ์: อาลีบาบากรุ๊ป, มหาวิทยาลัยซีอานเจียวทง
วันที่เผยแพร่: 2025.05.23
ภารกิจ: การสร้าง, การวางแผน
รหัส: FSDrive
ชุดข้อมูล: nuScenes
สรุป:
วิธีการให้เหตุผล CoT เชิงเวลาและพื้นที่ที่ช่วยให้แบบจำลองสามารถปรับปรุงการวางแผนวิถีได้โดยการคิดแบบภาพจากมิติเวลาและพื้นที่ในอนาคต
รูปแบบการฝึกอบรมล่วงหน้าแบบรวมสำหรับการสร้างภาพและความเข้าใจ
การนำทางเชิงความหมายที่คล้ายมนุษย์สำหรับการขับขี่อัตโนมัติโดยใช้การแสดงความรู้และโมเดลภาษาขนาดใหญ่

ออกัสโต หลุยส์ บัลลาร์ดินี, มิเกล แองเจล โซเตโล
สำนักพิมพ์: มหาวิทยาลัยอัลคาล
วันที่เผยแพร่: 2025.05.22
งาน : QA
สรุป:
เอกสารนี้สำรวจการใช้ Large Language Models เพื่อสร้างกฎการเขียนโปรแกรมชุดคำตอบโดยแปลคำสั่งการนำทางที่ไม่เป็นทางการให้เป็นการใช้เหตุผลตามตรรกะที่มีโครงสร้าง
VL-SAFE: การเรียนรู้เสริมความปลอดภัยที่คำนึงถึงการมองเห็นและภาษานำทางด้วยโมเดลโลกสำหรับการขับขี่อัตโนมัติ

หยานซ่ง คู, ซีหลิน ฮวง, ซีเฮา เซิง, เจี้ยนฉง เฉิน, ซือไค เฉิน, ซามูเอล ลาบี
สำนักพิมพ์: มหาวิทยาลัยเพอร์ดู, มหาวิทยาลัยวิสคอนซิน-แมดิสัน,
วันที่เผยแพร่: 2025.05.22
หน้าโครงการ: VL-SAFE
รหัส : VL-SAFE
งาน: กรอบงาน
สรุป:
VL-SAFE กรอบการทำงาน RL ที่ปลอดภัยตามแบบจำลองโลกที่มีแบบจำลองภาษาวิสัยทัศน์ (VLM) เป็นแนวทางด้านความปลอดภัย ออกแบบมาเพื่อการเรียนรู้นโยบายความปลอดภัยแบบออฟไลน์
DriveMoE: การผสมผสานของผู้เชี่ยวชาญสำหรับโมเดลวิสัยทัศน์-ภาษา-การกระทำในการขับขี่อัตโนมัติแบบครบวงจร

เจิ้นเจี๋ย หยาง, อี้หลิน ไช่, เสี่ยวซง เจีย, ฉีเฟิง ลี, หยูเฉียน เชา, ซู่ไค จู, ไห่เซิง ซู, จุนชี่ หยาน
สำนักพิมพ์: มหาวิทยาลัยเซี่ยงไฮ้เจียวถง
วันที่เผยแพร่: 2025.05.22
หน้าโครงการ: DriveMoE
รหัส: DriveMoE
ชุดข้อมูล: Bench2Drive
ภารกิจ: การวางแผน
สรุป:
DriveMoE กรอบงาน E2E-AD แบบใหม่ที่ใช้ MoE เป็นพื้นฐาน พร้อมด้วย MoE ด้านวิสัยทัศน์ที่เน้นฉาก และ MoE ด้านการกระทำที่เน้นทักษะ
DriveMoE ถูกสร้างขึ้นบนพื้นฐาน Vision-Language-Action (VLA) ของเรา (เดิมมาจากฟิลด์ AI ที่เป็นรูปธรรม) ที่เรียกว่า Drive-π0
AgentThink: กรอบการทำงานแบบรวมสำหรับการใช้เหตุผลแบบห่วงโซ่แห่งความคิดที่เสริมด้วยเครื่องมือในแบบจำลองภาษาวิสัยทัศน์สำหรับการขับขี่อัตโนมัติ

Kangan Qian, Sicong Jiang, Yang Zhong, Ziang Luo, Zilin Huang, Tianze Zhu, Kun Jiang, Mengmeng Yang, Zheng Fu, Jinyu Miao, Yining Shi, He Zhe Lim, Li Liu, Tianbao Zhou, Huang Yu, Yifei Hu, Guang Li, Guang Chen, Hao Ye, ลี่จุนซุน, Diange Yang
ผู้จัดพิมพ์: มหาวิทยาลัยชิงหัว, มหาวิทยาลัยแมคกิลล์, บริษัท Xiaomi, มหาวิทยาลัยวิสคอนซิน – เมดิสัน
วันที่เผยแพร่: 2025.06.12
งาน: VQA
สรุป:
AgentThink กรอบงานแรกที่จะบูรณาการการเรียกใช้เครื่องมือแบบไดนามิกในรูปแบบตัวแทนเข้ากับการใช้เหตุผลแบบภาษาวิสัยทัศน์สำหรับงานการขับขี่อัตโนมัติ
ท่อส่งการฝึกอบรมสองขั้นตอนที่รวม SFT เข้ากับ GRPO
การขยายโมเดลภาษาวิสัยทัศน์ขนาดใหญ่สำหรับงานโต้ตอบที่หลากหลายในการขับขี่อัตโนมัติ

Zongchuang Zhao, Haoyu Fu, Dingkang Liang, Xin Zhou, Dingyuan Zhang, Hongwei Xie, Bing Wang, Xiang Bai
Publisher: Huazhong University of Science and Technology, Xiaomi EV
Publish Date: 2025.05.13
Task: VQA
Code: DriveMonkey
Summary:
NuInteract, a large-scale dataset for advancing LVLMs in autonomous driving. With 239K images,34K frames, and over 1.5M image-language pairs across 850 scenes, NuInteract provides dense captions detailing the surrounding environment and 2D/3D annotations for tasks like 2D/3D visual grounding, enabling comprehensive perception, prediction, and planning.
DriveMonkey, a flexible framework supporting multiple interactive tasks via user prompts.
Towards Human-Centric Autonomous Driving: A Fast-Slow Architecture Integrating Large Language Model Guidance with Reinforcement Learning

Chengkai Xu, Jiaqi Liu, Yicheng Guo, Yuhang Zhang, Peng Hang, Jian Sun
Publisher: Tongji University
Publish Date: 2025.05.11
Task: Planning
Env: Highway-Env
Summary:
A “fast-slow” decision-making framework that integrates a Large Language Model (LLM) for high-level instruction parsing with a Reinforcement Learning (RL) agent for low-level real-time decision.
Natural Reflection Backdoor Attack on Vision Language Model for Autonomous Driving

Ming Liu, Siyuan Liang, Koushik Howlader, Liwen Wang, Dacheng Tao, Wensheng Zhang
Publisher: Iowa State University, National University of Singapore
Publish Date: 2025.05.09
Task: VQA
Datasets: DriveLM
Summary:
It proposes a natural reflection-based backdoor attack targeting VLM systems in autonomous driving scenarios, aiming to induce substantial response delays when specific visual triggers are present.
DSDrive: Distilling Large Language Model for Lightweight End-to-End Autonomous Driving with Unified Reasoning and Planning

Wenru Liu, Pei Liu, Jun Ma
Publisher: The Hong Kong University of Science and Technology
Publish Date: 2025.05.08
Task: Planning
Video: DSDrive
Summary:
DSDrive, a lightweight E2E AD framework that employs a compact LLM to process multi-modal inputs for explicit reasoning and closed-loop planning. Specifically, we utilize knowledge distillation to empower the compact LLM to undertake the reasoning and planning tasks, thereby improving its overall performance.
A novel waypoint-driven dual-head coordination module that bridges high-level reasoning and lowlevel trajectory planning.
X-Driver: Explainable Autonomous Driving with Vision-Language Models

Wei Liu, Jiyuan Zhang, Binxiong Zheng, Yufeng Hu, Yingzhan Lin, Zengfeng Zeng
Publisher: Harbin Institute of Technology, Baidu Inc
Publish Date: 2025.05.08
Task: VQA, Planning
Dataset: Bench2Drive
Summary:
X-Driver, a unified multi-modal large language models(MLLMs) framework designed for closed-loop autonomous driving, leveraging Chain-of-Thought(CoT) and autoregressive modeling to enhance perception and decisionmaking.
Seeking to Collide: Online Safety-Critical Scenario Generation for Autonomous Driving with Retrieval Augmented Large Language Models

Yuewen Mei, Tong Nie, Jian Sun, Ye Tian
Publisher: Tongji University, The Hong Kong Polytechnic University,
Publish Date: 2025.05.02
Task: Generation
Dataset: Waymo
Summary:
An LLM-based agent framework is proposed to generate interactive and safety-critical scenarios online.
A memorization and retrieval mechanism is developed to continuously adapt LLMs to changing scenarios.
V3LMA: Visual 3D-enhanced Language Model for Autonomous Driving

Jannik Lübberstedt, Esteban Rivera, Nico Uhlemann, Markus Lienkamp
Publisher: Technical University of Munich, Munich Institute of Robotics and Machine Intelligenc
Publish Date: 2025.04.30
Task: VQA
Datasets: LingoQA
Summary:
Proposal and evaluation of V3LMA, a novel method that combines the strengths of LLMs and LVLMs to enhance 3D scene understanding in traffic scenarios—without requiring model training or fine-tuning.
Enhancing Autonomous Driving Systems with On-Board Deployed Large Language Models

Nicolas Baumann, Cheng Hu, Paviththiren Sivasothilingam, Haotong Qin, Lei Xie, Michele Magno, Luca Benini RSS 2025
Publisher: ETH Zurich, Zhejiang University
Publish Date: 2025.04.15
Task: Planning
Summary:
A hybrid architecture combining low level Model Predictive Controller (MPC) with locally deployed Large Language Models (LLMs) to enhance decision-making and Human Machine Interaction (HMI).
NuScenes-SpatialQA: A Spatial Understanding and Reasoning Benchmark for Vision-Language Models in Autonomous Driving

Kexin Tian, Jingrui Mao, Yunlong Zhang, Jiwan Jiang, Yang Zhou, Zhengzhong Tu
Publisher: Texas A&M University, University of Wisconsin-Madison
Publish Date: 2025.04.07
Project Page: NuScenes-SpatialQA
Task: VQA
Summary:
NuScenes-SpatialQA, the first large-scale ground-truth-based Question-Answer (QA) benchmark specifically designed to evaluate the spatial understanding and reasoning capabilities of VLMs in autonomous driving.
OpenDriveVLA: Towards End-to-end Autonomous Driving with Large Vision Language Action Model

Xingcheng Zhou, Xuyuan Han, Feng Yang, Yunpu Ma, Alois C. Knoll
Publisher: Technical University of Munich, Ludwig Maximilian University of Munich
Publish Date: 2025.03.30
Project Page: OpenDriveVLA
Code: OpenDriveVLA
Task: VQA, Planning
Summary:
OpenDriveVLA, a Vision-Language Action (VLA) model designed for end-to-end autonomous driving.
VLM-C4L: Continual Core Dataset Learning with Corner Case Optimization via Vision-Language Models for Autonomous Driving

Haibo Hu, Jiacheng Zuo, Yang Lou, Yufei Cui, Jianping Wang, Nan Guan, Jin Wang, Yung-Hui Li, Chun Jason Xue COLM 2025
Publisher: City University of Hong Kong, Soochow University, McGill University, Hon Hai Research Institute, Mohamed bin Zayed University of Artificial Intelligence
Publish Date: 2025.03.29
Project Pages: VLM-C4L
Task: Perception
Summary:
VLM-C4L, a continual learning framework that introduce Vision-Language Models (VLMs) to dynamically optimize and enhance corner case datasets, and VLM-C4L combines VLM-guided high-quality data extraction with a core data replay strategy, enabling the model to incrementally learn from diverse corner cases while preserving performance on previously routine scenarios, thus ensuring long-term stability and adaptability in real-world autonomous driving.
Fine-Grained Evaluation of Large Vision-Language Models in Autonomous Driving

Yue Li, Meng Tian, Zhenyu Lin, Jiangtong Zhu, Dechang Zhu, Haiqiang Liu, Zining Wang, Yueyi Zhang, Zhiwei Xiong, Xinhai Zhao
Publisher: University of Science and Technology of China, Huawei Noah’s Ark Lab, University of California, Berkeley
Publish Date: 2025.03.27
Code: VLADBench
Task: VQA
Summary:
VLADBench, specifically designed to rigorously evaluate the capabilities of VLMs in AD. VLADBench employes a hierarchical structure that reflects the complex skill set required for reliable driving, progressing from fundamental scene and traffic elements comprehension to advanced reasoning and decision-making.
ORION: A Holistic End-to-End Autonomous Driving Framework by Vision-Language Instructed Action Generation

Haoyu Fu, Diankun Zhang, Zongchuang Zhao, Jianfeng Cui, Dingkang Liang, Chong Zhang, Dingyuan Zhang, Hongwei Xie, Bing Wang, Xiang Bai
Publisher: Huazhong University of Science and Technology, Xiaomi EV
Publish Data: 2025.03.25
Task: Planning
Project Page: ORION
Code: ORION
Dataset: Bench2Drive
Summary:
ORION, a hOlistic E2E autonomous dRiving framework by vIsion-language instructed actiON generation. ORION uniquely combines a QT-Former to aggregate long-term history context, a Large Language Model (LLM) for driving scenario reasoning, and a generative planner for precision trajectory prediction.
AED: Automatic Discovery of Effective and Diverse Vulnerabilities for Autonomous Driving Policy with Large Language Models

Le Qiu, Zelai Xu, Qixin Tan, Wenhao Tang, Chao Yu, Yu Wang
Publisher: Tsinghua University, Beijing Zhongguancun Academy
Publish Date: 2025.03.24
Task: Planning
Env: Highway-Env
Summary:
AED, a framework that uses large language models (LLMs) to Automatically discover Effective and Diverse vulnerabilities in autonomous driving policies.
AED first utilize an LLM to automatically design reward functions for RL training.
AutoDrive-QA- Automated Generation of Multiple-Choice Questions for Autonomous Driving Datasets Using Large Vision-Language Models

Boshra Khalili, Andrew W.Smyth
Publisher: Columbia University
Publish Date: 2025.03.20
Task: VQA
Summary:
AutoDrive-QA, Automatic pipeline that converts existing driving QA datasets (including DriveLM, NuScenes-QA, and LingoQA) into a structured multiple-choice question (MCQ) format.
RAD: Retrieval-Augmented Decision-Making of Meta-Actions with Vision-Language Models in Autonomous Driving

Yujin Wang, Quanfeng Liu, Zhengxin Jiang, Tianyi Wang, Junfeng Jiao, Hongqing Chu, Bingzhao Gao, Hong Chen
Publisher: Tongji University, Yale University, University of Texas at Austin
Publish Date: 2025.03.18
Task: VQA
Summary:
Propose a retrieval-augmented decision-making (RAD) framework, a novel architecture designed to enhance VLMs’ capabilities to reliably generate meta-actions in autonomous driving scenes.
A Framework for a Capability-driven Evaluation of Scenario Understanding for Multimodal Large Language Models in Autonomous Driving

Tin Stribor Sohn, Philipp Reis, Maximilian Dillitzer, Johannes Bach, Jason J. Corso, Eric Sax
Publisher: Dr. Ing. h.c. F. Porsche AG, Forschungszentrum Informatik，Hochschule Esslingen, University of Michigan, Karlsruher Institut f ̈ur Technologie
Publish Date: 2025.03.14
Task: Evaluation
Summary:
This paper proposes a holistic framework for a capability-driven evaluation of MLLMs in autonomous driving. The framework structures scenario understanding along the four core capability dimensions semantic, spatial, temporal, and physical.
DynRsl-VLM: Enhancing Autonomous Driving Perception with Dynamic Resolution Vision-Language Models

Xirui Zhou, Lianlei Shan, Xiaolin Gui
Publisher: Xi’an Jiaotong University, University of Chinese Academy of Sciences
Publish Date: 2025.03.14
Task: VQA
Summary:
DynRsl-VLM incorporates a dynamic resolution image input processing approach that captures all entity feature information within an image while ensuring that the image input remains computationally tractable for the Vision Transformer (ViT).
SimLingo: Vision-Only Closed-Loop Autonomous Driving with Language-Action Alignment

Katrin Renz, Long Chen, Elahe Arani, Oleg Sinavski CVPR 2025
Publisher: Wayve, University of T ̈ubingen, T ̈ubingen AI Center
Publish Date: 2025.03.12
Task: Planning
Datasets: Carla Leadboard V2, Bench2Drive
Summary:
A VLM-based driving model that achieves state-of-the-art driving performance on the official CARLA Leaderboard 2.0 and the local benchmark Bench2Drive in the CARLA simulator. (2) A new task (Action Dreaming), which comes with a methodology to collect instruction-action pairs and a benchmark to evaluate the connection of language and action understanding without having to execute unsafe actions. (3) A generalist model that achieves not only good driving performance but also includes several language related tasks in the same model.
CoT-Drive: Efficient Motion Forecasting for Autonomous Driving with LLMs and Chain-of-Thought Prompting

Haicheng Liao, Hanlin Kong, Bonan Wang, Chengyue Wang, Wang Ye, Zhengbing He, Chengzhong Xu, Zhenning Li IEEE TAI 2025
Publisher: University of Macau, Massachusetts Institute of Technology
Publish Date: 2025.03.10
Task: VQA
Summary:
Introduce a teacher-student knowledge distillation strategy to effectively transfer LLMs’ advanced scene understanding capabilities to lightweight language models (LMs), ensuring that CoT-Drive operates in real-time on edge devices while maintaining comprehensive scene understanding and generalization capabilities.
Evaluation of Safety Cognition Capability in Vision-Language Models for Autonomous Driving

Enming Zhang, Peizhe Gong, Xingyuan Dai, Yisheng Lv, Qinghai Miao
Publisher: University of Chinese Academy of Sciences,
Publish Date: 2025.03.09
Code: SCD-Bench
Task: Evaluation
Summary:
Propose a novel evaluation method: Safety Cognitive Driving Benchmark (SCD-Bench) and debelop the Autonomous Driving Image-Text Annotation System (ADA).
VLM-E2E: Enhancing End-to-End Autonomous Driving with Multimodal Driver Attention Fusion

Pei Liu, Haipeng Liu, Haichao Liu, Xin Liu, Jinxin Ni, Jun Ma
Publisher: The Hong Kong University of Science and Technology (Guangzhou), Li Auto Inc., Xiamen University, The Hong Kong University of Science and Technology
Publish Date: 2025.02.25
Task: Planning
Datasets: nuScenes
Summary:
VLME2E, a novel framework that uses the VLMs to enhance training by providing attentional cues.
Integrates textual representations into Bird’s-Eye-View (BEV) features for semantic supervision, which enables the model to learn richer feature representations that explicitly capture the driver’s attentional semantics.
CurricuVLM: Towards Safe Autonomous Driving via Personalized Safety-Critical Curriculum Learning with Vision-Language Models

Zihao Sheng, Zilin Huang, Yansong Qu, Yue Leng, Sruthi Bhavanam, Sikai Chen
Publisher: University of Wisconsin-Madison, Purdue University
Publish Date: 2025.02.21
Task: Planning
Project Page: CurricuVLM
Datasets: MetaDrive, Waymo
Summary:
CurricuVLM, a novel framework that leverages Vision-Language Models (VLMs) to enable personalized curriculum learning for autonomous driving agents.
CurricuVLM is the first work to utilize VLMs for dynamic curriculum generation in closed-loop autonomous driving training.
V2V-LLM: Vehicle-to-Vehicle Cooperative Autonomous Driving with Multi-Modal Large Language Models

Hsu-kuang Chiu, Ryo Hachiuma, Chien-Yi Wang, Stephen F. Smith, Yu-Chiang Frank Wang, Min-Hung Chen
Publisher: NVIDIA, Carnegie Mellon University
Publish Date: 2025.02.14
Task: VQA
Summary:
Create and introduce the V2V-QA dataset to support the development and evaluation of LLM-based approaches to end-to-end cooperative autonomous driving.
Propose a baseline method V2V-LLM for cooperative autonomous driving to provide an initial benchmark for V2V-QA.
Occ-LLM: Enhancing Autonomous Driving with Occupancy-Based Large Language Models

Tianshuo Xu, Hao Lu, Xu Yan, Yingjie Cai, Bingbing Liu, Yingcong Chen ICRA 2025
Publisher: Hong Kong University of Science and Technology (Guangzhou), Huawei Noah’s Ark Lab
Publish Date: 2025.02.10
Task: Perception, Planning
Dataset: nuScenes
Summary:
Introduce an occupancy-based large language model (Occ-LLM) for autonomous driving, demonstrating superior scene comprehension.
INSIGHT: Enhancing Autonomous Driving Safety through Vision-Language Models on Context-Aware Hazard Detection and Edge Case Evaluation

Dianwei Chen, Zifan Zhang, Yuchen Liu, Xianfeng Terry Yang
Publisher: University of Maryland, North Carolina State University
Publish Date: 2025.02.01
Task: VQA
Summary:
INSIGHT (Integration of Semantic and Visual Inputs for Generalized Hazard Tracking), a hierarchical vision-language model (VLM) framework designed to enhance hazard detection and edge-case evaluation.
LLM-attacker: Enhancing Closed-loop Adversarial Scenario Generation for Autonomous Driving with Large Language Models

Yuewen Mei, Tong Nie, Jian Sun, Ye Tian IEEE TITS 2025
Publisher: Tongji University, The Hong Kong Polytechnic University
Publish Date: 2025.01.27
Viddeo: LLM-attacker
Task: Generation
Dataset: MetaDrive, Waymo
Summary:
LLM-attacker: a closedloop adversarial scenario generation framework leveraging large language models (LLMs).
Black-Box Adversarial Attack on Vision Language Models for Autonomous Driving

Lu Wang, Tianyuan Zhang, Yang Qu, Siyuan Liang, Yuwei Chen, Aishan Liu, Xianglong Liu, Dacheng Tao
Publisher: Beihang University, National University of Singapore, Aviation Industry Development Research Center of China, Nanyang Technological University
Publish Date: 2025.01.23
Task: VQA
Summary:
Cascading Adversarial Disruption (CAD) first introduces Decision Chain Disruption, which targets low-level reasoning breakdown by generating and injecting deceptive semantics, ensuring the perturbations remain effective across the entire decision-making chain.
Distilling Multi-modal Large Language Models for Autonomous Driving

Deepti Hegde, Rajeev Yasarla, Hong Cai, Shizhong Han, Apratim Bhattacharyya, Shweta Mahajan, Litian Liu, Risheek Garrepalli, Vishal M. Patel, Fatih Porikli
Publisher: Johns Hopkins University, Qualcomm AI Research
Publish Date: 2025.01.16
Task: Planning
Summary:
DiMA, an end-to-end autonomous driving framework that distills knowledge from an MLLM to a vision-based planner to ensure robustness to long-tail events while maintaining efficiency.
Propose a distillation task along with the following surrogate tasks to align the objectives of the vision-based planner and the MLLM: (i) masked token reconstruction (ii) future token prediction (iii) scene editing.
Modeling Language for Scenario Development of Autonomous Driving Systems

Toshiaki Aoki, Takashi Tomita, Tatsuji Kawai, Daisuke Kawakami, Nobuo Chida
Publisher: JAIST, Kochi University, Mitsubishi Electric Corporation
Publish Date: 2025.01.16
Task: Development
Summary:
This study introduces a notation called the car position diagram (CPD). The CPD allows for the concise representation of numerous scenarios and is particularly suitable for scenario analysis and design.
Application of Vision-Language Model to Pedestrians Behavior and Scene Understanding in Autonomous Driving

Haoxiang Gao, Yu Zhao
Publisher: Motional AD LLC, University of Toronto
Publish Date: 2025.01.12
Task: VQA
Summary:
Analyze effective knowledge distillation of LLM semantic labels to smaller Vision networks, which can be used for the semantic representation of complex scenes for downstream decision-making for planning and control.
DriVLM: Domain Adaptation of Vision-Language Models in Autonomous Driving

Xuran Zheng, Chang D. Yoo
Publisher: KAIST
Publish Date: 2025.01.09
Task: VQA
Summary:
Explore the utility of small-scale MLLMs and applied small-scale MLLMs to the field of autonomous driving.
Vision-Language Models for Autonomous Driving: CLIP-Based Dynamic Scene Understanding

Mohammed Elhenawy, Huthaifa I. Ashqar, Andry Rakotonirainy, Taqwa I. Alhadidi, Ahmed Jaber, Mohammad Abu Tami
Publisher: Queensland University of Technology, Arab American University, Columbia University
Publish Date: 2025.01.09
Task: Scene Understanding
Summary:
This study developed a dynamic scene retrieval system using Contrastive Language–Image Pretraining (CLIP) models, which can be optimized for real-time deployment on edge devices.
Are VLMs Ready for Autonomous Driving? An Empirical Study from the Reliability, Data, and Metric Perspectives

Shaoyuan Xie, Lingdong Kong, Yuhao Dong, Chonghao Sima, Wenwei Zhang, Qi Alfred Chen, Ziwei Liu, Liang Pan ICCV 2025
Project Page: DriveBench
Code: DriveBench
HuggingFace: DriveBench
Publish Date: 2025.01.07
Task: Benchmark
Summary:
DriveBench, a benchmark dataset designed to evaluate VLM reliability across 17 settings (clean, corrupted, and text-only inputs), encompassing 19, 200 frames, 20, 498 question-answer pairs, three question types, four mainstream driving tasks, and a total of 12 popular VLMs.
Generating Traffic Scenarios via In-Context Learning to Learn Better Motion Planner

Aizierjiang Aiersilan AAAI 2025 Oral
Publisher: University of Macau
Publish Date: 2024.12.24
Task: Generation
Env : CARLA
Project Pages: AutoSceneGen
Code: AutoSceneGen
Summary:
A universal, general, and cost-effective framework, “AutoSceneGen”, is proposed to automatically enhance the heterogeneity of traffic scenarios through scenario descriptions, thereby accelerating the simulation and testing process.
Large Language Model guided Deep Reinforcement Learning for Decision Making in Autonomous Driving

Hao Pang, Zhenpo Wang, Guoqiang Li
Publisher: Beijing Institute of Technology
Publish Date: 2024.12.24
Task: Planning
Code: LGDRL
Env: HighwayEnv
Summary:
Propose a novel large language model (LLM) guided deep reinforcement learning (LGDRL) framework for addressing the decision-making problem of autonomous vehicles. Within this framework, an LLM-based driving expert is integrated into the DRL to provide intelligent guidance for the learning process of DRL.
Application of Multimodal Large Language Models in Autonomous Driving

Md Robiul Islam
Publisher: William & Mary
Publish Date: 2025.12.21
Task: VQA
Summary:
Conduct a Virtual Question Answering (VQA) dataset to fine-tune the model and address problems with the poor performance of MLLM on AD.
VLM-RL: A Unified Vision Language Models and Reinforcement Learning Framework for Safe Autonomous Driving

Zilin Huang, Zihao Sheng, Yansong Qu, Junwei You, Sikai Chen
Publisher: University of Wisconsin-Madison, Purdue University,
Publish Date: 2024.12.20
Task: Reward Design
Project Page: VLM-RL
Summary:
VLM-RL, a unified framework that integrates pre-trained Vision-Language Models (VLMs) with RL to generate reward signals using image observation and natural language goals.
AutoTrust: Benchmarking Trustworthiness in Large Vision Language Models for Autonomous Driving

Shuo Xing, Hongyuan Hua, Xiangbo Gao, Shenzhe Zhu, Renjie Li, Kexin Tian, Xiaopeng Li, Heng Huang, Tianbao Yang, Zhangyang Wang, Yang Zhou, Huaxiu Yao, Zhengzhong Tu
Publisher: Texas A&M University, University of Toronto, University of Michigan, University of Wisconsin-Madison, University of Maryland, University of Texas at Austin, University of North Carolina at Chapel Hill
Publish Date: 2024.12.19
Task: VQA
Code: AutoTrust
Leaderboard: AutoTrust
Summary:
AutoTrust is a groundbreaking benchmark designed to assess the trustworthiness of DriveVLMs. This work aims to enhance public safety by ensuring DriveVLMs operate reliably across critical dimensions.
VLM-AD: End-to-End Autonomous Driving through Vision-Language Model Supervision

Yi Xu, Yuxin Hu, Zaiwei Zhang, Gregory P. Meyer, Siva Karthik Mustikovela, Siddhartha Srinivasa, Eric M. Wolff, Xin Huang
Publisher: Cruise LLC, Northeastern University
Publish Date: 2024.12.19
Task: Planning
Dataset: nuScenes
Summary:
VLM-AD, a method that leverages vision-language models (VLMs) as teachers to enhance training by providing additional supervision that incorporates unstructured reasoning information and structured action labels.
RAC3: Retrieval-Augmented Corner Case Comprehension for Autonomous Driving with Vision-Language Models

Yujin Wang, Quanfeng Liu, Jiaqi Fan, Jinlong Hong, Hongqing Chu, Mengjian Tian, Bingzhao Gao, Hong Chen
Publisher: Tongji University, Shenzhen Technology University
Publish Date: 2024.12.15
Task: VQA
Datasets: CODA-LM
Summary:
RAC3, a novel framework designed to enhance the performance of VLMs in corner case comprehension.
RAC3 integrates a frequencyspatial fusion (FSF) image encoder, a cross-modal alignment training method for embedding models with hard and semihard negative mining, and a fast querying and retrieval pipeline based on K-Means clustering and hierarchical navigable small world (HNSW) indexing.
WiseAD: Knowledge Augmented End-to-End Autonomous Driving with Vision-Language Model

Songyan Zhang, Wenhui Huang, Zihui Gao, Hao Chen, Chen Lv
Publisher: Nanyang Technology University, Zhejiang University
Publish Date: 2024.12.13
Task: Planning
Summary:
Investigate the effects of the depth and breadth of fundamental driving knowledge on closed-loop trajectory planning and introduce WiseAD, a specialized VLM tailored for end-to-end autonomous driving capable of driving reasoning, action justification, object recognition, risk analysis, driving suggestions, and trajectory planning across diverse scenarios.
PKRD-CoT: A Unified Chain-of-thought Prompting for Multi-Modal Large Language Models in Autonomous Driving

Xuewen Luo, Fan Ding, Yinsheng Song, Xiaofeng Zhang, Junnyong Loo ICONIP 2024
Publisher: Monash University Malaysia
Task: QA, Prompt Engineer
Publish Date: 2024.12.02
Summary:
PKRD-CoT is constructed based on the four fundamental capabilities of autonomous driving—perception, knowledge, reasoning, and decision-making.
Visual Adversarial Attack on Vision-Language Models for Autonomous Driving

Tianyuan Zhang, Lu Wang, Xinwei Zhang, Yitong Zhang, Boyi Jia, Siyuan Liang, Shengshan Hu, Qiang Fu, Aishan Liu, Xianglong Liu
Publisher: Beihang University, National University of Singapore, Huazhong University of Science and Technology
Task: VQA
Publish Date: 2024.11.27
Summary:
ADvLM, the first visual adversarial attack framework specifically designed for VLMs in AD.
Semantic-Invariant Induction in the textual domain and Scenario-Associated Enhancement in the visual domain, ensuring attack effectiveness across varied instructions and sequential viewpoints.
Explanation for Trajectory Planning using Multi-modal Large Language Model for Autonomous Driving

Shota Yamazaki, Chenyu Zhang, Takuya Nanri, Akio Shigekane, Siyuan Wang, Jo Nishiyama, Tao Chu, Kohei Yokosawa ECCV 2024 VCAD Workshop
Publisher: Nissan Motor Co., Ltd,
Publish Date: 2024.11.15
Task: VQA
Summary:
Propose a reasoning model that takes future planning trajectories of the ego vehicle as input to generate reasoning text.
Integrating Object Detection Modality into Visual Language Model for Enhanced Autonomous Driving Agent

Linfeng He, Yiming Sun, Sihao Wu, Jiaxu Liu, Xiaowei Huang NeurIPS 2024 SafeGenAI Workshop
Publisher: University of Liverpool, University of Nottingham
Publish Date: 2024.11.08
Task: Precption
Dataset: DriveLM
Summary:
Extend the Llama-Adapter architecture by incorporating a YOLOS-based detection network alongside the CLIP perception network, addressing limitations in object detection and localisation.
Senna: Bridging Large Vision-Language Models and End-to-End Autonomous Driving

Bo Jiang, Shaoyu Chen, Bencheng Liao, Xingyu Zhang, Wei Yin, Qian Zhang, Chang Huang, Wenyu Liu, Xinggang Wang
Publisher: Huazhong University of Science and Technology
Publish Date: 2024.10.29
Task: VQA, Planning
Code: Senna
Dataset: nuScenes, DriveX
Summary:
Senna, an autonomous driving system that integrates an LVLM with an end-to-end model, achieving structured planning from high-level decisions to low-level trajectory prediction.
Words to Wheels: Vision-Based Autonomous Driving Understanding Human Language Instructions Using Foundation Models

Chanhoe Ryu, Hyunki Seong, Daegyu Lee, Seongwoo Moon, Sungjae Min, D.Hyunchul Shim
Publisher: KAIST, ETRI
Publish Date: 2024.10.14
Task: VQA
Summary:
Introduce an innovative application of foundation models, enabling Unmanned Ground Vehicles (UGVs) equipped with an RGB-D camera to navigate to designated destinations based on human language instructions.
LeGEND: A Top-Down Approach to Scenario Generation of Autonomous Driving Systems Assisted by Large Language Models

Shuncheng Tang, Zhenya Zhang, Jixiang Zhou, Lei Lei, Yuan Zhou, Yinxing Xue ASE 2024
Publisher: University of Science and Technology of China, Kyushu University, Zhejiang Sci-Tech University
Task: Generation
Publish Date: 2024.09.16
Code: LeGEND
Summary:
LeGEND, a top-down scenario generation approach that can achieve both criticality and diversity of scenarios.
Devise a two-stage transformation, by using an intermediate language, from accident reports to logical scenarios; so, LeGEND involves two LLMs, each in charge of one different stage.
Implement LeGEND and demonstrate its effectiveness on Apollo, and we detect 11 types of critical concrete scenarios that reflect different aspects of system defects.
MiniDrive: More Efficient Vision-Language Models with Multi-Level 2D Features as Text Tokens for Autonomous Driving

Enming Zhang, Xingyuan Dai, Yisheng Lv, Qinghai Miao
Publisher: University of Chinese Academy of Sciences, CASIA
Task: QA
Publish Date: 2024.09.14
Code: MiniDrive
Summary:
MiniDrive addresses the challenges of efficient deployment and real-time response in VLMs for autonomous driving systems. It can be fully trained simultaneously on an RTX 4090 GPU with 24GB of memory.
Feature Engineering Mixture of Experts (FE-MoE) addresses the challenge of efficiently encoding 2D features from multiple perspectives into text token embeddings, effectively reducing the number of visual feature tokens and minimizing feature redundancy.
Dynamic Instruction Adapter through a residual structure, which addresses the problem of fixed visual tokens for the same image before being input into the language model.
Hint-AD: Holistically Aligned Interpretability in End-to-End Autonomous Driving

Kairui Ding, Boyuan Chen, Yuchen Su, Huan-ang Gao, Bu Jin, Chonghao Sima, Wuqiang Zhang, Xiaohui Li, Paul Barsch, Hongyang Li, Hao Zhao CoRL 2024
Publisher: Institute for AI Industry Researc, Mercedes-Benz Group China Ltd, Tsinghua University, Shanghai AI Lab
Publish Date: 2024.09.10
Project Page: Hint-AD
Task: VQA
Summary:
Hint-AD, an integrated AD-language system that generates language aligned with the holistic perception-prediction-planning outputs of the AD model. By incorporating the intermediate outputs and a holistic token mixer sub-network for effective feature adaptation, Hint-AD achieves desirable accuracy, achieving state-of-the-art results in driving language tasks including driving explanation, 3D dense captioning, and command prediction.
Contribute a human-labeled driving explanation dataset, Nu-X on nuScenesto address the lack of driving explanation data on this widely-used AD dataset.
OccLLaMA: An Occupancy-Language-Action Generative World Model for Autonomous Driving

Julong Wei, Shanshuai Yuan, Pengfei Li, Qingda Hu, Zhongxue Gan, Wenchao Ding
Publisher: Fudan University, Tsinghua University
Task: Perception(Occ) + Reasoning
Publish Date: 2024.09.05
Summary:
OccLLaMA, a unified 3D occupancy-language-action generative world model, which unifies VLA-related tasks including but not limited to scene understanding, planning, and 4D occupancy forecasting.
A novel scene tokenizer(VQVAE-like architecture) that efficiently discretize and reconstruct Occ scenes, considering sparsity and classes imbalance.
ContextVLM: Zero-Shot and Few-Shot Context Understanding for Autonomous Driving using Vision Language Models

Shounak Sural, Naren, Ragunathan Rajkumar ITSC 2024
Publisher: Carnegie Mellon University
Task: Context Recognition
Code: ContextVLM
Publish Date: 2024.08.30
Summary:
DrivingContexts, a large publicly-available datasetwith a combination of hand-annotated and machine annnotated labels to improve VLMs for better context recognition.
ContextVLM uses vision-language models to detect contexts using zero- and few-shot approaches.
DriveGenVLM: Real-world Video Generation for Vision Language Model based Autonomous Driving

Yongjie Fu, Anmol Jain, Xuan Di, Xu Chen, Zhaobin Mo IAVVC 2024
Publisher: Columbia University
Task: Generation
Dataset: Waymo open dataset
Publish Date: 2024.08.29
Summary:
DriveGenVLM employ a video generation framework based on Denoising Diffusion Probabilistic Models to create realistic video sequences that mimic real-world dynamics.
The videos generated are then evaluated for their suitability in Visual Language Models (VLMs) using a pre-trained model called Efficient In-context Learning on Egocentric Videos (EILEV).
Edge-Cloud Collaborative Motion Planning for Autonomous Driving with Large Language Models

Jiao Chen, Suyan Dai, Fangfang Chen, Zuohong Lv, Jianhua Tang
Publisher: South China University of Technology, Pazhou Lab
Task: Planning + QA
Project Page: EC-Drive
Publish Date: 2024.08.19
Summary:
EC-Drive, a novel edge-cloud collaborative autonomous driving system.
V2X-VLM: End-to-End V2X Cooperative Autonomous Driving Through Large Vision-Language Models

Junwei You, Haotian Shi, Zhuoyu Jiang, Zilin Huang, Rui Gan, Keshu Wu, Xi Cheng, Xiaopeng Li, Bin Ran
Publisher: University of Wisconsin-Madison, Nanyang Technological University, Texas A&M University, Cornell University
Task: Planning
Projcet Page: V2X-VLM
Code: V2X-VLM
Dataset: DAIR-V2X
Publish Date: 2024.08.09
Summary:
V2X-VLM, a large vision-language model empowered E2E VICAD framework, which improves the ability of autonomous vehicles to navigate complex traffic scenarios through advanced multimodal understanding and decision-making.
A contrastive learning technique is employed to refine the model’s ability to distinguish between relevant and irrelevant features, which ensures that the model learns robust and discriminative representations of specific driving environments, leading to improved accuracy in trajectory planning in V2X cooperation scenarios.
AgentsCoMerge: Large Language Model Empowered Collaborative Decision Making for Ramp Merging

Senkang Hu, Zhengru Fang, Zihan Fang, Yiqin Deng, Xianhao Chen, Yuguang Fang, Sam Kwong IEEE TMC
Publisher: City University of Hong Kong, The University of Hong Kong, Lingnan University
Task: Multi Agent Planning
Publish Date: 2024.08.07
Summary:
AgentsCoMerge, a large language model empowered collaborative decision making for ramp merging. It includes observation, planning, communication, and reinforcement training modules. Experiments demonstrate its effectiveness in improving multi-agent collaboration and efficiency.
VLM-MPC: Vision Language Foundation Model (VLM)-Guided Model Predictive Controller (MPC) for Autonomous Driving

Keke Long, Haotian Shi, Jiaxi Liu, Xiaopeng Li
Publisher: University of Wisconsin-Madison
Task: Planning
Publish Date: 2024.08.04
Summary:
It proposed a closed-loop autonomous driving controller that applies VLMs for high-level vehicle control.
The upper-level VLM uses the vehicle's front camera images, textual scenario description, and experience memory as inputs to generate control parameters needed by the lower-level MPC.
The lower-level MPC utilizes these parameters, considering vehicle dynamics with engine lag, to achieve realistic vehicle behavior and provide state feedback to the upper level.
This asynchronous two-layer structure addresses the current issue of slow VLM response speeds.
SimpleLLM4AD: An End-to-End Vision-Language Model with Graph Visual Question Answering for Autonomous Driving

Peiru Zheng, Yun Zhao, Zhan Gong, Hong Zhu, Shaohua Wu IEIT Systems
Publisher: University of Wisconsin-Madison
Task: QA
Publish Date: 2024.07.31
Summary:
SimpleLLM4AD reimagines the traditional autonomous driving pipeline by structuring the task into four interconnected stages: perception, prediction, planning, and behavior.
Each stage is framed as a series of visual question answering (VQA) pairs, which are interlinked to form a Graph VQA (GVQA). This graph-based structure allows the system to reason about each VQA pair systematically, ensuring a coherent flow of information and decision-making from perception to action.
Testing Large Language Models on Driving Theory Knowledge and Skills for Connected Autonomous Vehicles

Zuoyin Tang, Jianhua He, Dashuai Pei, Kezhong Liu, Tao Gao
Publisher: Aston University, Essex University, Wuhan University of Technology, Chang’An University
Task: Evaluation
Publish Date: 2024.07.24
Data: UK Driving Theory Test Practice Questions and Answers
Summary:
Design and run driving theory tests for several proprietary LLM models (OpenAI GPT models, Baidu Ernie and Ali QWen) and open-source LLM models (Tsinghua MiniCPM-2B and MiniCPM-Llama3-V2.5) with more than 500 multiple-choices theory test questions.
KoMA: Knowledge-driven Multi-agent Framework for Autonomous Driving with Large Language Models

Kemou Jiang, Xuan Cai, Zhiyong Cui, Aoyong Li, Yilong Ren, Haiyang Yu, Hao Yang, Daocheng Fu, Licheng Wen, Pinlong Cai
Publisher: Beihang University, Johns Hopkins University, Shanghai Artificial Intelligence Laboratory
Task: Multi Agent Planning
Env: HighwayEnv
Project Page: KoMA
Publish Date: 2024.07.19
Summary:
Introduce a knowledge-driven autonomous driving framework KoMA that incorporates multiple agents empowered by LLMs, comprising five integral modules: Environment, Multi-agent Interaction, Multi-step Planning, Shared Memory, and Ranking-based Reflection.
WOMD-Reasoning: A Large-Scale Language Dataset for Interaction and Driving Intentions Reasoning

Yiheng Li, Chongjian Ge, Chenran Li, Chenfeng Xu, Masayoshi Tomizuka, Chen Tang, Mingyu Ding, Wei Zhan
Publisher: UC Berkeley, UT Austin
Task: Dataset + Reasoning
Publish Date: 2024.07.05
Datasets: WOMD-Reasoning
Summary:
WOMD-Reasoning, a language dataset centered on interaction descriptions and reasoning. It provides extensive insights into critical but previously overlooked interactions induced by traffic rules and human intentions.
Develop an automatic language labeling pipeline, leveraging a rule-based translator to interpret motion data into language descriptions, and a set of manual prompts for ChatGPT to generate Q&A pairs.
Exploring the Potential of Multi-Modal AI for Driving Hazard Prediction

Korawat Charoenpitaks, Van-Quang Nguyen, Masanori Suganuma, Masahiro Takahashi, Ryoma Niihara, Takayuki Okatani IEEE TIV 2024
Publisher: Tohoku University, RIKEN Center for AIP, DENSO CORPORATION
Task: Prediction
Code: DHPR
Publish Date: 2024.06.21
Summary:
DHPR (Driving Hazard Prediction and Reasoning) dataset, consists of 15K dashcam images of street scenes, and each image is associated with a tuple containing car speed, a hypothesized hazard description, and visual entities present in the scene.
Present several baseline methods and evaluate their performance.
Asynchronous Large Language Model Enhanced Planner for Autonomous Driving

Yuan Chen, Zi-han Ding, Ziqin Wang, Yan Wang, Lijun Zhang, Si Liu ECCV 2024
Publisher: Beihang University, Tsinghua University
Task: Planning
Publish Date: 2024.06.20
Code: AsyncDriver
Datasets: nuPlan Closed-Loop Reactive Hard20
Summary:
AsyncDriver, a novel asynchronous LLM-enhanced framework, in which the inference frequency of LLM is controllable and can be decoupled from that of the real-time planner.
Adaptive Injection Block, which is model-agnostic and can easily integrate scene-associated instruction features into any transformer based real-time planner, enhancing its ability in comprehending and following series of language-based routing instructions.
Compared with existing methods, our approach demonstrates superior closedloop evaluation performance in nuPlan’s challenging scenarios.
A Superalignment Framework in Autonomous Driving with Large Language Models

Xiangrui Kong, Thomas Braunl, Marco Fahmi, Yue Wang
Publisher: University of Western Australia, Queensland Government, Brisbane, Queensland University of Technology
Task: QA
Publish Date: 2024.06.09
Summary
Propose a secure interaction framework for LLMs to effectively audit data interacting with cloud-based LLMs.
Analyze 11 autonomous driving methods based on large language models, including driving safety, token usage, privacy, and consistency with human values.
Evaluate the effectiveness of driving prompts in the nuScenesQA dataset and compare different results between gpt-35-turbo and llama2-70b LLM backbones.
PlanAgent: A Multi-modal Large Language Agent for Closed-loop Vehicle Motion Planning

Yupeng Zheng, Zebin Xing, Qichao Zhang, Bu Jin, Pengfei Li, Yuhang Zheng, Zhongpu Xia, Kun Zhan, Xianpeng Lang, Yaran Chen, Dongbin Zhao
Publisher: Chinese Academy of Sciences, Beijing University of Posts and Telecommunications, Beihang University, Tsinghua University, Li Auto
Task: Planning
Publish Date: 2024.06.04
Summary:
PlanAgent is the first closed-loop mid-to-mid(use bev, no raw sensor) autonomous driving planning agent system based on a Multi-modal Large Language Model.
Propose an efficient Environment Transformation module that extracts multi-modal information inputs with lanegraph representation.
Design a Reasoning Engine module that introduces a hierarchical chain-of-thought (CoT) to instruct MLLM to generate planner code and a Reflection module that combines simulation and scoring to filter out unreasonable proposals generated by the MLLM.
ChatScene: Knowledge-Enabled Safety-Critical Scenario Generation for Autonomous Vehicles

Jiawei Zhang, Chejian Xu, Bo Li CVPR 2024
Publisher: UIUC, UChicago
Task: Scenario Generation
Env: Carla
Code: ChatScene
Publish Date: 2024.05.22
Summary:
ChatScene, a novel LLM-based agent capable of generating safety-critical scenarios by first providing textual descriptions and then carefully transforming them into executable simulations in CARLA via Scenic programming language.
An expansive retrieval database of Scenic code snippets has been developed. It catalogs diverse adversarial behaviors and traffic configurations, utilizing the rich knowledge stored in LLMs, which significantly augments the variety and critical nature of the driving scenarios generated.
Probing Multimodal LLMs as World Models for Driving

Shiva Sreeram, Tsun-Hsuan Wang, Alaa Maalouf, Guy Rosman, Sertac Karaman, Daniela Rus
Publisher: MIT CSAIL, TRI, MIT LID
Task: Benchmark & Evaluation
Code: DriveSim
Publish Date: 2024.05.09
Summary:
A comprehensive experimental study to evaluate the capability of different MLLMs to reason/understand scenarios involving closed-loop driving and making decisions.
DriveSim, a specialized simulator designed to generate a diverse array of driving scenarios, thereby providing a platform to test and evaluate/benchmark the capabilities of MLLMs in understanding and reasoning about real-world driving scenes from a fixed in-car camera perspective, the same as the drive viewpoint.
OmniDrive: A Holistic LLM-Agent Framework for Autonomous Driving with 3D Perception Reasoning and Planning

Shihao Wang, Zhiding Yu, Xiaohui Jiang, Shiyi Lan, Min Shi, Nadine Chang, Jan Kautz, Ying Li, Jose M. Alvarez
Publisher: Beijing Inst of Tech, NVIDIA, Huazhong Univ of Sci and Tech
Task: Benchmark & Planning
Publisher Data: 2024.05.02
Code: OmniDrive
Summary:
OmniDrive, a holistic framework for strong alignment between agent models and 3D driving tasks.
Propose a new benchmark with comprehensive visual question-answering (VQA) tasks, including scene description, traffic regulation, 3D grounding, counterfactual reasoning, decision making and planning.
Chat2Scenario: Scenario Extraction From Dataset Through Utilization of Large Language Model

Yongqi Zhao, Wenbo Xiao, Tomislav Mihalj, Jia Hu, Arno Eichberger IEEE IV 2024
Publisher:
Publisher Data: 2024.04.26
Task: Generation
Dataset: Chat2Scenario
Summary:
Chat2Scenario is a web-based tool that allows users to search for specific driving scenarios within a dataset by inputting descriptive functional scenario text.
VLAAD: Vision and Language Assistant for Autonomous Driving

SungYeon Park, MinJae Lee, JiHyuk Kang, Hahyeon Choi, Yoonah Park, Juhwan Cho, Adam Lee, DongKyu Kim WACV 2024 WorkShop
Publisher: Seoul National University, University of California, Berkeley
Publisher Data: 2024.04.16
Task: VQA
Code: VLAAD
Summary:
Introduce a multi-modal instruction tuning dataset that facilitates language models in learning visual instructions across diverse driving scenarios.
Capitalizing on this dataset, present a multi-modal LLM driving assistant named VLAAD.
REvolve: Reward Evolution with Large Language Models for Autonomous Driving

Rishi Hazra, Alkis Sygkounas, Andreas Persson, Amy Loutfi, Pedro Zuidberg Dos Martires
Publisher: Centre for Applied Autonomous Sensor Systems (AASS), Örebro University, Swede
Task: Reward Generation
Env: AirSim
Project Page: REvolve
Publish Date: 2024.04.09
Summary:
Reward Evolve (REvolve), a novel evolutionary framework using LLMs, specifically GPT-4, to output reward functions (as executable Python codes) for AD and evolve them based on human feedback.
AGENTSCODRIVER: Large Language Model Empowered Collaborative Driving with Lifelong Learning

Senkang Hu, Zhengru Fang, Zihan Fang, Xianhao Chen, Yuguang Fang
Publisher: City University of Hong Kong, The University of Hong Kong
Task: Planning(Multiple vehicles collaborative)
Publish Date: 2024.04.09
Env: HighwayEnv
Summary:
AGENTSCODRIVER, an LLM-powered multi-vehicle collaborative driving framework with lifelong learning, which allows different driving agents to communicate with each other and collaboratively drive in complex traffic scenarios.
It features reasoning engine, cognitive memory, reinforcement reflection, and communication module.
Multi-Frame, Lightweight & Efficient Vision-Language Models for Question Answering in Autonomous Driving

Akshay Gopalkrishnan, Ross Greer, Mohan Trivedi
Publisher: UCSD
Task: QA
Publish Date: 2024.03.28
Code: official
Datasets: DriveLM
Summary:
EM-VLM4AD, an efficient, lightweight, multi-frame vision language model which performs Visual Question Answering for autonomous driving.
EM-VLM4AD requires at least 10 times less memory and floating point operations, while also achieving higher BLEU-4, METEOR, CIDEr, and ROGUE scores than the existing baseline on the DriveLM dataset.
LC-LLM: Explainable Lane-Change Intention and Trajectory Predictions with Large Language Models

Mingxing Peng, Xusen Guo, Xianda Chen, Meixin Zhu, Kehua Chen, Hao (Frank) Yang, Xuesong Wang, Yinhai Wang
Publisher: The Hong Kong University of Science and Technology, Johns Hopkins University, Tongji University, STAR Lab
Task: Trajectory Prediction
Publish Date: 2024.03.27
Datasets: highD
Summary:
LC-LLM, the first Large Language Model for lane change prediction. It leverages the powerful capabilities of LLMs to understand complex interactive scenarios, enhancing the performance of lane change prediction.
LC-LLM achieves explainable predictions. It not only predicts lane change intentions and trajectories but also generates explanations for the prediction results.
AIDE: An Automatic Data Engine for Object Detection in Autonomous Driving

Mingfu Liang, Jong-Chyi Su, Samuel Schulter, Sparsh Garg, Shiyu Zhao, Ying Wu, Manmohan Chandraker
Publisher: Northwestern University, NEC Laboratories America, Rutgers University, UC San Diego
Publish Date: 2024.03.26
Task: Object Detection
Datasets: Mapillary, Cityscapes, nuImages, BDD100k, Waymo, KITTI
Summary:
An Automatic Data Engine (AIDE) that can automatically identify the issues, efficiently curate data, improve the model using auto-labeling, and verify the model through generated diverse scenarios.
Engineering Safety Requirements for Autonomous Driving with Large Language Models

Ali Nouri, Beatriz Cabrero-Daniel, Fredrik Törner, Hȧkan Sivencrona, Christian Berger
Publisher: Chalmers University of Technology, University of Gothenburg, Volvo Cars, Zenseact, University of Gothenburg
Task: QA
Publish Date: 2024.03.24
Summary:
Propose a prototype of a pipeline of prompts and LLMs that receives an item definition and outputs solutions in the form of safety requirements.
LeGo-Drive: Language-enhanced Goal-oriented Closed-Loop End-to-End Autonomous Driving

Pranjal Paul, Anant Garg, Tushar Choudhary, Arun Kumar Singh, K. Madhava Krishna
Publisher: The International Institute of Information Technology, Hyderabad, University of Tartu, Estonia
Project Page: LeGo-Drive
Code: LeGo-Drive
Env: Carla
Task: Trajectory Prediction
Publish Date: 2024.03.20
Summary:
A novel planning-guided end-to-end LLM-based goal point navigation solution that predicts and improves the desired state by dynamically interacting with the environment and generating a collision-free trajectory.
Hybrid Reasoning Based on Large Language Models for Autonomous Car Driving

Mehdi Azarafza, Mojtaba Nayyeri, Charles Steinmetz, Steffen Staab, Achim Rettberg
Publisher: Univ. of Applied Science Hamm-Lippstadt, University of Stuttgart
Publish Date: 2024.03.18
Task: Reasoning
Env: Carla
Summary:
Combining arithmetic and commonsense elements, utilize the objects detected by YOLOv8.
Regarding the "location of the object," "speed of our car," "distance to the object," and "our car’s direction" are fed into the large language model for mathematical calculations within CARLA.
หลังจากการคำนวณเหล่านี้โดยอิงจากการเอาชนะสภาพอากาศแล้ว จะได้ค่าควบคุมที่แม่นยำสำหรับเบรกและความเร็ว
Large Language Models Powered Context-aware Motion Prediction

Xiaoji Zheng, Lixiu Wu, Zhijie Yan, Yuanrong Tang, Hao Zhao, Chen Zhong, Bokui Chen, Jiangtao Gong
Publisher: Tsinghua University
Task: Motion Prediction
เผยแพร่ข้อมูล: 2024.03.17
ชุดข้อมูล: WOMD
สรุป:
ออกแบบและดำเนินการทางวิศวกรรมที่รวดเร็วเพื่อให้ GPT4-V ที่ไม่ได้ปรับแต่งอย่างละเอียดสามารถเข้าใจสถานการณ์การรับส่งข้อมูลที่ซับซ้อนได้
แนะนำแนวทางใหม่ที่ผสมผสานข้อมูลบริบทที่ส่งออกโดย GPT4-V เข้ากับMTR
แบบจำลองการทำนายทั่วไปสำหรับการขับขี่อัตโนมัติ

เจียจือ หยาง, เสินหยวน เกา, ยี่ฮัง ชิว, หลี่ เฉิน, เทียนหยู่ ลี่, โป ได, คาชยัป ชิตต้า, เผิงห่าว วู, เจีย เซง, ปิงหลัว, จุน จาง, อันเดรียส ไกเกอร์, หยู เฉียว, หงหยาง หลี่อีซีซีวี 2024
ผู้จัดพิมพ์: OpenDriveLab และ Shanghai AI Lab, มหาวิทยาลัยวิทยาศาสตร์และเทคโนโลยีฮ่องกง, มหาวิทยาลัยฮ่องกง, มหาวิทยาลัยทูบิงเงน, ศูนย์ AI ทูบิงเงน
งาน: ชุดข้อมูล + การสร้าง
รหัส: DriveAGI
วันที่เผยแพร่: 2024.03.14
สรุป:
แนะนำโมเดลการคาดการณ์วิดีโอขนาดใหญ่รุ่นแรกในสาขาการขับขี่อัตโนมัติ
ชุดข้อมูลที่ได้จะรวบรวมวิดีโอการขับรถมากกว่า 2,000 ชั่วโมง ครอบคลุมพื้นที่ทั่วโลกที่มีสภาพอากาศและสถานการณ์การจราจรที่หลากหลาย
GenAD สืบทอดข้อดีจากโมเดลการแพร่กระจายแฝงล่าสุด จัดการกับพลวัตที่ท้าทายในฉากการขับเคลื่อนด้วยบล็อกการใช้เหตุผลเชิงเวลาแบบใหม่
LLM-Assisted Light: การใช้ประโยชน์จากความสามารถของโมเดลภาษาขนาดใหญ่สำหรับการควบคุมสัญญาณไฟจราจรแบบเลียนแบบมนุษย์ในสภาพแวดล้อมเมืองที่ซับซ้อน

เหมาหนาน หวาง, อ้าวหยู ปัง, หยูเหิงกัน, มานออนปัน, ชุงซือเฉิน, โบฮวง
ผู้จัดพิมพ์: มหาวิทยาลัยจีนแห่งฮ่องกง ห้องปฏิบัติการ AI เซี่ยงไฮ้ SenseTime Group Limited และ Nokia Bell Labs
วันที่เผยแพร่: 2024.03.13
ภารกิจ: การสร้าง
รหัส: LLM-Assisted-Light
สรุป:
LA-Light กรอบงาน TSC แบบไฮบริดที่บูรณาการความสามารถในการใช้เหตุผลเลียนแบบมนุษย์ของ LLM ทำให้อัลกอริทึมการควบคุมสัญญาณสามารถตีความและตอบสนองต่อสถานการณ์การจราจรที่ซับซ้อนด้วยการตัดสินที่มีความละเอียดอ่อนตามแบบฉบับของการรับรู้ของมนุษย์
มีการพัฒนาระบบควบคุมสัญญาณไฟจราจรแบบวงปิด โดยบูรณาการ LLM เข้ากับชุดเครื่องมือที่ใช้งานร่วมกันได้อย่างครอบคลุม
DriveDreamer-2: โมเดลโลก LLM-Enhanced สำหรับการสร้างวิดีโอการขับขี่ที่หลากหลาย

Guosheng Zhao, Xiaofeng Wang, Zheng Zhu, Xinze Chen, Guan Huang, Xiaoyi Bao, Xingang Wang
ผู้จัดพิมพ์: สถาบันระบบอัตโนมัติ สถาบันวิทยาศาสตร์จีน GigaAI
วันที่เผยแพร่: 2024.03.11
ภารกิจ: การสร้าง
โครงการ: DriveDreamer-2
ชุดข้อมูล: nuScenes
สรุป:
DriveDreamer-2 ซึ่งสร้างขึ้นบนกรอบงานของDriveDreamerและรวม Large Language Model (LLM) เพื่อสร้างวิดีโอการขับขี่ที่ผู้ใช้กำหนด
UniMVM (Unified Multi-View Model) ช่วยเพิ่มการเชื่อมโยงทางเวลาและพื้นที่ในวิดีโอการขับขี่ที่สร้างขึ้น
เครื่องสร้าง HDMap ช่วยให้แน่ใจว่าองค์ประกอบพื้นหลังไม่ขัดแย้งกับวิถีพื้นหน้า
ใช้ชุดข้อมูลข้อความเป็นสคริปต์ที่สร้างขึ้นเพื่อปรับแต่ง GPT-3.5 ให้เป็น LLM โดยมีความรู้เฉพาะด้านการสร้างวิถี
การจำลองฉากที่แก้ไขได้สำหรับการขับขี่อัตโนมัติผ่านตัวแทน LLM แบบร่วมมือ

หยูซี เว่ย, ซี หวาง, ยี่ฟาน ลู่, เฉินซิน ซู, ฉางซิง หลิว, ห่าว จ้าว, ซีเหิง เฉิน, หยานเฟิง หวาง
สำนักพิมพ์: มหาวิทยาลัยเซี่ยงไฮ้เจียวทง, ห้องปฏิบัติการปัญญาประดิษฐ์เซี่ยงไฮ้, มหาวิทยาลัยคาร์เนกีเมลลอน, มหาวิทยาลัยชิงหัว
วันที่เผยแพร่: 2024.03.11
ภารกิจ: การสร้าง
รหัส: ChatSim
ชุดข้อมูล: Waymo
สรุป:
ChatSim ระบบแรกที่ทำให้สามารถจำลองฉากการขับขี่แบบ 3 มิติที่สมจริงและแก้ไขได้โดยใช้คำสั่งภาษาธรรมชาติด้วยทรัพยากรดิจิทัลภายนอก
McNeRF วิธีการฉายรังสีนิวรอลแบบใหม่ที่ผสานรวมอินพุตจากกล้องหลายตัว มอบการเรนเดอร์ฉากที่กว้างขึ้น ช่วยสร้างผลลัพธ์ที่สมจริงราวกับภาพถ่าย
McLight ระบบประเมินแสงแบบหลายกล้องแบบใหม่ที่ผสานรวมสกายโดมและแสงโดยรอบเข้าด้วยกัน สร้างทรัพยากรดิจิทัลภายนอกด้วยพื้นผิวและวัสดุที่สมจริง
ความเข้าใจเชิงลึกเกี่ยวกับสถานการณ์การขับขี่

หยุนซง โจว, ลินหยาน หวง, ชิงเหวิน ปู้, เจีย เจิ้ง, เทียนหยู ลี, หัง ชิว, หงซี จู, มินยี่ กัว, หยู เฉียว, หงหยาง ลีECCV 2024
ห้องปฏิบัติการ AI เซี่ยงไฮ้ มหาวิทยาลัยเซี่ยงไฮ้เจียวทง มหาวิทยาลัยแคลิฟอร์เนีย ริเวอร์ไซด์
วันที่เผยแพร่: 2024.03.07
งาน: เกณฑ์มาตรฐานและความเข้าใจฉาก
รหัส: ELM
สรุป:
ELM เป็นโมเดลภาษาที่เป็นรูปธรรมสำหรับการทำความเข้าใจสถานการณ์การขับขี่ในระยะไกลในเชิงพื้นที่และเวลา
DriveVLM: การบรรจบกันของการขับขี่อัตโนมัติและโมเดลภาษาวิสัยทัศน์ขนาดใหญ่

เซียวหยู เทียน, จุนหรู กู่, ไป๋หลิน ลี่, อี้เฉิง หลิว, เฉินซู หู, หยาง หวาง, คุนจ้าน, เผิงเจีย, เซียนเผิงหลาง, หางจ้าว
สำนักพิมพ์: IIIS, มหาวิทยาลัยชิงหัว, Li Auto
วันที่เผยแพร่: 25.02.2567
งาน: + การวางแผน
โครงการ: DriveVLM
ชุดข้อมูล: nuScenes , SUP-AD
สรุป:
DriveVLM ระบบขับขี่อัตโนมัติรูปแบบใหม่ที่ใช้ประโยชน์จาก VLM เพื่อความเข้าใจและการวางแผนฉากอย่างมีประสิทธิภาพ
DriveVLM-Dual ระบบไฮบริดที่รวม DriveVLM และระบบท่ออัตโนมัติแบบดั้งเดิมเข้าด้วยกัน
GenAD: ระบบขับขี่อัตโนมัติแบบ End-to-End เชิงสร้างสรรค์

เหวินจ้าว เจิ้ง, รุ่ยฉี ซ่ง, ซีอันดา กัว, หลง เฉิน ECCV 2024
มหาวิทยาลัยแคลิฟอร์เนีย เบิร์กลีย์ เวย์ทัส สถาบันอัตโนมัติ สถาบันวิทยาศาสตร์จีน
วันที่เผยแพร่: 20.02.2024
ภารกิจ: การสร้าง
รหัส: GenAD
ชุดข้อมูล: nuScenes
สรุป:
GenAD สร้างแบบจำลองการขับขี่อัตโนมัติเป็นปัญหาการสร้างวิถีเพื่อปลดล็อกศักยภาพทั้งหมดของวิธีการแบบครบวงจร
เสนอตัวสร้างโทเค็นฉากที่เน้นอินสแตนซ์ซึ่งจะแปลงฉากโดยรอบเป็นโทเค็นอินสแตนซ์ที่รับรู้แผนที่ก่อน
ใช้ตัวเข้ารหัสอัตโนมัติแบบแปรผันเพื่อเรียนรู้การกระจายวิถีในอนาคตในพื้นที่แฝงเชิงโครงสร้างสำหรับการสร้างแบบจำลองก่อนหน้าวิถี และนำแบบจำลองชั่วคราวมาใช้เพื่อจับภาพการเคลื่อนไหวของตัวแทนและอัตตาในพื้นที่แฝงเพื่อสร้างวิถีในอนาคตที่มีประสิทธิภาพมากขึ้น
RAG-Driver: คำอธิบายการขับขี่แบบทั่วไปพร้อมการเรียนรู้แบบบริบทที่เสริมการดึงข้อมูลในแบบจำลองภาษาขนาดใหญ่แบบหลายโหมด

Jianhao Yuan, Shuyang Sun, Daniel Omeiza, Bo Zhao, Paul Newman, Lars Kunze, Matthew Gadd
Publisher: University of Oxford, Beijing Academy of Artificial Intelligence
Publish Date: 2024.02.16
Task: Explainable Driving
Project: RAG-Driver
Summary:
RAG-Driver is a Multi-Modal Large Language Model with Retrieval-augmented In-context Learning capacity designed for generalisable and explainable end-to-end driving with strong zero-shot generalisation capacity.
Achieve State-of-the-art action explanation and justification performance in both BDD-X (in-distribution) and SAX (out-distribution) benchmarks.
Driving Everywhere with Large Language Model Policy Adaptation

Boyi Li, Yue Wang, Jiageng Mao, Boris Ivanovic, Sushant Veer, Karen Leung, Marco Pavone CVPR 2024
Publisher: NVIDIA, University of Southern California, University of Washington, Stanford University
Publish Date: 2024.02.08
Task: Planning
Datasets: nuScenes
Project: LLaDA
Summary:
LLaDA is a training-free mechanism to assist human drivers and adapt autonomous driving policies to new environments.
Traffic Rule Extractor (TRE), which aims to organize and filter the inputs (initial plan+unique traffic code) and feed the output into the frozen LLMs to obtain the final new plan.
LLaDA set GPT-4 as default LLM.
LimSim++

Daocheng Fu, Wenjie Lei, Licheng Wen, Pinlong Cai, Song Mao, Min Dou, Botian Shi, Yu Qiao
Publisher: Shanghai Artificial Intelligence Laboratory, Zhejiang University
Publish Date: 2024.02.02
Project: LimSim++
Summary:
LimSim++, an extended version of LimSim designed for the application of (M)LLMs in autonomous driving.
Introduce a baseline (M)LLM-driven framework, systematically validated through quantitative experiments across diverse scenarios.
LangProp: A code optimization framework using Language Models applied to driving

Shu Ishida, Gianluca Corrado, George Fedoseev, Hudson Yeo, Lloyd Russell, Jamie Shotton, João F. Henriques, Anthony Hu
Publisher: Wayve Technologies, Visual Geometry Group, University of Oxford
Publish Date: 2024.01.18
Task: Code generation, Planning
Code: LangProp
Env: CARLA
Summary:
LangProp is a framework for iteratively optimizing code generated by large language models (LLMs) in a supervised/reinforcement learning setting.
Use LangProp in CARLA and generate driving code based on the state of the scene.
VLP: Vision Language Planning for Autonomous Driving

Chenbin Pan, Burhaneddin Yaman, Tommaso Nesti, Abhirup Mallik, Alessandro G Allievi, Senem Velipasalar, Liu Ren CVPR 2024
Publisher: Syracuse University, Bosch Research North America & Bosch Center for Artificial Intelligence (BCAI)
Publish Date: 2024.01.14
Datasets: nuScenes
Summary:
Propose VLP, a Vision Language Planning model, which is composed of novel components ALP and SLP, aiming to improve the ADS from self-driving BEV reasoning and self-driving decision-making aspects, respectively.
ALP(agent-wise learning paradigm) aligns the produced BEV with a true bird’s-eye-view map.
SLP(selfdriving-car-centric learning paradigm) aligns the ego-vehicle query feature with the ego-vehicle textual planning feature.
DME-Driver: Integrating Human Decision Logic and 3D Scene Perception in Autonomous Driving

Wencheng Han, Dongqian Guo, Cheng-Zhong Xu, and Jianbing Shen
Publisher: SKL-IOTSC, CIS, University of Macau
Publish Date: 2024.01.08
Summary:
DME-Driver = Decision-Maker + Executor + CL
Executor network which is based on UniAD incorporates textual information for the OccFormer and the Planning module.
Decision-Maker which is based on LLaVA process inputs from three different modalities: visual inputs from the current and previous scenes textual inputs in the form of prompts, and current status information detailing the vehicle’s operating state.
CL is a consistency loss mechanism, slightly reducing performance metrics but significantly enhancing decision alignment between Executor and Decision-Maker.
AccidentGPT: Accident Analysis and Prevention from V2X Environmental Perception with Multi-modal Large Model

Lening Wang, Yilong Ren, Han Jiang, Pinlong Cai, Daocheng Fu, Tianqi Wang, Zhiyong Cui, Haiyang Yu, Xuesong Wang, Hanchu Zhou, Helai Huang, Yinhai Wang
Publisher: Beihang University, Shanghai Artificial Intelligence Laboratory, The University of Hong Kong, Zhongguancun Laboratory, Tongji University, Central South University, University of Washington, Seattle
Publish Date: 2023.12.29
Project page: AccidentGPT
Summary:
AccidentGPT, a comprehensive accident analysis and prevention multi-modal large model.
Integrates multi-vehicle collaborative perception for enhanced environmental understanding and collision avoidance.
Offer advanced safety features such as proactive remote safety warnings and blind spot alerts.
Serve traffic police and management agencies by providing real-time intelligent analysis of traffic safety factors.
Holistic Autonomous Driving Understanding by Bird’s-Eye-View Injected Multi-Modal Large Models

Xinpeng Ding, Jinahua Han, Hang Xu, Xiaodan Liang, Wei Zhang, Xiaomeng Li CVPR 2024
Publisher: Hong Kong University of Science and Technology, Huawei Noah’s Ark Lab, Sun Yat-Sen University
Publish Date: 2023.12.21
Task: Datasets + VQA
Code: official
Summary:
Introduce NuInstruct, a novel dataset with 91K multi-view video-QA pairs across 17 subtasks, which based on nuScenes.
Propose BEV-InMLMM to integrate instructionaware BEV features with existing MLLMs, enhancing them with a full suite of information, including temporal, multi-view, and spatial details.
LLM-ASSIST: Enhancing Closed-Loop Planning with Language-Based Reasoning

S P Sharan, Francesco Pittaluga, Vijay Kumar B G, Manmohan Chandraker
Publisher: UT Austin， NEC Labs America， UC San Diego
Publish Date: 2023.12.30
Task: Planning
Env/Datasets: nuPlan Closed-Loop Non-Reactive Challenge
Project: LLM-ASSIST
Summary:
LLM-Planner takes over scenarios that PDM-Closed cannot handle
Propose two LLM-based planners.
LLM-ASSIST(unc) considers the most unconstrained version of the planning problem, in which the LLM must directly return a safe future trajectory for the ego car.
LLM-ASSIST(par) considers a parameterized version of the planning problem, in which the LLM must only return a set of parameters for a rule-based planner, PDM-Closed.
DriveLM: Driving with Graph Visual Question Answering

Chonghao Sima, Katrin Renz, Kashyap Chitta, Li Chen, Hanxue Zhang, Chengen Xie, Ping Luo, Andreas Geiger, Hongyang Li ECCV 2024
Publisher: OpenDriveLab, University of Tübingen, Tübingen AI Center, University of Hong Kong
Code: official
Publish Date: 2023.12.21
Summary:
DriveLM-Task
Graph VQA involves formulating P1-3(Perception, Prediction, Planning) reasoning as a series of questionanswer pairs (QAs) in a directed graph.
DriveLM-Data
DriveLM-Carla
Collect data using CARLA 0.9.14 in the Leaderboard 2.0 framework [17] with a privileged rule-based expert.
Drive-nuScenes
Selecting key frames from video clips, choosing key objects within these key frames, and subsequently annotating the frame-level P1−3 QAs for these key objects. A portion of the Perception QAs are generated from the nuScenes and OpenLane-V2 ground truth, while the remaining QAs are manually annotated.
DriveLM-Agent
DriveLMAgent is built upon a general vision-language model and can therefore exploit underlying knowledge gained during pre-training.
LingoQA: Video Question Answering for Autonomous Driving

Ana-Maria Marcu, Long Chen, Jan Hünermann, Alice Karnsund, Benoit Hanotte, Prajwal Chidananda, Saurabh Nair, Vijay Badrinarayanan, Alex Kendall, Jamie Shotton, Oleg Sinavski
Publisher: Wayve
Task: VQA + Evaluation/Datasets
Code: official
Publish Date: 2023.12.21
Summary:
Introduce a novel benchmark for autonomous driving video QA using a learned text classifier for evaluation.
Introduce a Video QA dataset of central London consisting of 419k samples with its free-form questions and answers.
Establish a new baseline based on Vicuna-1.5-7B for this field with an identified model combination.
DriveMLM: Aligning Multi-Modal Large Language Models with Behavioral Planning States for Autonomous Driving

Wenhai Wang, Jiangwei Xie, ChuanYang Hu, Haoming Zou, Jianan Fan, Wenwen Tong, Yang Wen, Silei Wu, Hanming Deng, Zhiqi Li, Hao Tian, Lewei Lu, Xizhou Zhu, Xiaogang Wang, Yu Qiao, Jifeng Dai
Publisher: OpenGVLab, Shanghai AI Laboratory, The Chinese University of Hong Kong, SenseTime Research, Stanford University, Nanjing University, Tsinghua University
Task: Planning + Explanation
Code: official
Env: Carla
Publish Date: 2023.12.14
Summary:
DriveMLM, the first LLM-based AD framework that can perform close-loop autonomous driving in realistic simulators.
Design an MLLM planner for decision prediction, and develop a data engine that can effectively generate decision states and corresponding explanation annotation for model training and evaluation.
Achieve 76.1 DS, 0.955 MPI results on CARLA Town05 Long.
Large Language Models for Autonomous Driving: Real-World Experiments

Can Cui, Yunsheng Ma, Xu Cao, Wenqian Ye, Yang Zhou, Kaizhao Liang, Jintai Chen, Juanwu Lu, Zichong Yang, Kuei-Da Liao, Tianren Gao, Erlong Li, Kun Tang, Zhipeng Cao, Tong Zhou, Ao Liu, Xinrui Yan, Shuqi Mei, Jianguo Cao, Ziran Wang, Chao Zheng
Publisher: Purdue University
Publish Date: 2023.12.14
Project: official
Summary:
Introduce a Large Language Model (LLM)-based framework Talk-to-Drive (Talk2Drive) to process verbal commands from humans and make autonomous driving decisions with contextual information, satisfying their personalized preferences for safety, efficiency, and comfort.
LMDrive: Closed-Loop End-to-End Driving with Large Language Models

Hao Shao, Yuxuan Hu, Letian Wang, Steven L. Waslander, Yu Liu, Hongsheng Li CVPR 2024
Publisher: CUHK MMLab, SenseTime Research, CPII under InnoHK, University of Toronto, Shanghai Artificial Intelligence Laboratory
Task: Planning + Datasets
Code: official
Env: Carla
Publish Date: 2023.12.12
Summary:
LMDrive, a novel end-to-end, closed-loop, languagebased autonomous driving framework.
Release 64K clips dataset, including navigation instruction, notice instructions, multi-modal multi-view sensor data, and control signals.
Present the benchmark LangAuto for evaluating the autonomous agents.
Evaluation of Large Language Models for Decision Making in Autonomous Driving

Kotaro Tanahashi, Yuichi Inoue, Yu Yamaguchi, Hidetatsu Yaginuma, Daiki Shiotsuka, Hiroyuki Shimatani, Kohei Iwamasa, Yoshiaki Inoue, Takafumi Yamaguchi, Koki Igari, Tsukasa Horinouchi, Kento Tokuhiro, Yugo Tokuchi, Shunsuke Aoki
Publisher: Turing Inc., Japan
Task: Evalution
Publish Date: 2023.12.11
Summary:
Evaluate the two core capabilities
the spatial awareness decision-making ability, that is, LLMs can accurately identify the spatial layout based on coordinate information;
the ability to follow traffic rules to ensure that LLMs Ability to strictly abide by traffic laws while driving
LaMPilot: An Open Benchmark Dataset for Autonomous Driving with Language Model Programs

Yunsheng Ma, Can Cui, Xu Cao, Wenqian Ye, Peiran Liu, Juanwu Lu, Amr Abdelraouf, Rohit Gupta, Kyungtae Han, Aniket Bera, James M. Rehg, Ziran Wang
Publisher: Purdue University, University of Illinois Urbana-Champaign, University of Virginia, InfoTech Labs, Toyota Motor North American
Task: Benchmark
Publish Date: 2023.12.07
Summary:
LaMPilot is the first interactive environment and dataset designed for evaluating LLM-based agents in a driving context.
It contains 4.9K scenes and is specifically designed to evaluate command tracking tasks in autonomous driving.
Reason2Drive: Towards Interpretable and Chain-based Reasoning for Autonomous Driving

Ming Nie, Renyuan Peng, Chunwei Wang, Xinyue Cai, Jianhua Han, Hang Xu, Li Zhang
Publisher: Fudan University, Huawei Noah’s Ark Lab
Task: VQA + Datasets
Code: official
Datasets:
nuScenes
Waymo
ONCE
Publish Date: 2023.12.06
Summary:
Reason2Drive, a benchmark dataset with over 600K video-text pairs, aimed at facilitating the study of interpretable reasoning in complex driving.
Introduce a novel evaluation metric to assess chain-based reasoning performance in autonomous driving environments, and address the semantic ambiguities of existing metrics such as BLEU and CIDEr.
Introduce a straightforward yet effective framework that enhances existing VLMs with two new components: a prior tokenizer and an instructed vision decoder.
GPT-4 Enhanced Multimodal Grounding for Autonomous Driving: Leveraging Cross-Modal Attention with Large Language Models

Haicheng Liao, Huanming Shen, Zhenning Li, Chengyue Wang, Guofa Li, Yiming Bie, Chengzhong Xu
Publisher: University of Macau, UESTC, Chongqing University, Jilin University
Task: Detection/Prediction
Code: official
Datasets:
Talk2car
Publish Date: 2023.12.06
Summaray:
Utilize five encoder Text, Image, Context, and Cross-Modal—with a Multimodal decoder to pridiction object bounding box.
Dolphins: Multimodal Language Model for Driving

Yingzi Ma, Yulong Cao, Jiachen Sun, Marco Pavone, Chaowei Xiao ECCV 2024
Publisher: University of Wisconsin-Madison, NVIDIA, University of Michigan, Stanford University
Task: VQA
Project: Dolphins
Code: Dolphins
Datasets:
Image instruction-following dataset
GQA
MSCOCO: VQAv2, OK-VQA, TDIUC, Visual Genome dataset
Video instruction-following dataset
BDD-X
Publish Date: 2023.12.01
Summary:
Dolphins which is base on OpenFlamingo architecture is a VLM-based conversational driving assistant.
Devise grounded CoT (GCoT) instruction tuning and develop datasets.
Driving into the Future: Multiview Visual Forecasting and Planning with World Model for Autonomous Driving

Yuqi Wang, Jiawei He, Lue Fan, Hongxin Li, Yuntao Chen, Zhaoxiang Zhang
Publisher: CASIA, CAIR, HKISI, CAS
Task: Generation
Project: Drive-WM
Code: Drive-WM
Datasets: nuScenes, Waymo Open Dataset
Publish Date: 2023.11.29
Summary:
Drive-WM, a multiview world model, which is capable of generating high-quality, controllable, and consistent multiview videos in autonomous driving scenes.
The first to explore the potential application of the world model in end-to-end planning for autonomous driving.
Empowering Autonomous Driving with Large Language Models: A Safety Perspective

Yixuan Wang, Ruochen Jiao, Chengtian Lang, Sinong Simon Zhan, Chao Huang, Zhaoran Wang, Zhuoran Yang, Qi Zhu
Publisher: Northwestern University, University of Liverpool, Yale University
Task: Planning
Env: HighwayEnv
Code: official
Publish Date: 2023.11.28
Summary:
Deploys the LLM as an intelligent decision-maker in planning, incorporating safety verifiers for contextual safety learning to enhance overall AD performance and safety.
GPT-4V Takes the Wheel: Evaluating Promise and Challenges for Pedestrian Behavior Prediction

Jia Huang, Peng Jiang, Alvika Gautam, Srikanth Saripalli
Publisher: Texas A&M University, College Station, USA
Task: Evaluation(Pedestrian Behavior Prediction)
Datasets:
JAAD
PIE
WiDEVIEW
Summary:
Provides a comprehensive evaluation of the potential of GPT-4V for pedestrian behavior prediction in autonomous driving using publicly available datasets.
It still falls short of the state-of-the-art traditional domain-specific models.
While GPT-4V represents a considerable advancement in AI capabilities for pedestrian behavior prediction, ongoing development and refinement are necessary to fully harness its capabilities in practical applications.
ADriver-I: A General World Model for Autonomous Driving

Fan Jia, Weixin Mao, Yingfei Liu, Yucheng Zhao, Yuqing Wen, Chi Zhang, Xiangyu Zhang, Tiancai Wang
Publisher: MEGVII Technology, Waseda University, University of Science and Technology of China, Mach Drive
Task: Generation + Planning
Datasets: nuScenes, Largescale private datasets
Publish Date: 2023.11.22
Summary:
ADriver-I takes the vision-action pairs as inputs and autoregressively predicts the control signal of current frame. The generated control signals together with the historical vision-action pairs are further conditioned to predict the future frames.
MLLM(Multimodal large language model)=LLaVA-7B-1.5, VDM(Video Diffusion Model)=latent-diffusion
Metrics:
L1 error including speed and steer angle of current frame.
Quality of Generation: Frechet Inception Distance(FID), Frechet Video Distance(FVD).
A Language Agent for Autonomous Driving

Jiageng Mao, Junjie Ye, Yuxi Qian, Marco Pavone, Yue Wang
University of Southern California, Stanford University, NVIDIA
Task: Generation + Planning
Project: Agent-Driver
Datasets: nuScenes
Publish Date: 2023.11.17
Summary:
Agent-Driver integrates a tool library for dynamic perception and prediction, a cognitive memory for human knowledge, and a reasoning engine that emulates human decision-making.
For motion planning, follow GPT-Driver(#GPT-Driver) and fine-tune the LLM with human driving trajectories in the nuScenes training set for one epoch.
For neural modules, adopte the modules in UniAD.
Metric:
L2 error (in meters) and collision rate (in percentage).
Human-Centric Autonomous Systems With LLMs for User Command Reasoning

Yi Yang, Qingwen Zhang, Ci Li, Daniel Simões Marta, Nazre Batool, John Folkesson
Publisher: KTH Royal Institute of Technology, Scania AB
Task: QA
Code: DriveCmd
Datasets: UCU Dataset
Publish Date: 2023.11.14
Summary:
Propose to leverage the reasoning capabilities of Large Language Models (LLMs) to infer system requirements from in-cabin users’ commands.
LLVM-AD Workshop @ WACV 2024
Metric:
Accuracy at the question level(accuracy for each individual question).
Accuracy at the command level(accuracy is only acknowledged if all questions for a particular command are correctly identified).
On the Road with GPT-4V(ision): Early Explorations of Visual-Language Model on Autonomous Driving

Licheng Wen, Xuemeng Yang, Daocheng Fu, Xiaofeng Wang, Pinlong Cai, Xin Li, Tao Ma, Yingxuan Li, Linran Xu, Dengke Shang, Zheng Zhu, Shaoyan Sun, Yeqi Bai, Xinyu Cai, Min Dou, Shuanglu Hu, Botian Shi
Publisher: Shanghai Artificial Intelligence Laboratory, GigaAI, East China Normal University, The Chinese University of Hong Kong, WeRide.ai
Project: official
Datasets:
Scenario Understanding: nuScenes, BDD-X, Carla, TSDD, Waymo, DAIR-V2X, CitySim.
Reasoning Capability: nuScenes, D2-city, Carla, CODA and the internet
Act as a driver: Real-world driving scenarios.
Publish Date: 2023.11.9
Summary:
Conducted a comprehensive and multi-faceted evaluation of the GPT-4V in various autonomous driving scenarios.
Test the capabilities of GPT-4V in Scenario Understanding, Reasoning, Act as a driver.
ChatGPT as Your Vehicle Co-Pilot: An Initial Attempt

Shiyi Wang, Yuxuan Zhu, Zhiheng Li, Yutong Wang, Li Li, Zhengbing He
Publisher: Tsinghua University, Institute of Automation, Chinese Academy of Sciences, Massachusetts Institute of Technology
Task: Planning
Publish Date: 2023.10.17
Summary:
Design a universal framework that embeds LLMs as a vehicle "Co-Pilot" of driving, which can accomplish specific driving tasks with human intention satisfied based on the information provided.
MagicDrive: Street View Generation with Diverse 3D Geometry Control

Ruiyuan Gao, Kai Chen, Enze Xie, Lanqing Hong, Zhenguo Li, Dit-Yan Yeung, Qiang Xu
Publisher: The Chinese University of Hong Kong, Hong Kong University of Science and Technology, Huawei Noah’s Ark Lab
Task: Generation
Project: MagicDrive
Code: MagicDrive
Datasets: nuScenes
Publish Date: 2023.10.13
Summary:
MagicDrive generates highly realistic images, exploiting geometric information from 3D annotations by independently encoding road maps, object boxes, and camera parameters for precise, geometry-guided synthesis. This approach effectively solves the challenge of multi-camera view consistency.
It also faces huge challenges in some complex scenes, such as night views and unseen weather conditions.
Receive, Reason, and React: Drive as You Say with Large Language Models in Autonomous Vehicles

Can Cui, Yunsheng Ma, Xu Cao, Wenqian Ye, Ziran Wang
Publisher: Purdue University, University of Illinois Urbana-Champaign，University of Virginia，PediaMed.AI.
Task: Planning
Project: video
Env: HighwayEnv
Publish Date: 2023.10.12
Summary:
Utilize LLMs’ linguistic and contextual understanding abilities with specialized tools to integrate the language and reasoning capabilities of LLMs into autonomous vehicles.
DrivingDiffusion: Layout-Guided multi-view driving scene video generation with latent diffusion model

Xiaofan Li, Yifu Zhang, Xiaoqing Ye
Publisher: Baidu Inc.
Task: Generation
Project: official
Datasets: nuScenes
Summary:
Address the new problem of multi-view video data generation from 3D layout in complex urban scenes.'
Propose a generative model DrivingDiffusion to ensure the cross-view, cross-frame consistency and the instance quality of the generated videos.
Achieve state-of-the-art video synthesis performance on nuScenes dataset.
Metrics:
Quality of Generation: Frechet Inception Distance(FID), Frechet Video Distance(FVD)
Segmentation Metrics: mIoU
LanguageMPC: Large Language Models as Decision Makers for Autonomous Driving

Hao Sha, Yao Mu, Yuxuan Jiang, Li Chen, Chenfeng Xu, Ping Luo, Shengbo Eben Li, Masayoshi Tomizuka, Wei Zhan, Mingyu Ding
Publisher: Tsinghua University, The University of Hong Kong, University of California, Berkeley
Task: Planning/Control
Code: official
Env:
ComplexUrbanScenarios
Carla
Publish Date: 2023.10.04
Summary:
Leverage LLMs to provide high-level decisions through chain-of-thought.
Convert high-level decisions into mathematical representations to guide the bottom-level controller(MPC).
Metrics: Number of failure/collision cases， Inefficiency，time, Penalty
Driving with LLMs: Fusing Object-Level Vector Modality for Explainable Autonomous Driving

Long Chen, Oleg Sinavski, Jan Hünermann, Alice Karnsund, Andrew James Willmott, Danny Birch, Daniel Maund, Jamie Shotton
Publisher: Wayve
Task: Planning + VQA
Code: official
Simulator: a custom-built realistic 2D simulator.(The simulator is not open source.)
Datasets: Driving QA, data collection using RL experts in simulator.
Publish Date: 2023.10.03
Summary:
Propose a unique object-level multimodal LLM architecture(Llama2+Lora), using only vectorized representations as input.
Develop a new dataset of 160k QA pairs derived from 10k driving scenarios(control commands collected by RL(PPO), QA pair generated by GPT-3.5)
Metrics:
Accuracy of traffic light detection
MAE for traffic light distance prediction
MAE for acceleration
MAE for brake pressure
MAE for steering wheel angle
Talk2BEV: Language-enhanced Bird’s-eye View Maps for Autonomous Driving

Vikrant Dewangan, Tushar Choudhary, Shivam Chandhok, Shubham Priyadarshan, Anushka Jain, Arun K. Singh, Siddharth Srivastava, Krishna Murthy Jatavallabhula, K. Madhava Krishna
Publisher: IIIT Hyderabad, University of British Columbia, University of Tartu, TensorTour Inc, MIT
Project Page: official
Code: Talk2BEV
Publish Date: 2023.10.03
Summary:
Introduces Talk2BEV, a large visionlanguage model (LVLM) interface for bird’s-eye view (BEV) maps in autonomous driving contexts.
Does not require any training or finetuning, relying instead on pre-trained image-language models
Develop and release Talk2BEV-Bench, a benchmark encom- passing 1000 human-annotated BEV scenarios, with more than 20,000 questions and ground-truth responses from the NuScenes dataset.
DriveGPT4: Interpretable End-to-end Autonomous Driving via Large Language Model

Zhenhua Xu, Yujia Zhang, Enze Xie, Zhen Zhao, Yong Guo, Kenneth K. Y. Wong, Zhenguo Li, Hengshuang Zhao
Publisher: The University of Hong Kong, Zhejiang University, Huawei Noah’s Ark Lab, University of Sydney
Project Page: official
Task: Planning/Control + VQA
Datasets:
BDD-X dataset.
Publish Date: 2023.10.02
Summary:
Develop a new visual instruction tuning dataset(based on BDD-X) for interpretable AD assisted by ChatGPT/GPT4.
Present a novel multimodal LLM called DriveGPT4(Valley + LLaVA).
Metrics:
BLEU4, CIDEr and METETOR, ChatGPT Score.
RMSE for control signal prediction.
GPT-DRIVER: LEARNING TO DRIVE WITH GPT

Jiageng Mao, Yuxi Qian, Hang Zhao, Yue Wang
Publisher: University of Southern California, Tsinghua University
Task: Planning(Fine-tuning Pre-trained Model)
Project: official
Datasets: nuScenes
Code: GPT-Driver
Publish Date: 2023.10.02
Summary:
Motion planning as a language modeling problem.
Align the output of the LLM with human driving behavior through fine-tuning strategies using the OpenAI fine-tuning API.
Leverage the LLM to generate driving trajectories.
Metrics:
L2 metric and Collision rate
GAIA-1: A Generative World Model for Autonomous Driving

Anthony Hu, Lloyd Russell, Hudson Yeo, Zak Murez, George Fedoseev, Alex Kendall, Jamie Shotton, Gianluca Corrado
Publisher: Wayve
Task: Generation
Datasets:
Training dataset consists of 4,700 hours at 25Hz of proprietary driving data collected in London, UK between 2019 and 2023. It corresponds to approximately 420M unique images.
Validation dataset contains 400 hours of driving data from runs not included in the training set.
text coming from either online narration or offline metadata sources
Publish Date: 2023.09.29
Summary:
Introduce GAIA-1, a generative world model that leverages video(pre-trained DINO), text(T5-large), and action inputs to generate realistic driving scenarios.
Serve as a valuable neural simulator, allowing the generation of unlimited data.
DiLu: A Knowledge-Driven Approach to Autonomous Driving with Large Language Models

Licheng Wen, Daocheng Fu, Xin Li, Xinyu Cai, Tao Ma, Pinlong Cai, Min Dou, Botian Shi, Liang He, Yu Qiao ICLR 2024
Publisher: Shanghai AI Laboratory, East China Normal University, The Chinese University of Hong Kong
Publish Date: 2023.09.28
Task: Planning
Env:
HighwayEnv
CitySim, a Drone-Based vehicle trajectory dataset.
Summary:
Propose the DiLu framework, which combines a Reasoning and a Reflection module to enable the system to perform decision-making based on common-sense knowledge and evolve continuously.
SurrealDriver: Designing Generative Driver Agent Simulation Framework in Urban Contexts based on Large Language Model

Ye Jin, Xiaoxi Shen, Huiling Peng, Xiaoan Liu, Jingli Qin, Jiayang Li, Jintao Xie, Peizhong Gao, Guyue Zhou, Jiangtao Gong
Keywords: human-AI interaction, driver model, agent, generative AI, large language model, simulation framework
Env: CARLA
Publisher: Tsinghua University
Summary: Propose a generative driver agent simulation framework based on large language models (LLMs), capable of perceiving complex traffic scenarios and providing realistic driving maneuvers.
Drive as You Speak: Enabling Human-Like Interaction with Large Language Models in Autonomous Vehicles

Can Cui, Yunsheng Ma, Xu Cao, Wenqian Ye, Ziran Wang
Publisher: Purdue University, PediaMed.AI Lab, University of Virginia
Task: Planning
Publish Date: 2023.09.18
Summary:
Provide a comprehensive framework for integrating Large Language Models (LLMs) into AD.
DriveDreamer: Towards Real-world-driven World Models for Autonomous Driving

Xiaofeng Wang, Zheng Zhu, Guan Huang, Xinze Chen, Jiwen Lu ECCV 2024
Publisher: GigaAI, Tsinghua University
Task: Generation
Project Page: official
Datasets: nuScenes
Publish Date: 2023.09.18
Summary:
Harness the powerful diffusion model to construct a comprehensive representation of the complex environment.
Generate future driving videos and driving policies by a multimodal(text, image, HDMap, Action, 3DBox) world model.
Can you text what is happening? Integrating pre-trained language encoders into trajectory prediction models for autonomous driving

Ali Keysan, Andreas Look, Eitan Kosman, Gonca Gürsun, Jörg Wagner, Yu Yao, Barbara Rakitsch
Publisher: Bosch Center for Artificial Intelligence, University of Tubingen,
Task: Prediction
Datasets: nuScenes
Publish Date: 2023.09.13
Summary:
Integrating pre-trained language models as textbased input encoders for the AD trajectory prediction task.
Metrics:
minimum Average Displacement Error (minADEk)
Final Displacement Error (minFDEk)
MissRate over 2 meters
TrafficGPT: Viewing, Processing and Interacting with Traffic Foundation Models

Siyao Zhang, Daocheng Fu, Zhao Zhang, Bin Yu, Pinlong Cai
Publisher: Beihang University, Key Laboratory of Intelligent Transportation Technology and System, Shanghai Artificial Intelligence Laboratory
Task: Planning
Code: official
Publish Date: 2023.09.13
Summary:
Present TrafficGPT—a fusion of ChatGPT and traffic foundation models.
Bridges the critical gap between large language models and traffic foundation models by defining a series of prompts.
HiLM-D: Towards High-Resolution Understanding in Multimodal Large Language Models for Autonomous Driving

Xinpeng Ding, Jianhua Han, Hang Xu, Wei Zhang, Xiaomeng Li
Publisher: The Hong Kong University of Science and Technology, Huawei Noah’s Ark Lab
Task: Detection + VQA
Datasets: DRAMA
Publish Date: 2023.09.11
Summary:
Propose HiLM-D (Towards High-Resolution Understanding in MLLMs for Autonomous Driving), an efficient method to incorporate HR information into MLLMs for the ROLISP task.
ROLISP that aims to identify, explain and localize the risk object for the ego-vehicle meanwhile predicting its intention and giving suggestions.
Metrics:
LLM metrics, BLEU4, CIDEr and METETOR, SPICE.
Detection metrics, mIoU, IoUs so on.
Language Prompt for Autonomous Driving

Dongming Wu, Wencheng Han, Tiancai Wang, Yingfei Liu, Xiangyu Zhang, Jianbing Shen
Publisher: Beijing Institute of Technology, University of Macau, MEGVII Technology, Beijing Academy of Artificial Intelligence
Task: Tracking
Code: official
Datasets: NuPrompt(not open), based on nuScenes.
Publish Date: 2023.09.08
Summary:
Propose a new large-scale language prompt set(based on nuScenes) for driving scenes, named NuPrompt(3D object-text pairs).
Propose an efficient prompt-based tracking model with prompt reasoning modification on PFTrack, called PromptTrack.
MTD-GPT: A Multi-Task Decision-Making GPT Model for Autonomous Driving at Unsignalized Intersections

Jiaqi Liu, Peng Hang, Xiao Qi, Jianqiang Wang, Jian Sun. ITSC 2023
Publisher: Tongji University, Tsinghua University
Task: Prediction
Env: HighwayEnv
Publish Date: 2023.07.30
Summary:
Design a pipeline that leverages RL algorithms to train single-task decision-making experts and utilize expert data.
Propose the MTD-GPT model for multi-task(left-turn, straight-through, right-turn) decision-making of AV at unsignalized intersections.
Domain Knowledge Distillation from Large Language Model: An Empirical Study in the Autonomous Driving Domain

Yun Tang, Antonio A. Bruto da Costa, Xizhe Zhang, Irvine Patrick, Siddartha Khastgir, Paul Jennings. ITSC 2023
Publisher: University of Warwick
Task: QA
Publish Date: 2023.07.17
Summary:
Develop a web-based distillation assistant enabling supervision and flexible intervention at runtime by prompt engineering and the LLM ChatGPT.
Drive Like a Human: Rethinking Autonomous Driving with Large Language Models

Daocheng Fu, Xin Li, Licheng Wen, Min Dou, Pinlong Cai, Botian Shi, Yu Qiao
Publisher: Shanghai AI Lab, East China Normal University
Task: Planning
Code: official
Env: HighwayEnv
Publish Date: 2023.07.14
Summary:
Identify three key abilities: Reasoning, Interpretation and Memorization(accumulate experience and self-reflection).
Utilize LLM in AD as decision-making to solve long-tail corner cases and increase interpretability.
Verify interpretability in closed-loop offline data.
Language-Guided Traffic Simulation via Scene-Level Diffusion

Ziyuan Zhong, Davis Rempe, Yuxiao Chen, Boris Ivanovic, Yulong Cao, Danfei Xu, Marco Pavone, Baishakhi Ray
Publisher: Columbia University, NVIDIA Research, Stanford University, Georgia Tech
Task: Diffusion
Publish Date: 2023.07.10
Summary:
Present CTG++, a language-guided scene-level conditional diffusion model for realistic query-compliant traffic simulation.
Leverage an LLM for translating a user query into a differentiable loss function and propose a scene-level conditional diffusion model (with a spatial-temporal transformer architecture) to translate the loss function into realistic, query compliant trajectories.
ADAPT: Action-aware Driving Caption Transformer

Bu Jin, Xinyu Liu, Yupeng Zheng, Pengfei Li, Hao Zhao, Tong Zhang, Yuhang Zheng, Guyue Zhou, Jingjing Liu ICRA 2023
Publisher: Chinese Academy of Sciences, Tsinghua University, Peking University, Xidian University, Southern University of Science and Technology, Beihang University
Code: ADAPT
Datasets: BDD-X dataset
Summary:
Propose ADAPT, a new end-to-end transformerbased action narration and reasoning framework for self-driving vehicles.
propose a multi-task joint training framework that aligns both the driving action captioning task and the control signal prediction task.
WorkShop
Toggle
Large Language and Vision Models for Autonomous Driving(LLVM-AD) Workshop @ WACV 2024
Publisher: Tencent Maps HD Map T.Lab, University of Illinois Urbana- Champaign, Purdue University, University of Virginia
Challenge 1: MAPLM: A Large-Scale Vision-Language Dataset for Map and Traffic Scene Understanding
Datasets: Download
Task: QA
Code: https://github.com/LLVM-AD/MAPLM
Description: MAPLM combines point cloud BEV (Bird's Eye View) and panoramic images to provide a rich collection of road scenario images. It includes multi-level scene description data, which helps models navigate through complex and diverse traffic environments.
Metric:
Frame-overall-accuracy (FRM): A frame is considered correct if all closed-choice questions about it are answered correctly.
Question-overall-accuracy (QNS): A question is considered correct if its answer is correct.
LAN: How many lanes in current road?
INT: Is there any road cross, intersection or lane change zone in the main road?
QLT: What is the point cloud data quality in current road area of this image?
SCN: What kind of road scene is it in the images? (SCN)
Challenge 2: In-Cabin User Command Understanding (UCU)
Datasets: Download
Task: QA
Code: https://github.com/LLVM-AD/ucu-dataset
Description:
This dataset focuses on understanding user commands in the context of autonomous vehicles. It contains 1,099 labeled commands. Each command is a sentence that describes a user’s request to the vehicle.
Metric:
Command-level accuracy: A command is considered correctly understood if all eight answers are correct.
Question-level accuracy: Evaluation at the individual question level.
Datasets
Toggle
format:
- [title](dataset link) [links]
  - author1, author2, and author3...
  - keyword
  - experiment environments or tasks
CoVLA: Comprehensive Vision-Language-Action Dataset for Autonomous Driving

Hidehisa Arai, Keita Miwa, Kento Sasaki, Yu Yamaguchi, Kohei Watanabe, Shunsuke Aoki, Issei Yamamoto WACV 2025 Oral
Publisher: Turing Inc.
Publish Date: 2024.12.02
Code: CoVLA
Summary:
CoVLA (Comprehensive Vision-Language-Action) Dataset, an extensive dataset comprising real-world driving videos spanning more than 80 hours. This dataset leverages a novel, scalable approach based on automated data processing and a caption generation pipeline to generate accurate driving trajectories paired with detailed natural language descriptions of driving environments and maneuvers.
Rank2Tell: A Multimodal Driving Dataset for Joint Importance Ranking and Reasoning

Enna Sachdeva, Nakul Agarwal, Suhas Chundi, Sean Roelofs, Jiachen Li, Behzad Dariush, Chiho Choi, Mykel Kochenderfer
Publisher: Honda Research Institute, Stanford University
Publish Date: 2023.09.10
Summary:
A multi-modal ego-centric dataset for Ranking the importance level and Telling the reason for the importance.
Introduce a joint model for joint importance level ranking and natural language captions generation to benchmark our dataset.
DriveLM: Drive on Language

Publisher: Sima, Chonghao and Renz, Katrin and Chitta, Kashyap and Chen, Li and Zhang, Hanxue and Xie, Chengen and Luo, Ping and Geiger, Andreas and Li, Hongyang ECCV 2024
Dataset: DriveLM
Publish Date: 2023.08
Summary:
Construct dataset based on the nuScenes dataset.
Perception questions require the model to recognize objects in the scene.
Prediction questions ask the model to predict the future status of important objects in the scene.
Planning questions prompt the model to give reasonable planning actions and avoid dangerous ones.
WEDGE: A multi-weather autonomous driving dataset built from generative vision-language models

Aboli Marathe, Deva Ramanan, Rahee Walambe, Ketan Kotecha. CVPR 2023
Publisher: Carnegie Mellon University, Symbiosis International University
Dataset: WEDGE
Publish Date: 2023.05.12
Summary:
A multi-weather autonomous driving dataset built from generative vision-language models.
NuScenes-QA: A Multi-modal Visual Question Answering Benchmark for Autonomous Driving Scenario

Tianwen Qian, Jingjing Chen, Linhai Zhuo, Yang Jiao, Yu-Gang Jiang
Publisher: Fudan University
Dataset: NuScenes-QA
Summary:
NuScenes-QA provides 459,941 question-answer pairs based on the 34,149 visual scenes, with 376,604 questions from 28,130 scenes used for training, and 83,337 questions from 6,019 scenes used for testing, respectively.
The multi-view images and point clouds are first processed by the feature extraction backbone to obtain BEV features.
DRAMA: Joint Risk Localization and Captioning in Driving

Srikanth Malla, Chiho Choi, Isht Dwivedi, Joon Hee Choi, Jiachen Li
Publisher:
Datasets: DRAMA
Summary:
Introduce a novel dataset DRAMA that provides linguistic descriptions (with the focus on reasons) of driving risks associated with important objects and that can be used to evaluate a range of visual captioning capabilities in driving scenarios.
Language Prompt for Autonomous Driving

Datasets: Nuprompt(Not open)
Previous summary
Driving with LLMs: Fusing Object-Level Vector Modality for Explainable Autonomous Driving

Datasets: official, data collection using RL experts in simulator.
Previous summary
Textual Explanations for Self-Driving Vehicles

Jinkyu Kim, Anna Rohrbach, Trevor Darrell, John Canny, Zeynep Akata ECCV 2018.
Publisher: University of California, Berkeley, Saarland Informatics Campus, University of Amsterdam
BDD-X dataset
Grounding Human-To-Vehicle Advice for Self-Driving Vehicles

Jinkyu Kim, Teruhisa Misu, Yi-Ting Chen, Ashish Tawari, John Canny CVPR 2019
Publisher: UC Berkeley, Honda Research Institute USA, Inc.
HAD dataset
License
Awesome LLM for Autonomous Driving Resources is released under the Apache 2.0 license.

การเปิดตัว
ไม่มีการเผยแพร่ข่าวประชาสัมพันธ์
แพ็คเกจ
ไม่มีการเผยแพร่แพ็คเกจ
ผู้สนับสนุน
2
@jayyoung0802
jayyoung0802 เจิ้นเจี๋ยหยาง
@jiaxiaosong1002
jiaxiaosong1002 เซียวซง เจีย
ส่วนท้าย
© 2025 GitHub, Inc.
การนำทางส่วนท้าย
เงื่อนไข
ความเป็นส่วนตัว
ความปลอดภัย
สถานะ
ชุมชน
เอกสาร
ติดต่อ
จัดการคุกกี้
อย่าแบ่งปันข้อมูลส่วนตัวของฉัน
พบเจ้าของ 1 ราย
รายการที่อัปเดต รายการที่เน้น: ไม่มีใบอนุญาต เลือก 1 จาก 14
```
