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
```
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
```
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
```
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
xp-soaring.github.io  >  หน้าแรกรูปแบบไฟล์ igc  > ข้อมูลอ้างอิงและคู่มือ

คู่มืออ้างอิงรูปแบบไฟล์ IGC และผู้พัฒนา - Ian Forster-Lewis
บันทึกเหล่านี้สร้างขึ้นเพื่อการใช้งานส่วนตัวของผม เพื่อพยายามทำให้เอกสารประกอบของ FAI มีประโยชน์มากขึ้นสำหรับผมในฐานะนักพัฒนาโปรแกรมบันทึกข้อมูล สำหรับตัวอย่างไฟล์ IGC โดยละเอียด โปรดดูไฟล์ IGC จริงที่สร้างโดย LXNนี้

ลิงก์เว็บในFIAเปลี่ยนแปลงทุกครั้งที่มีการจ้างนักพัฒนาเว็บใหม่ ดังนั้นสำเนาของ FAI IGC Specification 2023 จึงถูกโฮสต์ไว้ที่นี่

เวอร์ชัน HTML ที่ลิงก์กับเว็บนี้มีไว้สำหรับ IGC spec 2008 แต่ไม่ได้เปลี่ยนแปลงมากนัก ฉันได้เก็บหมายเลขบท/หัวข้อของ FAI ไว้ แต่ได้เพิ่มเข้าไปในหัวข้อบางส่วนแล้ว

เนื้อหา
คำนำ: ตัวอย่างพร้อมคำอธิบาย
1. บทนำ
1.1 พื้นหลังและการผลิตไฟล์ IGC
1.2 การควบคุมการแก้ไข
2. ทั่วไป
2.1 โครงสร้างไฟล์
2.2 ประเภทของบันทึก
2.3 ลำดับการบันทึก
2.4 หน่วย
2.5 การตั้งชื่อไฟล์
3. บันทึกข้อมูลแบบอินสแตนซ์เดียว
3.1 บันทึก - หมายเลขประจำตัว FR
3.2 G record - ความปลอดภัย
3.3 บันทึก H - ส่วนหัวของไฟล์
3.4 ฉันบันทึก - การขยายการบันทึกการแก้ไข (B)
3.5 บันทึก J - ส่วนขยายไปยังบันทึก K
3.6 บันทึก C - งาน
4. บันทึกข้อมูลอินสแตนซ์หลายรายการ
4.1 บันทึก B - แก้ไข
4.2 บันทึก E - เหตุการณ์
4.3 F record - กลุ่มดาวเทียม
บันทึก 4.4 K - ข้อมูลที่ต้องการน้อยกว่าการแก้ไข
บันทึก 4.5 ลิตร - สมุดบันทึก / ความคิดเห็น
4.6 D record - GPS เชิงอนุพันธ์
5. คำจำกัดความ
6. อักขระที่ถูกต้อง
7. รหัสสามตัวอักษร (TLC)
8. ข้อมูลพิกัดทางภูมิศาสตร์ GNSS
9. ตัวอย่างไฟล์รูปแบบ IGC
คำนำ: ตัวอย่างพร้อมคำอธิบาย
นี่คือ "ตัวอย่างการใช้งาน" ของไฟล์ IGC ที่ถูกต้อง ซึ่งไม่มีอยู่ในเอกสารต้นฉบับของ FAI มีการใส่อักขระ "ช่องว่าง" ไว้เพื่อให้อ่านง่าย หากต้องการคัดลอกและวางไฟล์นี้เป็นจุดเริ่มต้นสำหรับการพัฒนา คุณสามารถใช้ไฟล์เวอร์ชันเดียวกันในส่วนที่ 9โดยไม่ต้องใส่ช่องว่าง ข้อความอิสระเป็นตัวเอียง หมายความว่าคุณสามารถป้อนอะไรก็ได้ มิฉะนั้นจำนวนอักขระที่แน่นอนจะต้องตรงกับตัวอย่าง แต่ละ "เรคคอร์ด" ในไฟล์ IGC จะอยู่ในบรรทัดเดียว และอักขระสองสามตัวแรกจะเป็นตัวกำหนดประเภท ของเรคคอร์ด ฉันได้ลิงก์อักขระเริ่มต้นในตัวอย่างด้านล่างไปยังส่วนที่เกี่ยวข้องในข้อกำหนด

เที่ยวบิน XXX  ABC  :1	รหัสผู้ผลิตใช้ XXX หากคุณไม่มี ABC คือรหัสเฉพาะของเครื่องบันทึกนี้ (หมายเลขซีเรียล?) ส่วนที่เหลือของบรรทัดสามารถเป็นอะไรก็ได้ตามต้องการ
HFFXA  035	ความแม่นยำในการแก้ไขโดยทั่วไปคือ 35 เมตร นอกจากนี้ยังสามารถเพิ่มฟิลด์ FXA ให้กับบันทึก B แต่ละรายการได้อีกด้วย
HFDTE  160701	วันที่บินตามเวลา UTC ที่นี่คือวันที่ 16 กรกฎาคม พ.ศ. 2544
HFPLT  PILOTINCHARGE:  บล็อกส์ บิล ดี	ชื่อข้อความอิสระของนักบิน
HFCM2  CREW2:  สมิธ-แบร์รี่ จอห์น เอ	ชื่อข้อความอิสระของนักบินคนที่สองในเครื่องบินสองที่นั่ง
HFGTY  GLIDERTYPE:  Schleicher ASH-25	ประเภทเครื่องร่อนแบบข้อความอิสระ
HFGID  GLIDERID:  N116 EL	หมายเลขหรือรหัสทะเบียนเครื่องบินแบบข้อความอิสระ เช่น หมายเลข N ในสหรัฐอเมริกา หรือหมายเลขบนครีบ - ไม่สำคัญจริงๆ
HFDTM 100 GPSDATUM: WGS-1984	ตัวบันทึกใช้ข้อมูล GPS ใด จากประสบการณ์ของผม 100 เสมอ แต่ดู เอกสารต้นฉบับของ FAI หากคุณต้องการทำอะไรที่แปลกใหม่
เวอร์ชันเฟิร์มแวร์ HFRFW  : 6.4	เวอร์ชันเฟิร์มแวร์ (เช่น ซอฟต์แวร์) ของตัวบันทึก - อะไรก็ได้ที่คุณต้องการ
เวอร์ชันฮาร์ดแวร์ HFRHW  : 3.0	เวอร์ชันฮาร์ดแวร์ของตัวบันทึก - ข้อความใด ๆ ที่เหมาะสม
HFFTY  FRTYPE:  Calibri, FunkyLogger 77	ประเภทบันทึกเที่ยวบิน - ข้อความใดๆ ก็ได้
HFGPS  มาร์โคนี ซุปเปอร์สตาร์ 12 ช่อง 10,000 เมตร	ผู้ผลิตเครื่องรับ GPS ภายในเครื่องบันทึกข้อมูล เราสนใจจริงหรือ? ข้อความใดๆ ก็ใช้ได้
HFPRS  PRESSALTSENSOR:  Sensyn,XYZ11,11000m	ผู้ผลิตเซ็นเซอร์วัดแรงดันในเครื่องบันทึกข้อมูล ข้อความใดๆ
HFCID  COMPETITIONID:  B21	หมายเลขครีบหางของเครื่องร่อน ซอฟต์แวร์วิเคราะห์บันทึกการบิน IGC (เช่น SeeYou) มักจะใช้ค่านี้เพื่อติดป้ายกำกับบันทึกที่คุณอัปโหลด ซึ่งมีประโยชน์เมื่อสร้างภาพเคลื่อนไหวบันทึกหลายรายการ ข้อความอิสระแต่ควรเขียนให้สั้น
HFCCL  COMPETITIONCLASS: เครื่องร่อนมอเตอร์ 15 เมตร	ข้อความอิสระที่อธิบายคลาสเครื่องร่อน เช่น มาตรฐาน 15 เมตร แต่ไม่มีมาตรฐานสำหรับค่าต่างๆ
ฉัน  03 36 38  FXA  39 40  SIU  41 43  ENL	(ตั้งแต่ปี 2009 เป็นต้นมา มีเพียงส่วนขยาย FXA เท่านั้นที่ 'บังคับ') นี่คือเรกคอร์ดส่วนหัว 'ส่วนขยาย' ซึ่งอธิบาย ฟิลด์ เพิ่มเติมที่สามารถผนวกเข้ากับเรกคอร์ด B ทุก เรกคอร์ด เรกคอร์ด B คือข้อมูล 'แก้ไข' ไทม์ซีรีส์พื้นฐานที่โปรแกรมวิเคราะห์เกือบทั้งหมดใช้ (คุณคงแปลกใจว่าข้อมูล 'H' พวกนี้ทิ้งไปเยอะมากขนาดไหน...) ดังนั้นเรกคอร์ด I จึง สามารถรวมระดับเสียงเครื่องยนต์เข้ากับจุดแก้ไขทุกจุดได้ ตัวอย่างนี้ระบุว่าระดับเสียงเครื่องยนต์ ( ENL ) จะถูกเพิ่มเป็นไบต์ 41 ถึง 43 ให้กับเรกคอร์ด B แต่ละเรกคอร์ด เช่นเดียวกับ FXA และ SIU ตัวเลข "03" หลัง "I" คือจำนวนส่วนขยายที่กำหนด นั่นคือสาม
เจ  01 08 12  เอชดีที	(ไม่บังคับ) เนื่องจากระเบียน Iข้างต้นขยายระเบียน B ระเบียนJจึงขยาย ระเบียน K ระเบียน Kโดยพื้นฐานแล้วระเบียน K คือ "ค่าประทับเวลา K" ซึ่งค่าทั้งหมดถูกกำหนดโดยระเบียน J นี้ และสามารถฝังระเบียน K ไว้ที่ใดก็ได้ระหว่างระเบียน B โดยถือว่าระเบียนเหล่านี้ใช้สำหรับการอัปเดตที่น้อยกว่าระเบียน B ที่มีความถี่สูง ตัวอย่างนี้แสดง Heading True ( HDT ) ซึ่งเป็นข้อมูลที่ถูกใส่ลงในบันทึกโดยใช้ระเบียน K
C  150701 213841 160701 0001 02  500K ไตร	(ทางเลือก) (ตัวอย่างบันทึก C (คำประกาศ) ต่อไปนี้ใช้สำหรับการบินรูปสามเหลี่ยมระยะทาง 500 กม. จากศูนย์ร่อน Lasham ในสหราชอาณาจักร)
บรรทัดแรกนี้ประกอบด้วยวันที่/เวลาของคำประกาศ (15 ก.ค. 2544) 21:38 น. (21:38 น.) และ 14 วินาที วันที่ของเที่ยวบินที่ต้องการ (16 ก.ค. 2544) รหัสภารกิจสี่หลัก (0001) จำนวนจุดเปลี่ยน (02) โดยไม่รวมจุดเริ่มต้น/สิ้นสุด และข้อความอิสระที่อธิบายภารกิจ
C  5111359N 00101899W  ลาแชมคลับเฮาส์	ละติจูด C เป็น DDMMmmmN ลองจิจูดเป็น DDDMMmmmE คำอธิบาย
C  5110179N 00102644W  Lasham สตาร์ท S, สตาร์ท	 
C  5209092N 00255227W  ซาร์เนสฟิลด์, TP1	 
C  5230147N 00017612W  นอร์แมน ครอส, TP2	 
C  5110179N 00102644W  Lasham สตาร์ท S, จบ	บันทึก C มีรูปแบบเดียวกับบันทึกอื่นๆ ข้างต้น แต่นี่คือจุดขึ้นบินและไม่ได้เป็นส่วนหนึ่งของการประกาศภารกิจอย่างเป็นทางการ โดยทั่วไปจะระบุตำแหน่งของสนามบินต้นทางเท่านั้น
C  5111359N 00101899W  ลาแชมคลับเฮาส์	บันทึก C เหมือนกับข้างต้น คราวนี้สำหรับ สถาน ที่ลงจอดอีกครั้ง ไม่ได้เป็นส่วนหนึ่งของการประกาศภารกิจอย่างเป็นทางการ และโดยทั่วไปจะเป็นสนามบินบ้าน
ฟ. 160240 04 06 09 12 36 24 22 18 21	วิธีนี้จะแสดง ID ของดาวเทียมที่มองเห็นได้ในรูปแบบ "F-timestamp-ID-ID-ID..." โดยที่ timestamp คือ HHMMSS และแต่ละ ID คือคู่ขนาดสองไบต์ ในตัวอย่างนี้ เวลา 16:02:40 น. เครื่องบันทึกข้อมูลสามารถเห็นดาวเทียมได้เก้าดวง
B 160240 5407121N 00249342W A 00280 00421 205 09 950	เยี่ยมเลย ในที่สุดเราก็มาถึงจุดบันทึกที่เราสนใจแล้ว รูปแบบคือ "B-timestamp-latitude-longitude-AVflag-pressure alt-GPS alt-extensions" ดังที่ได้กล่าวไปแล้ว 35 ไบต์แรกของบันทึก B มีนิยามที่ตายตัว จากนั้นฟิลด์จะถูกกำหนดโดย บันทึก Iบันทึก B นี้มีเวลาประทับ16:02:40 , ละติจูด54 องศา 7.121 นาทีเหนือ , ลองจิจูด 2 องศา 49.342 นาทีตะวันตก , AVflag (ความถูกต้อง 3 มิติ) A , ความสูง 280 เมตรจากเซ็นเซอร์ความดัน, ความสูง 421 เมตรจาก GPS, และFXA (ความแม่นยำ) 205 เมตร, SIU (จำนวนดาวเทียม) 09 และ ENL (เสียงเครื่องยนต์) 950 (แสดงว่าเครื่องยนต์กำลังทำงาน...)
ด.  20331	(ทางเลือก) นี้จะให้ ID ของสถานี "GPS เชิงอนุพันธ์" ที่กำลังใช้งานอยู่ รูปแบบ "D2xxxx" โดยที่ xxxx คือ ID
อี 160245 พีอีวี	(ไม่บังคับ) บันทึกนี้จะบันทึกเหตุการณ์ในรูปแบบ "timestamp-code" โดยใช้รหัส 3 ตัวอักษรที่อนุญาตตามที่กำหนดไว้ในส่วนที่ 7ในตัวอย่างนี้ รหัสนี้เป็น "Pilot Event" ทั่วไป ซึ่งโดยทั่วไปจะใช้เพื่อทำให้โปรแกรมบันทึกข้อมูลเร่งอัตราการบันทึกข้อมูลชั่วคราว บันทึก Eต้องตามด้วยบันทึก B ที่ระบุตำแหน่ง
B 160245 5107126N 00149300W A 00288 00429 195 09 020	บันทึก Bนี้ตรงกับบันทึก E ด้านบนกล่าวคือ มีไทม์สแตมป์เดียวกัน ผู้ที่ตาไวจะสังเกตเห็นว่าระดับเสียงเครื่องยนต์ลดลงจาก 950 ในบันทึก B ก่อนหน้าเป็น 020 ซึ่งหมายความว่าเครื่องยนต์ดับภายใน 5 วินาทีหลังจากการแก้ไขเหล่านี้
B 160250 5107134N 00149283W A 00290 00432 210 09 015	บันทึกต่อเป็นช่วงเวลา 5 วินาที (ช่วงเวลาใดก็ได้)
บี 160255 5107140N 00149221W เอ 00290 00430 200 09 012	ยังคงบันทึกเป็นช่วงเวลา 5 วินาที... โดยปกติไฟล์จะประกอบด้วยบันทึกเหล่านี้เกือบทั้งหมด
ฟ. 160300 06 09 12 36 24 22 18 21	ดาวเทียมที่ใช้งานลดลงจาก 9 เหลือ 8 ดวง เนื่องจากไม่สามารถรับสัญญาณ ID 04 ได้อีกต่อไป
บี 160300 5107150N 00149202W เอ 00291 00432 256 08 009	นี่คือบันทึกการแก้ไข (B) ที่ให้ตำแหน่งสำหรับบันทึก F ด้านบน
E 160305  พีอีวี	"เหตุการณ์นำร่อง" เช่น เขา/เธอกดปุ่มเพื่อเพิ่มอัตราการบันทึกข้อมูล
บี 160305 5107180N 00149185W เอ 00291 00435 210 08 015	บันทึกการแก้ไขที่ให้ละติจูด/ลองจิจูดของเหตุการณ์ PEV ด้านบน
B 160310 5107212N 00149174W A 00293 00435 196 08 024	การแก้ไขอีกครั้ง
เค  160248 00090	เรกคอร์ด Kนี้เป็นตัวแทนสำหรับค่าคาบทั่วไปที่เลือกจากรายการ ซึ่งสามารถกำหนดได้ในเรกคอร์ด J เดี่ยว ในส่วนหัว ในตัวอย่างนี้ เรกคอร์ด J ที่ด้านบนของไฟล์ตัวบันทึกนี้ระบุว่าไบต์ 8 ถึง 12 จะเป็น True Heading ( ) ในที่นี้ ค่าของ True Heading ที่เวลา 16:02:48 คือ 90 องศา ( AL7 )
บี 160248 5107220N 00149150W เอ 00494 00436 190 08 018	นี่คือบันทึกการแก้ไข (B) ที่ให้ตำแหน่งสำหรับบันทึก K ด้านบน (โปรดทราบว่ามีการประทับเวลาเดียวกัน)
B 160252 5107330N 00149127W A 00496 00439 195 08 015	บันทึกการแก้ไขทั่วไปอีกอัน
L  XXX  มาตรฐานแห่งชาติของยูริทาเนีย วันที่ 1	นี่คือบันทึก 'ความคิดเห็น' ทั่วไป อักขระสามตัวหลัง 'L' อาจเป็นรหัสผู้ผลิต (XXX ในตัวอย่างนี้), 'PLT' (ความคิดเห็นของนักบิน), 'OOI' (ความคิดเห็นของผู้สังเกตการณ์) หรือ 'PFC' (ความคิดเห็นหลังการบิน) หลังจากนั้น สามารถใช้ข้อความอิสระใดๆ ก็ได้
L  XXX เวลาบิน: 4:14:25, ความเร็วภารกิจ: 58.48KT	บันทึกความคิดเห็นอีกรายการหนึ่ง
จี รี  เจงเจอร์JKNJKRE31895478537H43982FJN9248F942389T433T	รหัสความปลอดภัยที่คำนวณโดยโปรแกรมบันทึกข้อมูลจากเนื้อหาด้านบน ประเด็นเดียวคือควรมีโปรแกรมแยกต่างหากสำหรับตรวจสอบรหัสนี้ เพื่อให้คุณมั่นใจได้ว่าไฟล์บันทึกนั้นถูกต้อง...
G  JNJK2489IERGNV3089IVJE9GO398535J3894N358954983O0934	อนุญาตให้ บันทึก Gหลายรายการไม่ว่าซอฟต์แวร์บันทึกจะต้องการอะไรก็ตาม
จี  SKTO5427FGTNUT5621WKTC6714FT8957FGMKJ134527FGTR6751	 
G  K2489IERGNV3089IVJE39GO398535J3894N358954983FTGY546	 
G  12560DJUWT28719GTAOL5628FGWNIST78154INWTOLP7815FITN	 
1. บทนำ
1.1 ความเป็นมาและการสร้างไฟล์ IGCมาตรฐานไฟล์ข้อมูล IGC ได้รับการพัฒนาขึ้นในขั้นต้นโดยกลุ่มตัวแทนจาก IGC ผู้ผลิตเครื่องร่อน FR และนักพัฒนาซอฟต์แวร์อิสระหลายราย ซึ่งส่วนใหญ่เกี่ยวข้องกับโปรแกรมวิเคราะห์ข้อมูลการบิน หลังจากการหารือและพัฒนาระหว่างปี พ.ศ. 2536 และ พ.ศ. 2537 มาตรฐานนี้ได้รับการกำหนดขึ้นในเดือนธันวาคม พ.ศ. 2537 และกลายเป็นส่วนหนึ่งของเอกสารอย่างเป็นทางการของ IGC/FAI หลังจากได้รับอนุมัติจาก IGC ในเดือนมีนาคม พ.ศ. 2538 ต่อมาได้รับการปรับปรุงและพัฒนาอย่างต่อเนื่อง มาตรฐานนี้ให้รูปแบบข้อมูลมาตรฐานสากลสำหรับการตรวจสอบป้าย สถิติ และเที่ยวบินแข่งขันตามมาตรฐาน FAI/IGC มาตรฐานนี้ยังสามารถใช้ในกีฬาและกิจกรรมอื่นๆ ของ FAI ได้อีกด้วย

1.1.1การจัดทำไฟล์ข้อมูลการบิน ต้องสามารถจัดทำไฟล์ข้อมูลการบิน IGC แยกต่างหากและสมบูรณ์สำหรับแต่ละเที่ยวบิน ซึ่งรวมถึงบันทึกทุกประเภท ( ดูข้อ 2.2ต่อไปนี้) ที่เกี่ยวข้องกับเที่ยวบินนั้น เช่น บันทึกส่วนหัว การประกาศเที่ยวบิน ฯลฯ มีสองวิธีในการทำเช่นนี้ คือ การบันทึกการแก้ไขอย่างต่อเนื่องระหว่างเวลาที่เปิดและปิด FR หรือสำหรับ FR ที่อยู่ในสถานะ "สแตนด์บาย" เมื่อเปิดเครื่อง ให้บันทึกเฉพาะการแก้ไขหลังจากเกินเกณฑ์การเคลื่อนที่และการเปลี่ยนแปลงความดันที่ตั้งไว้ล่วงหน้า (หยุดการบันทึกเมื่อการเปลี่ยนแปลงต่ำกว่าเกณฑ์ แต่ดูข้อ 1.1.1.2ในช่วงเวลาสั้นๆ ที่ไม่มีแหล่งจ่ายไฟภายนอก) ( AL3 )

1.1.1.1 เกณฑ์สำหรับการเริ่มต้นและหยุดการบันทึก รวมถึงโปรโตคอลการเปิดเครื่องสำหรับการสร้างไฟล์ IGC ใหม่ เกณฑ์ต่อไปนี้ก่อนการบันทึกการแก้ไขเคยพบว่าเหมาะสมในอดีต: การเปลี่ยนแปลงละติจูด/ลองจิจูด 10-15 กม./ชม. การเปลี่ยนแปลงระดับความสูงของความกดอากาศ 1 เมตรต่อวินาที เป็นเวลา 5 วินาที ต้องมีเส้นฐานก่อนขึ้นบินและหลังลงจอดอย่างน้อย 20 จุด สำหรับเส้นฐานก่อนขึ้นบิน สามารถใช้วงจรหน่วยความจำขนาดเล็กที่จัดเก็บจุดแก้ไขก่อนหน้าในจำนวนที่เหมาะสมอย่างต่อเนื่อง และเมื่อตรวจพบการเคลื่อนไหว จุดแก้ไขเหล่านั้นจะถูกบันทึกลงในบันทึกข้อมูลการบิน หลังจากลงจอด สามารถทำได้โดยการหน่วงเวลาก่อนที่จะหยุดการบันทึกจุดแก้ไข เงื่อนไขนี้อาจใช้กับช่วงเวลาที่คลื่นหรือสันเขายกตัวขึ้นเล็กน้อยหรือไม่มีการเคลื่อนไหวในแนวตั้งหรือแนวนอน ดังนั้น ไม่ควรเริ่มต้นไฟล์ IGC ใหม่ในขณะที่ยังมีแหล่งจ่ายไฟภายนอกอยู่และเครื่องบันทึกยังคงเปิดอยู่ แม้ว่าจะไม่ตรวจพบการเคลื่อนไหวใดๆ และไม่มีการบันทึกจุดแก้ไขก็ตาม โปรดทราบว่า "โปรโตคอลการเปิดเครื่อง" นี้จำเป็นสำหรับการสอบเทียบบารอกราฟด้วย เพื่อไม่ให้เกิดการสร้างไฟล์ใหม่ในขณะที่เครื่องสอบเทียบกำลังปรับความดันเล็กน้อยในแต่ละระดับของการสอบเทียบ ไฟล์ IGC ใหม่จะถูกสร้างขึ้นภายใต้ "โปรโตคอลการปิดเครื่อง" ซึ่งอธิบายไว้ในข้อ1.1.1.2ด้านล่าง ( AL5 ) ซึ่งแก้ไขโดย ( AL9 )

1.1.1.2 การสูญเสียพลังงานภายนอกเป็นระยะเวลาสั้นๆ - โปรโตคอลปิดเครื่องสำหรับการสร้างไฟล์ IGC ใหม่ เพื่อให้สามารถดำเนินการต่างๆ เช่น การเปลี่ยนหรือสลับแบตเตอรี่ระหว่างการบินได้ จะต้องปล่อยให้เวลาผ่านไป 5 นาทีโดยไม่มีพลังงานภายนอก ก่อนที่จะสร้างไฟล์ข้อมูลการบินใหม่เมื่อเปิดเครื่องอีกครั้ง หลังจากเวลานี้ผ่านไปแล้ว จะต้องสร้างไฟล์ IGC ใหม่ เพื่อให้หากมีการบินหลายเที่ยวบินในหนึ่งวัน แต่ละเที่ยวบินจะมีไฟล์ข้อมูล IGC ที่สมบูรณ์เป็นของตัวเอง ( AL3 )

1.1.1.3 การถ่ายโอนข้อมูลไปยังคอมพิวเตอร์ส่วนบุคคล หากข้อมูลของเที่ยวบินหลายเที่ยวบินถูกเก็บไว้ในหน่วยความจำ FR จะต้องตรวจสอบให้แน่ใจว่าเมื่อถ่ายโอนข้อมูล ประเภทบันทึกทั้งหมดในไฟล์ IGC ที่อยู่ถัดจากไฟล์แรกจะต้องเป็นประเภทบันทึกที่เกี่ยวข้องกับเที่ยวบินแต่ละเที่ยวบินถัดไป หากมีการเปลี่ยนแปลงประเภทบันทึกใดๆ ระหว่างเที่ยวบิน (เช่น การประกาศ ชื่อนักบิน ฯลฯ) การเปลี่ยนแปลงจะต้องรวมอยู่ในไฟล์ข้อมูลเที่ยวบินถัดไป (แต่ไม่ใช่ไฟล์ก่อนหน้า) ( AL3 )

1.1.1.4 เครื่องบันทึกข้อมูลทำงานโดยใช้พลังงานภายใน เครื่องบันทึกข้อมูลบางเครื่องได้รับการออกแบบให้ฟังก์ชันทั้งหมดทำงานโดยใช้พลังงานภายใน สำหรับเครื่องบันทึกข้อมูลเหล่านี้ ใช้พลังงานภายนอกเพื่อชาร์จไฟและใช้เป็นพลังงานสำรองสำหรับเที่ยวบินระยะไกล เมื่อใช้งานโดยใช้พลังงานภายใน ต้องมั่นใจว่าภายใต้สภาวะการบินที่มีการเคลื่อนไหวในแนวนอนหรือแนวตั้งเพียงเล็กน้อย (เช่น การบินแบบสันเขาหรือแบบคลื่น) ไฟล์ IGC จะยังคงสามารถบันทึกข้อมูลได้ และจะไม่หยุดทำงานในขณะที่เที่ยวบินยังคงดำเนินต่อไป ไฟล์ IGC ควรหยุดทำงานหลังจากหนึ่งในสามเงื่อนไขต่อไปนี้: (1) หากไม่พบการเคลื่อนไหวในแนวนอนหรือแนวตั้งเป็นเวลา 10 นาที (เกณฑ์ตามข้อ1.1.1.1ข้างต้น); (2) หลังจากเครื่องบันทึกข้อมูลถูกปิดโดยการกระทำโดยเจตนา หรือ; (3) หากเครื่องบันทึกข้อมูลยังคงมีพลังงานอยู่หลังจากการบินเสร็จสิ้น เมื่อผู้ใช้เชื่อมต่อเพื่อดาวน์โหลดข้อมูลจากเครื่องบันทึกข้อมูล ( AL10 )

1.2 การควบคุมการแก้ไข รูปแบบไฟล์ข้อมูลการบินของ IGC ได้รับการแก้ไขตามกระบวนการแก้ไขปกติสำหรับเอกสารนี้ ดูขั้นตอนการแก้ไขและรายการการแก้ไขในหน้า (i)

2. ทั่วไป
2.1 โครงสร้างไฟล์ ไฟล์รูปแบบ IGC ประกอบด้วยบรรทัดอักขระ โดยแต่ละบรรทัดจะแสดงชุดข้อมูล เช่น ข้อมูลสำหรับการแก้ไข GNSS แต่ละบรรทัดจะขึ้นต้นด้วยอักษรตัวพิมพ์ใหญ่ซึ่งแสดงถึงประเภท Record หนึ่งประเภทที่ระบุไว้ในข้อ 2.2 และลงท้ายด้วย CRLF (Carriage Return Line Feed) แต่ละบรรทัดมีความยาวไม่เกิน 76 อักขระ ไม่รวม CRLF ที่ถูกซ่อนไว้และไม่ปรากฏในรูปแบบข้อความ บางประเภท Record ใช้พื้นที่เพียงบรรทัดเดียว บางประเภท เช่น task และ header ใช้พื้นที่หลายบรรทัด ตัวอย่างเช่น task/declaration (C) Record ประกอบด้วยบรรทัดสำหรับแต่ละจุดอ้างอิง และ Header (H) Record ประกอบด้วยบรรทัดแยกต่างหากสำหรับประเภท GNSS FR ชื่อนักบิน การระบุเครื่องร่อน ฯลฯ ลำดับของประเภท Record ภายในไฟล์ IGC จะแสดงอยู่ในข้อ 2.3 บางประเภท Record จะปรากฏในตำแหน่งเดียวในไฟล์ (Record อินสแตนซ์เดียว) ในขณะที่บางประเภท เช่น fixes จะเกิดขึ้นซ้ำเมื่อเวลาผ่านไป (Record อินสแตนซ์หลายรายการ) ให้ใช้เฉพาะอักขระที่ระบุว่าถูกต้องตามวรรค 6 ในไฟล์เท่านั้น หากใช้อักขระอื่นๆ เช่น อักขระเน้นเสียง (เช่น เครื่องหมายอะคิวต์, แฮทช์, อัมเลาต์ ฯลฯ) ในชื่อสนามบินและจุดเลี้ยว ในรูปแบบไฟล์ที่เป็นกรรมสิทธิ์ของผู้ผลิต (ต้นฉบับ) อักขระดังกล่าวจะต้องถูกแปลงเป็นอักขระที่ถูกต้อง ซึ่งเป็นส่วนหนึ่งของการแปลงเป็นรูปแบบ IGC เพื่อให้โปรแกรมวิเคราะห์ที่ออกแบบมาสำหรับรูปแบบ IGC ไม่จำเป็นต้องจดจำอักขระที่ไม่เป็นมาตรฐาน

2.2 ประเภทระเบียน ระเบียนแต่ละประเภทจะขึ้นต้นด้วยอักษรตัวพิมพ์ใหญ่ ดังนี้

รูปแบบไฟล์ข้อมูล IGC - ตัวอักษรระบุประเภทบันทึก
ผู้ผลิตและการระบุ A - FR
บี-ฟิกซ์
C - งาน/การประกาศ
D - GPS เชิงอนุพันธ์
อี - อีเว้นท์
F - กลุ่มดาว
G - ความปลอดภัย
H - ส่วนหัวของไฟล์
I - รายการข้อมูลส่วนขยายที่รวมอยู่ตอนท้ายของแต่ละรายการแก้ไขB บันทึก
J - รายการข้อมูลที่รวมอยู่ในส่วนขยายแต่ละส่วน (K) บันทึก
K - ข้อมูลส่วนขยาย
L - สมุดบันทึก/ความคิดเห็น
M, N, ฯลฯ - อะไหล่
2.3 ลำดับการบันทึก ระเบียน FR ​​I/D (A) จะอยู่ลำดับแรกในไฟล์เสมอ และระเบียนสุดท้ายคือระเบียน Security (G) ระเบียนA บรรทัดเดียว จะเป็นระเบียน Header (H) หลายบรรทัด ตามด้วยระเบียน I และ J ซึ่งแสดงรายการข้อมูลส่วนขยายที่นำไปใช้กับระเบียนประเภทอื่นๆ ในไฟล์ ระเบียนเหล่านี้ตามด้วยระเบียนประเภทอื่นๆ ที่ระบุว่าข้อมูลบางอย่างถูกบันทึกลงในไฟล์ รวมถึงระเบียน task/declaration (C) และกลุ่มดาวเทียมเริ่มต้น (F) ตามด้วยระเบียนเฉพาะเวลา ซึ่งจัดวางในไฟล์ตามลำดับเวลาโดยใช้ GNSS fix-time (หาก GNSS ถูกล็อกไว้) หรือ FR Real Time Clock (RTC) ได้แก่ B (fix), E (event), F (constellation change) และ K (extensions data) ข้อมูลบันทึกสมุดบันทึก/ความคิดเห็น (L) สามารถวางไว้ที่ใดก็ได้หลังระเบียน H, I และ Jและสามารถมีได้หลายบรรทัดตลอดทั้งไฟล์ ขึ้นอยู่กับลักษณะของความคิดเห็นที่ใส่ไว้

ลำดับของประเภทบันทึกต่อไปนี้เป็นลำดับทั่วไป แม้ว่าในไฟล์ข้อมูลการบินจริงจะมี เส้น บันทึก B คง ที่มากกว่าที่แสดงที่นี่มากก็ตาม:
รูปแบบไฟล์ข้อมูล IGC - ลำดับประเภทบันทึกในไฟล์ IGC
A - ผู้ผลิต FR และการระบุตัวตน (ก่อนเสมอ)
H - ส่วนหัวของไฟล์
I - แก้ไขรายการส่วนขยายของข้อมูลที่เพิ่มในตอนท้ายของแต่ละ B
บันทึก
J - รายการส่วนขยายของข้อมูลในแต่ละบรรทัดบันทึก K
C - งาน/ประกาศ (ถ้าใช้)
L - สมุดบันทึก/ความคิดเห็น (ถ้ามีการใช้)
D - GPS เชิงอนุพันธ์ (ถ้าใช้)
F - กลุ่มดาวเทียมเริ่มต้น
B - แก้ไขข้อมูลส่วนขยายใดๆ ที่ระบุไว้ในบันทึก I 
B - แก้ไขข้อมูลส่วนขยายใดๆ ที่ระบุไว้ในบันทึก I
อี - เหตุการณ์นำร่อง (PEV)
B - แก้ไขข้อมูลส่วนขยายใดๆ ที่ระบุไว้ในบันทึก I
K - ข้อมูลส่วนขยายตามที่กำหนดไว้ในบันทึก J
B - แก้ไขข้อมูลส่วนขยายใดๆ ที่ระบุไว้ในบันทึก I 
B - แก้ไขข้อมูลส่วนขยายใดๆ ที่ระบุไว้ในบันทึก I
F - การเปลี่ยนแปลงกลุ่มดาว
B - แก้ไขข้อมูลส่วนขยายใดๆ ที่ระบุไว้ในบันทึก I 
K - ข้อมูลส่วนขยายตามที่กำหนดไว้ในบันทึก J 
B - แก้ไขข้อมูลส่วนขยายใดๆ ที่ระบุไว้ในบันทึก I
อี - เหตุการณ์นำร่อง (PEV)
B - แก้ไขข้อมูลส่วนขยายใดๆ ที่ระบุไว้ในเรคคอร์ด I 
B - แก้ไขข้อมูลส่วนขยายใดๆ ที่ระบุไว้ในเรคคอร์ด I 
B - แก้ไขข้อมูลส่วนขยายใดๆ ที่ระบุไว้ในเรคคอร์ด I 
K - ข้อมูลส่วนขยายตามที่กำหนดไว้ในเรคคอร์ด J
L - สมุดบันทึก/ความคิดเห็น (ถ้ามีการใช้)
G - บันทึกความปลอดภัย (เสมอท้ายสุด)
2.4 หน่วย

ข้อมูลในไฟล์ IGC จะต้องใช้งานระบบหน่วยดังต่อไปนี้:

เวลา - UTC ได้จากแพ็กเกจข้อมูล GNSS เดียวกันกับที่ใช้บันทึกค่าละติจูด/ลองจิจูดและระดับความสูงของ GPS หรือหากไม่ได้ล็อก GPS ไว้ ก็จะใช้ข้อมูลจากนาฬิกาเวลาจริงในเครื่องบันทึก โปรดทราบว่า UTC ไม่เหมือนกับเวลาภายในระบบ GPS ซึ่งแตกต่างกัน 14 วินาทีในปี พ.ศ. 2549 เนื่องจากมีการเพิ่ม "วินาทีอธิกสุรทิน" นับตั้งแต่ระบบ GPS เริ่มใช้งานครั้งแรกในเดือนมกราคม พ.ศ. 2523 การแก้ไข UTC ที่มีอยู่ในระบบ GPS จะต้องนำไปใช้กับเวลาที่บันทึกในไฟล์ IGC ( AL9 )
ระยะทาง - กิโลเมตรและกิโลเมตรทศนิยม สำหรับการแปลงหน่วย FAI/IGC จากฟุตและไมล์ โปรดดูย่อหน้า 2.6.8
( AL6 )
ความเร็ว - กิโลเมตรต่อชั่วโมง สำหรับการแปลงหน่วย FAI/IGC จากไมล์ทะเลต่อชั่วโมง (นอต) และไมล์ตามกฎหมาย
ต่อชั่วโมง (ไมล์ต่อชั่วโมง) ดูวรรค2.6.8 ( AL6 )
วันที่ (ของบรรทัดแรกในระเบียน B ) - UTC DDMMYY (วัน เดือน ปี) ดูย่อหน้า2.5.4 ( AL6 )
ทิศทาง - องศา จริง ตามเข็มนาฬิกาจาก 000 (ทิศเหนือ)
ละติจูดและลองจิจูด - องศา นาที และนาทีทศนิยมพร้อมตัวกำหนด N, S, E, W
ระดับความสูง - เมตร บันทึกแยกสำหรับ GNSS และระดับความสูงของแรงดัน
ความดัน - เฮกโตปาสกาล (เช่นเดียวกับมิลลิบาร์) ถึงสองตำแหน่งทศนิยม เช่น การตั้งค่ามาตราส่วนย่อยของเครื่องวัดความสูง แต่
ดู * ด้านล่างภายใต้ PPPPpp
รายการข้างต้นจะต้องบันทึกไว้ในบันทึกการบินดังนี้:
เวลา - HHMMSSsss (UTC)
HH - ชั่วโมงที่ถูกกำหนดเป็น 2 หลักโดยมี 0 นำหน้าเมื่อจำเป็น
MM - นาทีที่ถูกกำหนดเป็น 2 หลักโดยมี 0 นำหน้าเมื่อจำเป็น
SS - วินาทีที่ถูกกำหนดเป็น 2 หลักโดยมี 0 นำหน้าเมื่อจำเป็น
sss - จำนวนวินาทีทศนิยมคือจำนวนที่มีอยู่ในบันทึกที่เกี่ยวข้อง ลบด้วยฟิลด์ที่ใช้สำหรับ HHMMSS ไปแล้ว ( AL8 )
ระยะทาง - DDDDddddกิโลเมตร สูงสุด 9999 พร้อมศูนย์นำหน้าตามต้องการ และทศนิยมสามตำแหน่ง (นั่นคือตัวเลขสุดท้ายเป็นเมตร)
ความเร็ว - SSSsss
SSS - กำหนดเป็น 3 หลักโดยมี 0 นำหน้า
sss - จำนวนทศนิยมความเร็ว (จำนวนฟิลด์ที่บันทึกคือฟิลด์ที่ใช้สำหรับความเร็วในเรคคอร์ดที่เกี่ยวข้อง ลบฟิลด์ที่ใช้สำหรับ SSS ไปแล้ว)
วันที่ - วว/ดด/
ปป วว - เลขที่วันในเดือน กำหนดเป็น 2 หลัก มี 0 นำหน้าเมื่อจำเป็น
ดม - เลขที่เดือนในปี กำหนดเป็น 2 หลัก มี 0 นำหน้าเมื่อจำเป็น
YY - เลขที่ปี โมดูโล 100 กำหนดเป็น 2 หลัก มี 0 นำหน้าเมื่อจำเป็น
ทิศทาง DDDddd.
DDD - กำหนดเป็น 3 หลัก โดยมี 0 นำหน้าเมื่อจำเป็น
ddd - จำนวนทศนิยมทิศทาง (จำนวนฟิลด์ที่บันทึกคือฟิลด์ที่พร้อมใช้งานสำหรับทิศทางในบันทึกที่เกี่ยวข้อง ลบฟิลด์ที่ใช้สำหรับ DDD ไปแล้ว)
ละติจูด/ลองจิจูด - DDM มม. มม. NDDDMM มม. E
DD- องศาละติจูดโดยมี 0 นำหน้าเมื่อจำเป็น
DDD - องศาลองจิจูดโดยมี 0 หรือ 00 นำหน้าเมื่อจำเป็น
MMmmmNSEW - นาทีละติจูด/ลองจิจูดโดยมี 0 นำหน้าเมื่อจำเป็น 3 ตำแหน่งทศนิยมของนาที (บังคับ ไม่ใช่ทางเลือก) ตามด้วยตัวอักษรทิศเหนือ ทิศใต้ ทิศตะวันออก หรือทิศตะวันตก ตามความเหมาะสม
ความสูง - AAAAAaaa
AAAAA - กำหนดเป็น 5 หลักโดยมี 0 นำหน้า
aaa - จำนวนทศนิยมของความสูง (จำนวนฟิลด์ที่บันทึกคือจำนวนฟิลด์ที่มีสำหรับความสูงในบันทึกที่เกี่ยวข้อง ลบฟิลด์ที่ใช้สำหรับ AAAAA ไปแล้ว)
PPPPpp - ความดันเป็น hPa (mb)พร้อมทศนิยมสองตำแหน่ง โดย PPPPpp กำหนดเป็น 6 หลักโดยมีเลขศูนย์นำหน้าสำหรับการตั้งค่าในช่วง 900 สำหรับการตั้งค่าย่อยของมาตรวัดความสูง 1013.25 mb (ISA Sea Level) มีรหัส PPPPpp คือ 101325 และ 980 mb มีรหัสคือ 098000
* การตั้งค่ามาตรวัดความสูง (และการเปลี่ยนแปลงใดๆ) อาจถูกบันทึกได้ เช่น เมื่อ FR ป้อนข้อมูลไปยังจอแสดงผลในห้องนักบิน (รหัส ATS สามตัวอักษร ดูย่อหน้าที่ 7 ) อย่างไรก็ตาม ห้ามใช้เพื่อเปลี่ยนระดับความสูงของความดันที่บันทึกในแต่ละครั้งที่ระบุในไฟล์ IGC ซึ่งต้องคงไว้ตามข้อมูลระดับน้ำทะเล ISA (1013.25 mb) ตลอดเวลา
ระดับความสูง GNSSหากไม่พบระดับความสูง GNSS จากเส้นตำแหน่ง GNSS เช่น ในกรณีของการตรึงตำแหน่งแบบ 2 มิติ (ระดับความสูงลดลง) จะต้องบันทึกเป็นศูนย์ในไฟล์รูปแบบ IGC เพื่อให้สามารถมองเห็นระดับความสูง GNSS ที่ไม่ถูกต้องได้อย่างชัดเจนในระหว่างการวิเคราะห์หลังการบิน ( AL3 )
2.5 การตั้งชื่อไฟล์

2.5.1รูปแบบชื่อไฟล์สั้น: YMDCXXXF.IGC
Y = ปี; ค่า 0 ถึง 9, หมุนเวียนทุก 10 ปี
M = เดือน; ค่า 1 ถึง 9 จากนั้น A สำหรับ 10, B=11, C=12
D = วัน; ค่า 1 ถึง 9 จากนั้น A=10, B=11, C=12, D=13, E=14, F=15, G=16, H=17, I=18, J=19, K=20, L=21, M=22, N=23, O=24, P=25, Q=26, R=27, S=28, T=29, U=30, V=31
C = ตัวอักษรรหัส IGC ของผู้ผลิต (ดูตารางด้านล่าง)
XXX = หมายเลขซีเรียล FR เฉพาะ (S/N); อักขระตัวอักษรและตัวเลข 3 ตัว
F = หมายเลขเที่ยวบินของวัน; 1 ถึง 9 จากนั้นถ้าจำเป็น A=10 ถึง Z=35

2.5.2รูปแบบชื่อไฟล์แบบยาว รูปแบบนี้ใช้ชุดอักขระเต็มในแต่ละฟิลด์ คั่นด้วยเครื่องหมายยัติภังค์ ลำดับฟิลด์จะเหมือนกับชื่อไฟล์แบบสั้น ตัวอย่างเช่น หากชื่อไฟล์แบบสั้นจากผู้ผลิต X คือ 36HXABC2.IGC ชื่อไฟล์แบบยาวที่เทียบเท่าคือ 2003-06-17-XXX-ABC-02.IGC ชื่อไฟล์แบบยาวอาจสร้างขึ้นโดยซอฟต์แวร์ที่เข้ากันได้กับชื่อไฟล์แบบยาว แม้ว่าโปรแกรม DATA, CONV และ VALI เวอร์ชัน DOS จะต้องยังคงสร้างและใช้ชื่อไฟล์แบบสั้นต่อไป ( AL3 )

2.5.3หมายเลขซีเรียล FR (S/N) ต้องใช้หมายเลขซีเรียล FR สามตัวอักษรในบันทึก Aและพิมพ์ลงบนตัวเครื่องบันทึก เว้นแต่จะมีจอแสดงผลอิเล็กทรอนิกส์ที่เข้าถึงได้ง่ายซึ่งมีหมายเลขซีเรียลรวมอยู่ด้วย

2.5.3.1 FR ที่มีอยู่ซึ่งใช้หมายเลขซีเรียลพร้อมระบบเข้ารหัส โดยที่ XXX แปลงเป็นรหัสตัวเลขห้าหลักอื่นที่ใช้ในระเบียน Aจะได้รับ "สิทธิ์แบบปู่" และไม่จำเป็นต้องเปลี่ยนแปลง FR ใหม่ต้องใช้ระบบตัวอักษรและตัวเลขสามตัวตามที่อธิบายไว้ข้างต้น

2.5.4 วันที่บิน - วันที่ที่ใช้ในชื่อไฟล์และในบันทึก H (รหัส DTE) คือวันที่ UTC ของการแก้ไขที่ถูกต้องครั้งแรกในบันทึกการบินที่ถ่ายโอนหลังจากเที่ยวบิน นั่นคือวันที่ที่ใช้กับเวลาในบรรทัดแรกของบันทึก B (แก้ไข) ไม่ใช่วันที่ในขณะที่เปิดเครื่องหรือบินขึ้น สิ่งนี้สำคัญอย่างยิ่งสำหรับเครื่องบันทึกที่ใช้งานในเขตเวลาที่เปิดเครื่องใกล้เที่ยงคืน UTC ( AL6 )

2.5.5. ความปลอดภัยของชื่อไฟล์ ชื่อไฟล์ไม่ได้รับการปกป้องโดยระบบรักษาความปลอดภัยอิเล็กทรอนิกส์ ซึ่งใช้กับข้อมูลภายในไฟล์เท่านั้น (ดูบทที่ 2 ย่อหน้า 2.8) ชื่อไฟล์อาจเปลี่ยนแปลงได้เพื่อวัตถุประสงค์เฉพาะ เช่น การแข่งขัน ซึ่งอาจสะดวกกว่าหากเปลี่ยนจากระบบชื่อ IGC ซึ่งไฟล์ถูกถ่ายโอนจาก FR เดิม (ย่อหน้า 2.5) เป็นระบบที่ใช้หมายเลขการแข่งขันเครื่องร่อนหรือชื่อนักบิน จะไม่มีการสูญเสียข้อมูลหรือความปลอดภัยเกิดขึ้น เนื่องจากข้อมูลทั้งหมดในชื่อไฟล์ IGC จะถูกทำซ้ำในไฟล์เองในบันทึก A และ H (AL2) ตัวอย่าง: 16AFXYZ2.IGC = 10 มิถุนายน 2544 หมายเลข FR ของ Filser XYZ เที่ยวบินที่ 2 ของวัน

2.5.6รหัสผู้ผลิต รหัสตัวอักษรเดียวและสามตัวแสดงไว้ด้านล่าง ผู้ผลิตที่ยื่นขอและชำระค่าธรรมเนียมการขออนุมัติ IGC แต่ไม่ได้อยู่ในรายชื่อ ควรยื่นขออนุมัติจากประธาน GFAC เพื่อขอจัดสรรรหัส ผู้ผลิตที่ใช้รูปแบบไฟล์ IGC แต่ไม่ได้ยื่นขออนุมัติ IGC ควรใช้รหัส X และ XXX ดูหมายเหตุ 2 ท้ายเล่ม

2.5.6.1 ชื่อไฟล์รูปแบบ Intermediate หากผู้ผลิตเลือกระบบที่ดาวน์โหลดข้อมูลจากเครื่องบันทึกในรูปแบบ Intermediate เช่น ไบนารี ชื่อไฟล์สำหรับรูปแบบ Intermediate จะต้องเหมือนกับไฟล์ IGC แต่ใช้รหัสสามตัวอักษรของผู้ผลิตแทน "IGC" หลังจุด จากนั้นจะสามารถแปลงรูปแบบ Intermediate เป็นรูปแบบ IGC ASCII ได้ผ่านยูทิลิตี้การแปลงซึ่งเป็นส่วนหนึ่งของไฟล์ IGC-XXX.DLL ของผู้ผลิต หรือสำหรับระบบก่อนหน้านี้ ให้ใช้โปรแกรม CONV-XXX.EXE ( AL8 )
รูปแบบไฟล์ข้อมูล IGC - รหัสสำหรับผู้ผลิตเครื่องบันทึกการบินที่ได้รับการรับรองจาก IGC ( AL5 )
รหัสอักขระเดี่ยว	รหัสสามตัวอักษร	ชื่อผู้ผลิต	รหัสอักขระเดี่ยว	รหัสสามตัวอักษร	ชื่อผู้ผลิต
เอ	จีซีเอส	การ์เร็ชท์	ส	เอสดีไอ	ปรับปรุงเครื่องมือข้อมูล
บี			ที	สาม	บริษัท ไทรอาดิส เอ็นจิเนียริ่ง จีเอ็มบีเอช
ซี	ลูกเบี้ยว	เคมบริดจ์ แอโร อินสตรูเมนต์ส	ใน		
ง	ดีเอสเอ็กซ์	ข้อมูล Swan/DSX	ใน		
และ	อีวา	อีดับบลิว เอวิโอนิกส์	ใน	เวส	เวสเตอร์โบเออร์
เอฟ	ใน	ไฟล์	เอ็กซ์	XXX	ผู้ผลิตอื่นๆ โปรดดูหมายเหตุด้านล่าง
จี	เอฟแอลเอ	สัญญาณเตือนการบิน (Flarm)	และ		
ชม	สช.	บุชเชล	กับ	ฉันจะ	แซนเดอร์
ฉัน	กระทำ	แอร์โคเทค	0		
เจ			1		
เค			2		
ล.	แอลเอ็กซ์เอ็น	LX การนำทาง	3		
เอ็ม	ฉัน	อุปกรณ์ร่อน IMI	4		
เอ็น	เอ็นทีอี	บริษัท นิว เทคโนโลยีส์ จำกัด	5		
เดอะ			6		
พี	พีอีเอส	เปชเกส	7		
คิว			8		
อาร์	พีอาร์ที	เทคโนโลยีการพิมพ์	9		

หมายเหตุ:

หากเป็นไปได้ อักษรตัวแรกของชื่อผู้ผลิตจะถูกกำหนดให้เป็นรหัสอักขระเดี่ยว ในกรณีที่มีการกำหนดอักษรนี้ไว้แล้ว โดยทั่วไปจะใช้อักษรตัวถัดไปในชื่อผู้ผลิต เป็นต้น
X และ XXX เป็นชื่อเรียกทั่วไปสำหรับไฟล์รูปแบบ IGC จากผู้ผลิตที่ไม่ได้ผลิตเครื่องบันทึกที่ได้รับการรับรองจาก IGC เครื่องบันทึกดังกล่าวจะไม่ได้รับการทดสอบและประเมินผลโดย GFAC และอาจไม่ตรงตามข้อกำหนดบางประการของ IGC เช่น การป้องกันความปลอดภัย การบันทึกระดับความสูงของความดัน ENL หรือตัวแปรอื่นๆ ไม่มีการรับประกันว่าไฟล์จะตรงตามรูปแบบ IGC อย่างแน่นอน แม้ว่าไฟล์ตัวอย่างจะถูกตรวจสอบว่าสอดคล้องกับรูปแบบ IGC หรือไม่ หากส่งอีเมลถึงประธาน GFAC เพื่อประเมินผล แม้จะผ่านขั้นตอนนี้แล้ว ก็ไม่สามารถรับประกันความสอดคล้องได้ เนื่องจากเครื่องบันทึกประเภทดังกล่าวยังไม่ได้ผ่านการประเมิน GFAC อย่างครบถ้วน โปรดทราบว่าแม้ว่าชื่อไฟล์จะไม่มีข้อมูล แต่รายละเอียดของผู้ผลิตและรุ่นของเครื่องบันทึกที่เกี่ยวข้องจะสามารถระบุได้ (หากไฟล์เป็นไปตามมาตรฐาน IGC) เนื่องจากข้อมูลเหล่านี้จะรวมอยู่ในบันทึก H (ส่วนหัว) ดังรายละเอียดด้านล่างภายใต้บันทึก H ในบรรทัด: HFFTYFRTYPE:MANUFACTURERSNAME,FRMODELNUMBER CRLF
จะไม่ใช้รหัสสามตัวอักษร PFC , PLT และ OOI เนื่องจากอาจทำให้เกิดความสับสนในบันทึก L
2.5.7 บันทึกบังคับบันทึกบางรายการเป็นสิ่งจำเป็นสำหรับไฟล์ IGC ใดๆ โดยสรุปได้ดังนี้:

ประเภทบันทึกตามลำดับไฟล์	ภาคผนวก 1 อ้างอิง	หมายเหตุ
เอ	3.1	ผู้ผลิตและรหัสเฉพาะสำหรับ FR
ชม	3.3.1	บันทึกส่วนหัว
ฉัน	3.4	การขยายเวลา FXAเป็นสิ่งที่จำเป็น
บี	4.1	แก้ไขบันทึก (ละติจูด/ลองจิจูด/ความสูง ฯลฯ)
เอฟ	4.2	ดาวเทียมที่ใช้ในบันทึก B
จี	3.2	บันทึกการรักษาความปลอดภัย
3. บันทึกข้อมูลแบบอินสแตนซ์เดียว
บันทึกเหล่านี้จะเกิดขึ้นเพียงครั้งเดียวในไฟล์ข้อมูลรูปแบบ IGC แต่ละไฟล์ แต่ประเภทบันทึกแต่ละประเภทอาจมีบรรทัดหลายบรรทัดที่ขึ้นต้นด้วยตัวอักษรประเภทของไฟล์นั้น

3.1 บันทึก A - หมายเลขประจำตัว FRบันทึก A ต้องเป็นบันทึกแรกในไฟล์ข้อมูล FR และประกอบด้วยหมายเลขประจำเครื่อง GNSS FR (S/N) สามตัวอักษรเฉพาะของผู้ผลิต FR ที่บันทึกเที่ยวบิน ( AL3 ) รูปแบบของบันทึก A:

AMMMNNNTEXTSTRING CR LF
บันทึก - คำอธิบาย	ขนาด	องค์ประกอบ	หมายเหตุ
ผู้ผลิต	3 ไบต์	เอ็มเอ็มเอ็ม	ตัวอักษรและตัวเลข ดูวรรค2.5.6
รหัสประจำตัวเฉพาะ	3 ไบต์	เอ็นเอ็นเอ็น	อักขระที่ถูกต้องคือตัวอักษรและตัวเลข ( AL3 )
ส่วนขยาย ID	ไม่จำเป็น	สตริงข้อความ	อักขระที่ถูกต้องคือตัวอักษรและตัวเลข
3.2 บันทึก G - ความปลอดภัยบันทึก G ตรวจสอบว่าข้อมูลไม่ได้ถูกเปลี่ยนแปลงในระหว่างหรือหลังการบิน ผู้ผลิต FR ต้องมีโปรแกรม VALI (ดูย่อหน้า 2.9.3.4 ในเนื้อหาหลักของเอกสารนี้) เพื่อตรวจสอบความสมบูรณ์ของไฟล์ด้วยรหัสความปลอดภัย รหัสความปลอดภัยต้องสร้างขึ้นโดย FR ไม่ใช่โดยคอมพิวเตอร์ที่ดึงข้อมูลการบินออกมา ซอฟต์แวร์วิเคราะห์การบินจากแหล่งอื่นที่ไม่ใช่ผู้ผลิตควรละเว้นข้อมูลรายละเอียดในบันทึกนี้ แต่สามารถใช้บันทึก G เป็นเครื่องหมายสำหรับตำแหน่งของข้อมูลและบันทึกอื่นๆ ในไฟล์ IGC ได้ บันทึกทั้งหมดต้องรวมอยู่ในกลไกความปลอดภัย ยกเว้นบันทึก H ที่มีแหล่งที่มา O หรือ P และบันทึก L ใดๆ ที่ไม่มีรหัสผู้ผลิต (เนื่องจากนักบินอาจใส่บันทึก L บางอย่างเข้าไป)

รูปแบบของ G Record:
กสสสสสสสสสสสสสสสสสส CR LF
กสสสสสสสสสสสสสสสสสส CR LF
ฯลฯ
G record - คำอธิบาย	ขนาด	องค์ประกอบ	หมายเหตุ
รหัสความปลอดภัย	สูงสุด 75 ไบต์ต่อบรรทัด	เอสเอสเอสเอส	อักขระที่ถูกต้องเป็นตัวอักษรและตัวเลข ดูบทที่ 2 ย่อหน้า 2.8.3.1 เกี่ยวกับความยาวของคีย์ความปลอดภัย ( AL3 )
G Record จะต้องไม่ใช้ตัวอักษรที่ไม่พิมพ์ เนื่องจากช่องว่างมักจะถูกลบออกเมื่อส่งไฟล์ ASCII ข้ามเครือข่ายการสื่อสารข้อมูล

3.3 บันทึก H - ส่วนหัวไฟล์

H-Record ใช้เพื่อจัดเก็บข้อมูลต่างๆ เช่น วันที่บันทึกการแก้ไขครั้งแรกใน B-Record ของไฟล์ IGC (นั่นคือวันที่ทำการบิน เว้นแต่จะทำในเขตเวลาที่หลายชั่วโมงนับจาก UTC) ชื่อนักบิน เครื่องร่อน ประเภทของ FR ที่ใช้ ประเภทของตัวรับสัญญาณ GNSS และเซ็นเซอร์วัดความดันอากาศ และอื่นๆ H-Record มีหลายประเภทย่อย ซึ่งบันทึกในบรรทัดแยกต่างหากที่ขึ้นต้นด้วย H รหัสสามตัวอักษร (CCC) ทั้งหมดที่มีธง H ในส่วนที่ 7 อาจเป็นประเภทย่อยของ H-Record

รายการในบรรทัดในระเบียน H อาจสร้างขึ้นโดย FR (รหัสต้นทาง F) หรือสำหรับรายการต่างๆ เช่น ชื่อนักบินและเครื่องร่อน อาจสร้างขึ้นโดยนักบินหรือ OO (บันทึกต้นทาง P และ O) หลังจากเที่ยวบิน (ดูบรรทัด "แหล่งข้อมูล" ในตารางด้านล่าง) เฉพาะข้อมูลระเบียน H ที่มีรหัสต้นทาง F เท่านั้นที่อยู่ภายใต้ระบบตรวจสอบรหัสความปลอดภัยและ VALI ( AL10 )

ภาคผนวก 1 ย่อหน้า 3.3 ย่อหน้าที่สอง คำที่อยู่ท้ายสุดที่อ่านได้ รูปแบบทั่วไปของ H-Record คือ: ตัวระบุเรคคอร์ด, แหล่งข้อมูล (S), ตัวระบุชนิดย่อยเรคคอร์ด (CCC), ชื่อยาวของชนิดย่อยเรคคอร์ด, เครื่องหมายโคลอน, ข้อมูลจริง (TEXTSTRING) ชื่อยาวนี้มีวัตถุประสงค์เพื่อช่วยเหลือผู้ที่อ่านไฟล์ สำหรับวัตถุประสงค์อย่างเป็นทางการเท่านั้น แหล่งที่มาของข้อมูล ชนิดย่อยเรคคอร์ด (CCC) และข้อมูลจริงถือเป็นข้อมูลสรุป

ข้อมูลอ้างอิงทางภูมิศาสตร์ GNSS ชื่อยาว เครื่องหมายโคลอน และชื่อของชุดข้อมูลอ้างอิงทางภูมิศาสตร์ (WGS84 = หมายเลข IGC 100 ดูย่อหน้า 8) จะอยู่หลังหมายเลขที่ IGC กำหนดให้กับข้อมูลอ้างอิง GPS ซึ่งอยู่ด้านหลังตัวระบุประเภทย่อยของเรกคอร์ด DTM โดยตรง

3.3.1 บันทึกที่จำเป็น บันทึก Hต่อไปนี้เป็นสิ่งจำเป็น ตามลำดับดังต่อไปนี้:

HFDTEDDMMYY
HFFXAAAAA
HFPLTPILOTINCHARGE: สตริงข้อความ
HFCM2CREW2:สตริงข้อความ
HFGTYGLIDERTYPE:สตริงข้อความ
HFGIDGLIDERID:สตริงข้อความ
HFDTMNNNGPSDATE:สตริงข้อความ
HFRFWFIRMWAREVERSION:TEXTSTRING
HFRHWHARDWAREVERSION: สตริงข้อความ
HFFTYFRTYPE:ชื่อผู้ผลิต,หมายเลขรุ่น FR
HFGPS:ชื่อผู้ผลิต,รุ่น,ช่อง,MAXALT( AL3 )
HFPRSPRESSALTSENSOR:ชื่อผู้ผลิต,รุ่น,MAXALT( AL3 )
นอกจากนี้คุณยังสามารถมีบันทึกเสริมดังต่อไปนี้:

HFCIDCOMPETITIONID: TEXTSTRING หมายเลขครีบเครื่องร่อน
HFCCLCOMPETITIONCLASS: TEXTSTRING เช่น Standard, 15m, 18m, Open
บันทึก	รูปแบบ	ตัวอย่าง	สรุป
เอชเอฟดีทีอี	
HFDTEDDMMYY
HFDTE280709

สำหรับวันที่ 28 กรกฎาคม 2552	วันที่ UTC ไฟล์นี้ถูกบันทึก
เอชเอฟเอฟเอ	
HFFXAAAAA
เอชเอฟเอฟเอ035

ความแม่นยำคงที่ 35 เมตร	แก้ไขความแม่นยำเป็นเมตร ดูข้อมูลอ้างอิงรหัสสามตัวอักษร FXA ด้วย
เอชเอฟพีแอลที	
HFPLTPILOTINCHARGE: สตริงข้อความ
HFPLTPILOTINCHARGE: บล็อกส์, บิล ดี
ชื่อนักบินที่เข้าแข่งขัน
เอชเอฟซีเอ็ม2	
HFCM2CREW2:สตริงข้อความ
HFCM2CREW2: สมิธ-แบร์รี่ จอห์น เอ
ชื่อนักบินคนที่สองในเครื่องบินสองที่นั่ง
เอชเอฟจีทีวาย	
HFGTYGLIDERTYPE:สตริงข้อความ
HFGTYGLIDERTYPE: Schleicher ASH-25
ชื่อข้อความอิสระของแบบจำลองเครื่องร่อน
HFGID	
HFGIDGLIDERID:สตริงข้อความ
HFGIDGLIDERID: N116 EL
หมายเลขทะเบียนเครื่องร่อน เช่น หมายเลข N
เอชเอฟดีทีเอ็ม	
HFDTMNNNGPSDATE:สตริงข้อความ
HFDTM100GPSDATUM: WGS-1984
ข้อมูล GPS ที่ใช้สำหรับจุดบันทึก - ใช้รหัส IGC 100 / WGS84 เว้นแต่คุณจะบ้า
เอชเอฟอาร์เอฟดับบลิว	
HFRFWFIRMWAREVERSION:TEXTSTRING
HFRFWFIRMWAREVERSION:6.4
สตริงข้อความอิสระใดๆ ที่อธิบายการแก้ไขเฟิร์มแวร์ของตัวบันทึก
เอชเอฟอาร์ดับบลิวเอช	
HFRHWHARDWAREVERSION: สตริงข้อความ
HFRHWHARDWARเวอร์ชัน:3.0
สตริงข้อความอิสระใดๆ ที่ให้หมายเลขการแก้ไขฮาร์ดแวร์ของตัวบันทึก
เฮฟฟี่	
HFFTYFRTYPE:ชื่อผู้ผลิต,หมายเลขรุ่น FR
HFFTYFRTYPE: Cambridge, FunkyLogger 77
ผู้ผลิตและรุ่นข้อความอิสระของ Logger
เอชเอฟจีพีเอส	
ผู้ผลิต HFGPS รุ่น ช่องสัญญาณ MAXALT
HFGPSMarconi,SuperX,12 ช่อง,10,000 เมตร
ผู้ผลิตและรุ่นของเครื่องรับ GPS ที่ใช้ในเครื่องบันทึกข้อมูลผมคิดว่ามีคำพิมพ์ผิดในส่วนนี้ของเอกสาร FAI (2008) ซึ่งบ่งชี้ว่าจำเป็นต้องใช้เครื่องหมายโคลอน
เอชเอฟพีอาร์เอส	
HFPRSPRESSALTSENSOR:ผู้ผลิต,รุ่น,MAXALT
HFPRSPRESSALTSENSOR: Sensyn,A32,11000m
คำอธิบายข้อความอิสระ (คั่นด้วยเครื่องหมายจุลภาค) ของเซ็นเซอร์วัดแรงดันที่ใช้ในเครื่องบันทึก
เอชเอฟซีไอดี	
HFCIDCOMPETITIONID: TEXTSTRING
HFCIDCOMPETITIONID: B21
หมายเลขครีบที่ใช้โดยทั่วไปในการจดจำเครื่องร่อน
เอชเอฟซีซีแอล	
HFCCLCOMPETITIONCLASS: TEXTSTRING
HFCCLCOMPETITIONCLASS: เครื่องร่อนมอเตอร์ 15 ม.
คำอธิบายข้อความอิสระของคลาสเครื่องร่อนนี้ เช่น มาตรฐาน 15 ม. 18 ม. เปิด
และนี่คือคำอธิบายฟิลด์จาก เอกสารต้นฉบับของ FAI

บันทึก H - คำอธิบาย	ขนาด	องค์ประกอบ	หมายเหตุ
แหล่งที่มาของข้อมูล	1 ไบต์	เอฟ โอ หรือ พี	วางไว้หลัง H นำหน้า: F=FR, O=OO, P=Pilot ใช้ F หากข้อมูลถูกถ่ายโอนจาก FR แม้ว่าข้อมูลนั้นจะถูกป้อนโดยนักบินหรือ OO ก็ตาม เพื่อให้แน่ใจว่าข้อมูลที่ป้อนก่อนบินได้รับการปกป้องโดยระบบรักษาความปลอดภัยในเครื่องบันทึก และหากมีการเปลี่ยนแปลงข้อมูลหลังจากบินแล้ว จะไม่ผ่านการตรวจสอบ VALI
ประเภทย่อยของบันทึก	3 ไบต์	ซีซีซี	ตัวอักษรและตัวเลข วางไว้หลังแหล่งข้อมูล ดูย่อหน้าที่ 7สำหรับ TLC
วันที่ UTC	6 ไบต์	วันเดือนปี	อักขระที่ถูกต้อง 0-9
หมวดหมู่ความแม่นยำ FXA , เมตร	3 ไบต์	เอเอเอ	อักขระที่ถูกต้อง 0-9 (ค่าเริ่มต้น 500)
สายบนเครื่องร่อน นักบินผู้รับผิดชอบและลูกเรือ 2	อย่างน้อย 30 ตัวอักษร	สตริงข้อความ	หลังจาก TLC ที่เกี่ยวข้อง PLT สำหรับชื่อนักบินผู้รับผิดชอบ CM2 สำหรับชื่อลูกเรือ 2 หากมี ( AL11 )
วันที่ GPS	3 ไบต์	เอ็นเอ็นเอ็น	ต้องใช้ WGS 84, 100 =WGS84 (ดูย่อหน้า 8)
บรรทัดบนชื่อ FR, เฟิร์มแวร์, ฮาร์ดแวร์	ตามความต้องการ	สตริงข้อความ	หลังจาก TLC ที่เกี่ยวข้อง (เช่น FTY สำหรับประเภท FR) ย่อหน้า 3.3.1
สายชนิด FR	ตามความต้องการ	เอฟ	ประกอบด้วยข้อมูลโมเดลโดยละเอียด รวมถึงประเภทย่อย เช่น ไม่ใช่แค่โมเดล XXX 1 เท่านั้น แต่รวมถึงโมเดล 1a, 1b เป็นต้น ( AL9 )
สาย HFGPS	ตามความต้องการ	สตริงข้อความ	ระบุผู้ผลิตเครื่อง GPS ประเภท จำนวนช่องสัญญาณ และความสูงสูงสุดของ GNSS เป็นเมตรที่สามารถบันทึกได้ในไฟล์ IGC ใช้เครื่องหมายจุลภาคคั่นข้อมูลแต่ละส่วน สำหรับระบบ GLONASS ของรัสเซีย ให้ใช้รหัส GLO แทน GPS และสำหรับระบบ Galileo ของยุโรป ให้ใช้รหัส GAL (GLO และ GAL ระบุไว้ในย่อหน้าที่ 7 ) หากใช้ระบบ GNSS อื่น ให้สมัครใช้รหัสสามตัวอักษรที่เหมาะสมกับ GFAC สำหรับอุปกรณ์ที่รับข้อมูลจากระบบ GNSS มากกว่าหนึ่งระบบ ให้ใส่ชื่อผู้ผลิตเครื่องรับก่อน จากนั้นจึงใส่รหัสสามตัวอักษรสำหรับระบบ GNSS แรก ตามด้วยจำนวนช่องสัญญาณและความสูงสูงสุดของ GNSS เป็นเมตร จากนั้นจึงใส่ข้อมูลเดียวกันสำหรับระบบ GNSS ที่สอง และพิมพ์ข้อมูลเดียวกันนี้สำหรับระบบอื่นๆ ต่อไป ( AL11 )
สาย HFPRS	ตามความต้องการ	สตริงข้อความ	ข้อมูลเซ็นเซอร์วัดความดันและระดับความสูง (ผู้ผลิตและประเภท) และค่าระดับความสูงของความดันสูงสุดเป็นเมตรที่สามารถบันทึกลงในไฟล์ IGC ได้ ใช้เครื่องหมายจุลภาคคั่นระหว่างข้อมูลแต่ละส่วน ( AL3 )
สาย HF FRS	ตามความต้องการ	สตริงข้อความ	รูปแบบ: HF FRS SECURITY SUSPECT USE VALI PROGRAM: TEXTSTRING ต้องใช้ในกรณีที่สงสัยว่าระบบรักษาความปลอดภัยมีปัญหา เช่น หากระบบรักษาความปลอดภัยทางกายภาพของเครื่องบันทึก (ไมโครสวิตช์) ทำงานอยู่ คำที่อยู่หน้าเครื่องหมายโคลอนเป็นคำบังคับ เหตุผลในการอ้างถึงโปรแกรม VALI คือ นี่เป็นวิธีเดียวที่สามารถตรวจสอบความปลอดภัยได้อย่างสมบูรณ์ ไม่ควรถือว่าวิธีนี้ใช้แทนการตรวจสอบ VALI เต็มรูปแบบ ซึ่งจะตรวจจับการเปลี่ยนแปลงใดๆ หลังจากการถ่ายโอนข้อมูล สตริงข้อความควรเป็นคำอธิบายถึงข้อผิดพลาดที่อาจเกิดขึ้น เช่น: "ไมโครสวิตช์รักษาความปลอดภัยทำงานอยู่ เครื่องบันทึกต้องรีเซ็ต" ( AL6 )
3.3.2 บันทึก Hเพิ่มเติมข้อมูลเหล่านี้เป็นทางเลือก สามารถแนบข้อมูลเพิ่มเติมต่อจากบันทึกบังคับได้ บันทึกเพิ่มเติมสองรายการ (Comp ID และ class) แสดงอยู่ด้านล่าง

HSCIDCOMPETITIONID : TEXTSTRING CR LF
HSCCLCOMPETITIONCLASS : สตริงข้อความ CR LF
หมายเหตุ - Ian Forster-Lewis: ผมคิดว่านี่เป็นการพิมพ์ผิด: H S CID จะไม่ใช่รูปแบบที่ถูกต้อง บันทึกที่ถูกต้องควรเป็น H F CID เช่นเดียวกับ HFCCL

3.3.3ชื่อและการระบุตัวตน

ชื่อที่คล้ายกัน ในกรณีที่อาจมีบุคคลที่มีชื่อคล้ายกันหรือคล้ายกัน (เช่น Smith/Schmidt) ควรใช้ชื่อย่อเต็มหรือชื่ออื่นๆ นอกจากนี้ ควรมีข้อมูล TLC ของวันเกิดสำหรับวันเดือนปีเกิด และหากใช้ ต้องระบุในบรรทัดถัดจากชื่อนักบินในรูปแบบ DDMMYY (รูปแบบเดียวกับที่ใช้สำหรับวันบินในบันทึก H )

ชื่อของสมาชิกลูกเรือ 2 (รหัส CM2) นามสกุลก่อน จากนั้นชื่ออื่นหรืออักษรย่อโดยไม่มีเครื่องหมายวรรคตอนแต่คั่นด้วยช่องว่าง (เช่น SMITH BS หรือ SMITH BERNALD)

ควรมีอักขระที่เพียงพอสำหรับชื่อและการระบุตัวตนที่ยาว เช่น สำหรับการจดทะเบียนเครื่องร่อน ให้อนุญาตให้จดทะเบียนเป็น XXXX-AAAA (โดย XXXX คือตัวระบุของประเทศหรือองค์กรกีฬาทางอากาศแห่งชาติ) ซึ่งกำหนดให้มีอักขระอย่างน้อย 9 ตัวในช่องนี้ ผู้ผลิตควรกำหนดให้มีอักขระมากกว่าจำนวนที่กำหนดในช่องเหล่านี้ เพื่อให้สามารถกรอกคำประกาศเที่ยวบินได้ครบถ้วน ( AL3 )

สโมสรหรือองค์กรที่บินหรือดำเนินการ (รหัส CLB) กับประเทศ (เช่น LASHAM UK, ELMIRA US) หากไม่มีช่องว่างสำหรับกรอกชื่อประเทศ ควรใช้รหัสสองตัวอักษรจากรายชื่อประเทศตามมาตรฐาน ISO 3166 (รหัสเหล่านี้ใช้สำหรับประเทศในที่อยู่อินเทอร์เน็ตด้วย) รหัสประเทศสองตัวอักษรตามมาตรฐาน ISO 3166 บางส่วนมีดังนี้ ( AL3 ):

รหัสประจำชาติสองตัวอักษร ISO 3166
AR - อาร์เจนตินา
AT - ออสเตรีย
AU - ออสเตรเลีย
BE - เบลเยียม
BR - บราซิล
CA - แคนาดา
CH - สวิตเซอร์แลนด์
CL - ชิลี
CN - จีน
CO - โคลอมเบีย
CZ - สาธารณรัฐเช็ก
DE - เยอรมนี
DK - เดนมาร์ก
EC - เอกวาดอร์ - เอสโตเนีย
EG - อียิปต์
ES - สเปน
FI - FINLAND
FR - FRANCE
GR - GREECE
HR - CROATIA (HRVATSKA)
HU - HUNGARY
ID - INDONESIA
IE - IRELAND
IL � ISRAEL
IN � INDIA
IS � ICELAND
IT � ITALY
JP � JAPAN
KR � KOREA (S)
LT � LITHUANIALV - LATVIA
MX � MEXICO
MY � MALAYSIA
NL - เนเธอร์แลนด์
ไม่ - นอร์เวย์
นิวซีแลนด์ - นิวซีแลนด์
PL - โปแลนด์
PT - โปรตุเกส
RU - รัสเซีย
SE - สวีเดน
SI - สโลวี เนีย
SK - สโลวาเกีย
TR - ตุรกี ไต้หวัน
-
สหราชอาณาจักร ไต้หวัน - สหราชอาณาจักร
สหรัฐอเมริกา - สหรัฐอเมริกา
UY - อุรุกวัย - เวเนซุเอลา
ZA - แอฟริกาใต้
3.4 บันทึก I - ส่วน ขยายของบันทึก FIX Bบันทึก I กำหนดส่วนขยายใดๆ ของ บันทึก FIX Bในรูปแบบของรายการรหัสสามตัวอักษร (CCC) ที่เหมาะสม ซึ่งข้อมูลจะปรากฏในตอนท้ายของบันทึก B ที่ตามมา แต่ละไฟล์จะมีเพียงบรรทัดบันทึก I หนึ่งบรรทัด ซึ่งอยู่หลังบันทึก Hและก่อนบันทึก B แรก ต้องระบุค่าความแม่นยำของ Fix ( FXA ) ในรูปแบบของค่าความคลาดเคลื่อนของตำแหน่งโดยประมาณ (ดูอภิธานศัพท์ภายใต้ EPE) ตามด้วย SIU, ENL และ RPM หากบันทึกใน FR ที่เกี่ยวข้อง โปรดทราบว่าแม้ว่าหมายเลข SIU จะเป็นตัวเลือกในบันทึก B แต่บันทึก F (กลุ่มดาวเทียมที่ใช้) เป็นสิ่งจำเป็น โปรดดูย่อหน้า4.3รูปแบบของบันทึก I มีดังนี้: ( AL11 )

INNSSFFCCCSSSFFCCC CR LF
ฉันบันทึก - คำอธิบาย	ขนาด	องค์ประกอบ	หมายเหตุ
จำนวนส่วนขยาย	2 ไบต์	เอ็นเอ็น	อักขระที่ถูกต้อง 0-9
หมายเลขไบต์เริ่มต้น	2 ไบต์	เอสเอส	อักขระที่ถูกต้อง 0-9
หมายเลขไบต์เสร็จสิ้น	2 ไบต์	เอฟเอฟ	อักขระที่ถูกต้อง 0-9
รหัส 3 ตัวอักษร	3 ไบต์	ซีซีซี	ตัวอักษรและตัวเลข ดูรายชื่อรหัสในย่อหน้าที่ 7
ไบต์แรกของข้อมูลส่วนขยายจะเริ่มต้นที่ตำแหน่งไบต์ 36 เสมอ เนื่องจากเป็นจุดสิ้นสุดของละติจูด/ลองจิจูด/ความสูงพื้นฐานของเรกคอร์ด B

การนับไบต์เริ่มต้นจากจุดเริ่มต้นของเรคคอร์ด B โดยนำ B แรกในบรรทัดเป็นไบต์ที่หนึ่ง ตัวอย่าง:

ฉัน 01 36 40 FXA CR LF
ข้อมูลนี้แสดงให้เห็นว่าค่าความแม่นยำคงที่ ( FXA ) ถูกบันทึกระหว่างไบต์ 36 ถึง 40 ในแต่ละบรรทัด B-record และสำหรับอุปกรณ์ที่บันทึกข้อมูลดาวเทียมที่ใช้งานอยู่ (SIU) และระดับเสียงรบกวนเครื่องยนต์ (ENL) ด้วย:

ฉัน 04 3638 FXA 3940 SIU 4143 ENL 4446 RPM CR LF
แสดงให้เห็นว่าในแต่ละบรรทัดของเรคคอร์ด B จะมีการบันทึกค่า Fix Accuracy ( FXA ) ระหว่างไบต์ 36 และ 38, Satellites In Use (SIU) ระหว่างไบต์ 39 และ 40, Engine Noise Level (ENL) ระหว่างไบต์ 41 และ 43 และ RPM ระหว่างไบต์ 44 และ 46 เพื่อความชัดเจน ได้มีการแทรกช่องว่างบางส่วนในบรรทัดตัวอย่างด้านบน ซึ่งไม่ควรใช้ในเรคคอร์ด B จริงในไฟล์ IGC ( AL11 )

3.5 ระเบียน J - ส่วนขยายของระเบียน Kระเบียน K ใช้สำหรับข้อมูลที่ต้องอัปเดตตามความคืบหน้าของเที่ยวบิน แต่ไม่จำเป็นต้องอัปเดตบ่อยเท่ากับระเบียน Bระเบียน J เป็นบรรทัดเดียวที่กำหนดว่าข้อมูลใดที่จะอยู่ในบรรทัดระเบียน K ถัดไป ระเบียนนี้ทำหน้าที่เดียวกันกับระเบียน K เช่นเดียวกับระเบียน I (3.4 ข้างต้น) สำหรับระเบียนB ระเบียน และทำงานในลักษณะเดียวกัน ระเบียนนี้จะถูกวางไว้ในไฟล์ทันทีหลังบรรทัดระเบียน I ก่อนระเบียน B แรก รูปแบบของระเบียน J มีดังนี้:

JNNSSFFCCCSSFFCCC CR LF
J record - คำอธิบาย	ขนาด	องค์ประกอบ	หมายเหตุ
จำนวนส่วนขยาย	2 ไบต์	เอ็นเอ็น	อักขระที่ถูกต้อง 0-9
หมายเลขไบต์เริ่มต้น	2 ไบต์	เอสเอส	อักขระที่ถูกต้อง 0-9 (จากจุดเริ่มต้นของ K Record)
หมายเลขไบต์เสร็จสิ้น	2 ไบต์	เอฟเอฟ	อักขระที่ถูกต้อง 0-9
รหัส 3 ตัวอักษร	3 ไบต์	ซีซีซี	ตัวอักษรและตัวเลข ดูวรรค 7
ตัวอย่าง:

J 0 1 0 8 1 2 HDT CR LF
สิ่งนี้แสดงให้เห็นว่า True Heading (HDT) จะถูกบันทึกระหว่างไบต์ 8 และ 12 บนบรรทัด K-record แต่ละบรรทัด

3.6 บันทึก C - งาน (การประกาศก่อนบิน)

ระเบียน C ใช้เพื่อระบุงานและประกาศก่อนการตรวจสอบ โดยจะวางไว้ในไฟล์ IGC ก่อนระเบียนB แรก และหลังระเบียน H, I และ J

3.6.1บรรทัดในบันทึก C บรรทัดแรกประกอบด้วยวันที่และเวลา UTC ของการประกาศ วันที่ท้องถิ่นของวันบินที่ต้องการ รหัสภารกิจ จำนวนจุดเลี้ยวของภารกิจ และสตริงข้อความที่สามารถใช้เพื่ออธิบายภารกิจ (เช่น สามเหลี่ยม 500k) นอกจากนี้ เครื่องบันทึกอาจกำหนดค่าเพื่อให้นักบินสามารถป้อนวันที่บินที่ต้องการในเวลาท้องถิ่น ไม่ใช่วันที่ UTC ซึ่งจะแตกต่างกันในประเทศที่มีเวลาชดเชยจาก UTC มาก (รหัสสามตัวอักษรสำหรับเขตเวลาชดเชยคือ TZN ดูรายการในย่อหน้าที่ 7 ) บรรทัดอื่นๆ ประกอบด้วยพิกัดละติจูด/ลองจิจูด WGS84 และสตริงข้อความสำหรับสถานที่หรือจุดที่เกี่ยวข้อง ซึ่งรวมถึงสนามบินขึ้นบิน จุดเริ่มต้น จุดเลี้ยว จุดสิ้นสุด และสนามบินลงจอด หลังจากบรรทัดแรก บรรทัดอื่นๆ ประกอบด้วยพิกัดละติจูด/ลองจิจูด WGS84 ของจุด ตามด้วยสตริงข้อความสำหรับสถานที่หรือจุดที่เกี่ยวข้อง ข้อความที่อธิบายประเภทของจุด (ดูตัวอย่างด้านล่าง) เป็นสิ่งจำเป็นเพื่อให้สามารถเห็นลักษณะของจุดต่างๆ ได้อย่างชัดเจนโดยการดูไฟล์ IGC ( AL6 ) และ 11)

3.6.2คำศัพท์ของ IGC คำว่า "จุดแวะพัก" หมายถึงจุดเริ่มต้น จุดกลับรถ หรือจุดสิ้นสุด คำว่า "จุดกลับรถ" หมายถึงจุดในเส้นทางที่วัดได้ระหว่างจุดเริ่มต้นและจุดสิ้นสุด จุดที่ต้องระบุไว้อย่างชัดเจนในประกาศการบินอย่างเป็นทางการของ IGC คือจุดเริ่มต้น จุดกลับรถ และจุดสิ้นสุดที่ตั้งใจไว้ (ประมวลกฎหมายกีฬา มาตรา 3 วรรค 4.2) จำนวนจุดกลับรถจะเป็นศูนย์สำหรับเที่ยวบินตรงเป้าหมาย หนึ่งจุดสำหรับเที่ยวบินขาออกและขากลับ สองจุดสำหรับเที่ยวบินสามเหลี่ยม สามจุดสำหรับระยะทาง 3-TP และมากกว่านั้นสำหรับภารกิจการแข่งขันบางประเภท ( AL6 )

3.6.3การขึ้นและลงจอด เส้นสองเส้นในรูปแบบ C-record สำหรับสนามบินขึ้นและลงจอด (หรือตำแหน่งขาออก หากมี) มีไว้สำหรับข้อมูลทั่วไป ไม่ใช่เป็นส่วนหนึ่งของประกาศการบินอย่างเป็นทางการของ IGC สามารถป้อนค่าโดยประมาณได้ หรือหากหาพิกัดได้ยากหรือไม่ได้ป้อน ค่าที่ตั้งไว้จะเป็น 00000000N000000000E สำหรับสองเส้นนี้ ( AL6 )

3.6.4จำนวนจุดเลี้ยวและเส้นบันทึก C-Record จากข้อมูลข้างต้นจะเห็นได้ว่าจำนวนจุดเลี้ยวจะน้อยกว่าจำนวนเส้นหลังจากเส้นที่ 1 (นั่นคือเส้นที่มีข้อมูลละติจูด/ลองจิจูด) สี่เส้น ข้อมูลที่ไม่ใช่จุดเลี้ยวทั้งสี่เส้นนี้ใช้สำหรับสนามบินที่ขึ้นบิน จุดเริ่มต้นที่แน่นอน จุดสิ้นสุดที่แน่นอน และสนามบิน/ตำแหน่งที่ลงจอด จำนวนจุดเลี้ยวจะถูกรวมเป็นฟิลด์ย่อยในเส้นที่ 1 ของบันทึก C-record และวางไว้หน้าสตริงข้อความเสริมที่ท้ายเส้น (ในรูปแบบ TT ในภาพประกอบด้านล่าง) ( AL6 )

3.6.5งานด้านพื้นที่ การรวมฟังก์ชันนี้ไว้ในเครื่องบันทึกการบินเป็นทางเลือก ในการแข่งขันบางรายการ พื้นที่ที่จะไปถึงจะถูกระบุโดยอ้างอิงจากจุดอ้างอิง (Waypoint) โดยระบุระยะทางและทิศทางที่แท้จริง (รัศมี) จากจุดอ้างอิง หากเครื่องบันทึกการบินสามารถบันทึกข้อมูลนี้ลงในบันทึก C ได้ ให้ใช้ระบบต่อไปนี้ในไฟล์ IGC: ที่ส่วนท้ายของบรรทัดจุดอ้างอิงที่เกี่ยวข้องในบันทึก C ระยะทางต่ำสุดและสูงสุดจะตามด้วยหน่วยกิโลเมตรจาก WP ตามด้วยระยะทาง 1 และ 2 เป็นองศาจริงจาก WP แล้วตามด้วยคำว่า AREA หลังประเภทของจุด ในกรณีที่การแข่งขันใช้หน่วยอื่นที่ไม่ใช่กิโลเมตร (เช่น มาตรา หรือไมล์ทะเลระหว่างประเทศ) จะต้องแปลงหน่วยเพื่อให้ไฟล์ IGC ยังคงใช้หน่วยกิโลเมตร (และกิโลเมตรทศนิยมตามความจำเป็น) พื้นที่จะหมุนตามเข็มนาฬิกาจากตำแหน่ง 1 ถึง 2 ในกรณีที่พื้นที่วงกลมรอบจุดใดจุดหนึ่ง ให้ใช้ตำแหน่งสองตำแหน่ง คือ 000 ถึง 360 และระยะห่างต่ำสุดจะเป็นศูนย์ หากต้องการระบุพื้นที่อ้างอิงถึงจุดอ้างอิง ให้เพิ่มบรรทัดบันทึก C ที่กำหนดจุดอ้างอิง แต่ก่อนถึง CRLF ที่ส่วนท้ายของบรรทัด ดังนี้

"DDDDddDDDDDDdddBBBbbbBBBbbbAREA"
ระยะทางสองระยะ Dd คือระยะทางขั้นต่ำแรกจาก WP เป็นกิโลเมตร และกิโลเมตรทศนิยม จากนั้นเป็นระยะทางสูงสุด ระยะ Bb ทั้งสองระยะเป็นองศา และองศาทศนิยมจริงจาก WP โดยพื้นที่งานขยายตามเข็มนาฬิกาจากระยะ 1 ถึง 2

ตัวอย่างเช่น: "C....0012000 0032000 122000 182000TURN AREA" จะเป็นพื้นที่ตั้งแต่ 12 ถึง 32 กม. จาก WP ระหว่างตำแหน่ง 122 และ 182 จากจุด ( AL6 )

รูปแบบของ C Record เป็นดังต่อไปนี้ โดยใช้ละติจูด N และลองจิจูด E เป็นตัวอย่าง:

C DD MM YY HH MM SS FDFMFY IIII TT TEXT STRING CR LF
C DD MM MMM N DDD MMMMM E สตริงข้อความ TAKEOFF CR LF
C DD MM MMM N DDD MMMMM E START TEXT STRING CR LF
C DD MM MMM N DDD MM MMM E TURN TEXT STRING CR LF
C DD MM MMM N DDD MM MMM E TURN TEXT STRING CR LF
C DD MM MMM N DDD MM MMM E FINISH TEXT STRING CR LF
C DD MM MMM N DDD MM MMM E LANDING TEXT STRING CR LF
มีการเพิ่มช่องว่างระหว่างฟิลด์ข้อมูลในตัวอย่างนี้เพื่อช่วยให้ชัดเจนยิ่งขึ้น

สตริงข้อความมีวัตถุประสงค์เพื่อเป็นชื่อและคำอธิบายสั้น ๆ ของจุด สำหรับพื้นที่ที่อ้างอิงถึงจุดเปลี่ยน:

C DD MMMMMN DDD MMMMME 0012000 0032000 122000 182000พื้นที่เลี้ยว CR LF( AL6 )
บันทึก C - คำอธิบาย	ขนาด	องค์ประกอบ	หมายเหตุ
วันที่ UTC	6 ไบต์	วันเดือนปี	อักขระที่ถูกต้อง 0-9
เวลา UTC	6 ไบต์	ฮึ่มมมส์	อักขระที่ถูกต้อง 0-9
วันที่บิน	6 ไบต์	เอฟดีเอฟเอ็มเอฟวาย	อักขระที่ถูกต้องคือ 0-9 หากไม่ใช้ให้เติมด้วยเลขศูนย์ (AL2)
หมายเลขงานประจำวันนี้	4 ไบต์	สาม	อักขระที่ถูกต้องเป็นตัวอักษรและตัวเลข อาจเป็นรหัสอ้างอิง ID หรือลำดับ 1-2-3 หากไม่ได้ใช้ ค่าเริ่มต้นคือ 0001 การประกาศครั้งสุดท้ายก่อนเครื่องขึ้นบินเป็นการประกาศขั้นสุดท้าย (ไม่จำเป็นต้องประกาศภารกิจในวันบิน การประกาศทางอิเล็กทรอนิกส์จะมีผลใช้ได้จนกว่าจะถูกแทนที่ด้วยการประกาศที่ถูกต้องอื่น)
จำนวน TP ของงาน	2 ไบต์	ทีที	อักขระที่ถูกต้อง 0-9, 1 แทนการออกและกลับ, 2 แทนรูปสามเหลี่ยม เป็นต้น
TO หรือ A/F LatLon	17 ไบต์	DDMMmmmN
DDDMMmmmE
ไปยังข้อมูลอ้างอิงทางภูมิศาสตร์ WGS84	จุดที่ประกาศไว้จะถูกกำหนดโดยละติจูดและลองจิจูด ( AL11 ) บวกสตริงข้อความสำหรับรหัสจุดเลี้ยวในท้องถิ่น หมายเลข ตัวอักษร ชื่อ หรือคำอธิบายโดยย่อ จุดเริ่มต้น จุดเลี้ยว และจุดสิ้นสุดที่ประกาศไว้พร้อมละติจูดและลองจิจูดเป็นสิ่งจำเป็น ข้อมูลการขึ้น/ลงจอดหรือสนามบินไม่รวมอยู่ในข้อกำหนดการประกาศ IGC ที่กำหนดไว้ใน Sporting Code for Gliding (SC3) แต่เป็นข้อมูลเพิ่มเติมที่มีประโยชน์ โดยเฉพาะอย่างยิ่งเมื่อมีการใช้จุดเริ่มต้นหรือจุดสิ้นสุดจากระยะไกล หากพิกัดของจุดที่ไม่ได้เป็นส่วนหนึ่งของภารกิจอย่างเป็นทางการนั้นยากที่จะระบุล่วงหน้า (เช่น พิกัดการขึ้น พิกัดการลงจอด หรือพิกัดการขึ้นและลงจอด) ควรตั้งค่าเป็น 00000000N000000000E
เริ่มละติจูด/ลองจิจูด
T/P ละติจูด/ลองจิจูด
T/P ละติจูด/ลองจิจูด
เสร็จสิ้น LatLon
ที่ดินหรือ A/F LatLon
4.บันทึกข้อมูลอินสแตนซ์หลายรายการ
เหล่านี้เป็นประเภทบันทึกที่สามารถเกิดขึ้นซ้ำได้ในเวลาต่างกันในระหว่างไฟล์ IGC ซึ่งแตกต่างจากบันทึกอินสแตนซ์เดียวที่เกิดขึ้นในแต่ละไฟล์ในที่เดียวเท่านั้น

4.1 B RECORD - FIX.ไม่นับ CRLF ล่าสุด ซึ่งประกอบด้วยข้อมูลพื้นฐาน 35 ไบต์ บวกกับข้อมูลอักขระที่กำหนดไว้ในI Recordเช่น ความแม่นยำในการแก้ไข ( FXAในรูปแบบของตัวเลข Estimated Position Error ดูอภิธานศัพท์ภายใต้ EPE), Satellites In Use (SIU), Engine Noise Level (ENL สำหรับเครื่องร่อนแบบใช้มอเตอร์ทั้งหมด), RPM (เพิ่มเติมสำหรับเครื่องร่อนแบบใช้มอเตอร์ที่มีเครื่องยนต์เงียบ) ข้อมูลพื้นฐานที่จำเป็นคือ: UTC, ละติจูด WGS84, ลองจิจูด WGS84, ความถูกต้องของการแก้ไข, ความแม่นยำในการแก้ไข, ระดับความสูงของความดัน และระดับความสูงของ GNSS ข้อมูลทั้งหมดในแต่ละ B-record ต้องมีเวลาออกข้อมูลภายใน 0.1 วินาทีของเวลาที่ระบุใน B-record ในกรณีที่ใช้ข้อมูล NMEA ภายใน FR ข้อมูลการแก้ไขควรนำมาจากประโยค GGA หรือ GNS GGA เป็นระบบเฉพาะสำหรับระบบ GPS ของสหรัฐอเมริกา GNS มีไว้สำหรับระบบ GNSS ทั้งหมด (GPS, GLONASS, Galileo และระบบในอนาคต) และควรใช้หากมีอยู่ในบอร์ด GNSS ที่ติดตั้งไว้ ในบันทึก B ควรบันทึก FXAเป็นกลุ่มตัวเลขสามหลักในหน่วยเมตร และ SIU เป็นหมายเลขสองกลุ่ม SIU เป็นบันทึกเสริมและอาจใช้เพื่อสำรองข้อมูลดาวเทียมที่มีรายละเอียดมากขึ้นใน บันทึก F ที่จำเป็น ควรใส่เลขศูนย์นำหน้าตามความจำเป็น เนื่องจาก GNSS FR ที่ได้รับการอนุมัติจาก IGC ก่อนหน้านี้อาจไม่มีFXAและ SIU ในบันทึก B ตำแหน่งของข้อมูลนี้ในแต่ละบรรทัดบันทึก B จะต้องระบุ (เช่น สำหรับโปรแกรมวิเคราะห์) โดยระบุตำแหน่งฟิลด์เพิ่มเติมในบันทึกI ควรวาง FXAไว้หลังสองกลุ่มสำหรับระดับความสูง ตามด้วยฟิลด์เสริม เช่น SIU และ ENL สำหรับเครื่องร่อนแบบมอเตอร์ ในแต่ละบรรทัดของเรกคอร์ด B FXAมักจะใช้พื้นที่ไบต์ 36, 37 และ 38, ไบต์ SIU 39 และ 40, ENL 39-41 หรือ 41-43 ขึ้นอยู่กับว่าใช้ SIU หรือไม่ รูปแบบของข้อมูลพื้นฐานคือ: ( AL11 )

BHHMMSSDDM MM MM NDDDM MM MM EVPPPPPGGGGG CR LF
บันทึก B - คำอธิบาย	ขนาด	องค์ประกอบ	หมายเหตุ
เวลา UTC	6 ไบต์	ฮึ่มมมส์	อักขระที่ถูกต้อง 0-9 เมื่อได้รับค่า GNSS ที่ถูกต้อง เวลา UTC ในบรรทัดบันทึก B จะต้องได้รับโดยตรงจากแพ็คเกจข้อมูล GNSS เดียวกันกับที่เป็นแหล่งของละติจูด/ลองจิจูดและระดับความสูง GNSS ที่บันทึกในบรรทัดบันทึก B เดียวกัน แหล่งข้อมูลอื่นๆ สำหรับเวลาในบรรทัดบันทึก B (เช่น นาฬิกาเวลาจริงในเครื่องบันทึก) ต้องใช้เฉพาะเพื่อให้ความต่อเนื่องของเวลาในกรณีที่ไม่มีค่า GNSS ( AL9 )
ละติจูด	8 ไบต์	วววววววววววววว/ส	อักขระที่ถูกต้องคือ N, S, 0-9 ได้มาโดยตรงจากแพ็กเกจข้อมูล GPS เดียวกันกับที่เป็นแหล่งที่มาของเวลา UTC ที่บันทึกในบรรทัด B-record เดียวกัน หากไม่ได้ค่าละติจูดจากข้อมูลดาวเทียม การกำหนดระดับความสูงของความกดอากาศจะต้องดำเนินต่อไป โดยใช้เวลาจาก RTC ในกรณีนี้ ในบรรทัด B-record จะต้องทำซ้ำค่าละติจูดสุดท้ายที่ได้จากข้อมูลดาวเทียม จนกว่าจะได้ค่า GPS กลับมา ( AL11 )
ลองจิจูด	9 ไบต์	วววววววววววววววว	อักขระที่ถูกต้องคือ E, W, 0-9 ได้มาโดยตรงจากแพ็กเกจข้อมูล GPS เดียวกันกับที่เป็นแหล่งเวลา UTC ที่บันทึกในเส้นบันทึก B เดียวกัน หากไม่พบลองจิจูดจากข้อมูลดาวเทียม การกำหนดระดับความสูงและความกดอากาศจะต้องดำเนินต่อไป โดยใช้เวลาจาก RTC ในกรณีนี้ ในเส้นบันทึก B จะต้องทำซ้ำลองจิจูดสุดท้ายที่บันทึกจากข้อมูลดาวเทียม จนกว่าจะได้ตำแหน่ง GPS อีกครั้ง ( AL11 )
แก้ไขความถูกต้อง	1 ไบต์	เอ หรือ วี	ใช้ A สำหรับการแก้ไขแบบ 3 มิติและ V สำหรับการแก้ไขแบบ 2 มิติ (ไม่มีระดับความสูง GPS) หรือไม่มีข้อมูล GPS (ข้อมูลระดับความสูงความกดอากาศจะต้องบันทึกต่อไปโดยใช้เวลาจาก RTC) ( AL11 )
กด Alt	5 ไบต์	พีพีพีพี	ระดับความสูงจากระดับน้ำทะเลตามเกณฑ์มาตรฐาน ICAO ISA สูงกว่า 1013.25 HPa อักขระที่ถูกต้องคือ 0-9 และเครื่องหมายลบ "-" ค่าลบต้องมีเครื่องหมายลบแทนเลขศูนย์นำหน้า
GNSS ทางเลือก	5 ไบต์	ก๊กก๊ก	ความสูงเหนือรูปทรงรี WGS84 อักขระที่ถูกต้อง 0-9
หากต้องการเพิ่มค่าความแม่นยำในการแก้ไข ( FXA , บังคับ), ดาวเทียมที่ใช้งาน (SIU), ระดับเสียงเครื่องยนต์ (ENL) และ RPM (RPM) หรือตัวแปรอื่นๆ ให้กับแต่ละค่าที่แก้ไข จะต้องกำหนดค่าเหล่านี้ไว้ก่อนหน้านี้ในบันทึก I (เพื่อให้โปรแกรมวิเคราะห์สามารถรับรู้ได้) ตัวอย่างเช่น:

ฉัน 04 3638 FXA 3940 SIU 4143 ENL 4446 RPM CR LF
สิ่งนี้แสดงให้เห็นว่าในแต่ละ บรรทัด บันทึก Bจะมีการบันทึกความแม่นยำในการแก้ไขระหว่างไบต์ 36 และ 38 ดาวเทียมที่ใช้งานอยู่ระหว่างไบต์ 39 และ 40 ระดับเสียงรบกวนของเครื่องยนต์ระหว่างไบต์ 41 และ 43 และ RPM ของเครื่องยนต์ระหว่างไบต์ 44 และ 46

บันทึก Bที่ได้จะกลายเป็น (พร้อมช่องว่างเพื่อความชัดเจนในตัวอย่างนี้):

BHH MM SS DD MMMMM N DDD MMMMM EV PPPPP GGGGG AAA SS NNN RRR CR LF"
บันทึก B - คำอธิบาย	รหัส	ขนาด	องค์ประกอบ	หมายเหตุ
แก้ไขความแม่นยำ	เอฟเอ็กซ์เอ	3 ไบต์	เอเอเอ	อักขระที่ถูกต้อง 0-9, เมตร, พารามิเตอร์บังคับหลังการแก้ไขครั้งที่ 4
ดาวเทียมที่ใช้งาน	ซิว	2 ไบต์	เอสเอส	อักขระที่ถูกต้อง 0-9
เสียงเครื่องยนต์	อีเอ็นแอล	3 ไบต์	เอ็นเอ็นเอ็น	อักขระที่ถูกต้อง 0-9
หมายเหตุ (Ian Forster-Lewis): ส่วนนี้ของเอกสารดูเหมือนจะมีข้อผิดพลาด - บันทึก B นี้ ควรมี RPM

4.2 บันทึกเหตุการณ์

บันทึก E ใช้เพื่อบันทึกเหตุการณ์เฉพาะในไฟล์ IGC ที่เกิดขึ้นในช่วงเวลาที่ไม่สม่ำเสมอ เหตุการณ์ดังกล่าวรวมถึงเหตุการณ์ที่นักบินเป็นผู้ริเริ่ม (รหัส PEV) หรือสำหรับเครื่องบันทึกที่ติดตั้งอุปกรณ์ตรวจจับความใกล้ชิด เหตุการณ์ที่ใกล้ชิดโดยใช้รหัสสามตัวอักษรที่เหมาะสมตามด้วยข้อมูลที่เหมาะสมตามที่กำหนดไว้ใน TLC ที่เหมาะสมในส่วนที่ 7บันทึก E จะถูกวางไว้หน้า บันทึก B แต่ละรายการ ในช่วงเวลาเดียวกันที่แสดงสถานที่และเวลาที่เหตุการณ์เกิดขึ้น เหตุการณ์ต้องมีรหัสสามตัวอักษร (TLC) จากส่วนที่ 7อาจใช้บันทึกเหตุการณ์มากกว่าหนึ่งรายการในเวลาเดียวกันได้ แต่เหตุการณ์ที่เริ่มต้นภายใน FR (ไม่ใช่โดยนักบิน) คาดว่าจะเกิดขึ้นเป็นครั้งคราวในประวัติเวลาของไฟล์การบิน และไม่ควรใช้สำหรับการสร้างบันทึกเพิ่มเติมทุกครั้งที่มีการแก้ไข สิ่งนี้อาจทำให้โปรแกรมวิเคราะห์ที่ออกแบบมาเพื่อใช้กับรูปแบบไฟล์นี้สับสน ซึ่งมักจะค้นหาและไฮไลต์บันทึกเหตุการณ์ หากผู้ผลิต FR ต้องการแทรกข้อมูลเพิ่มเติมในแต่ละการแก้ไข ควรทำผ่านส่วนขยายไปยังบันทึก Bโดยระบุรหัสข้อมูล (CCC) ในบันทึก I ก่อน (แก้ไข ( AL9 )

หากผู้ผลิตต้องการเพิ่มเหตุการณ์ประเภทใหม่ควรขอ รหัสสามตัวอักษรใหม่ ( ย่อหน้า 7 ) จาก GFAC ผู้ผลิตต้องระบุคำจำกัดความที่ชัดเจนของเหตุการณ์และรหัสที่เสนอ GFAC อาจตัดสินใจว่าข้อเสนอไม่ควรถือเป็นเหตุการณ์ แต่ควรรวมข้อมูลไว้ใน บันทึก B หรือ Kตามปกติสำหรับบันทึกเหล่านี้ โดยการระบุไว้ในบันทึก I และJ

รูปแบบของ E-Record ประกอบด้วยตัวระบุเรคคอร์ด เวลา TLC และสตริงข้อความ ตัวอย่างบางส่วนมีดังนี้:

อี 1 0 4 5 3 3 พีอีวี ซีอาร์ แอลเอฟ
บ 1 0 4 5 3 3 4 9 4 5 3 3 3 น 0 1 1 3 2 4 4 4 EA 0 1 3 5 7 0 1 5 0 1 CR LF
สิ่งนี้ระบุถึงเหตุการณ์ที่ริเริ่มโดยนักบิน (PEV) ในเวลา 10:45:33 UTC และบันทึก B ที่เกี่ยวข้อง แสดงตำแหน่ง 49:45.333 N 11:32.444 E ที่ระดับความสูงของความกดอากาศ 1,357 เมตร และระดับความสูงของ GNSS 1,501 เมตร

เหตุการณ์บางอย่างต้องการมากกว่าแค่ TLC เพื่อการตีความ:

อี 1 0 4 5 4 4 เอทีเอส 1 0 2 3 1 2 ซีอาร์ แอลเอฟ
การตั้งค่าเครื่องวัดความสูงในอุปกรณ์แสดงผลที่เชื่อมต่อกับ FR ถูกเปลี่ยนเป็น 1023.12 hPa เมื่อเวลา 10:45:44 น.

อี 1 0 4 5 5 5 อีออน ซีอาร์ แอลเอฟ
B 1 0 4 5 5 5 4 9 4 5 3 3 3 N 0 1 1 3 2 4 4 4 EA 0 1 3 3 7 0 1 5 6 7 CR LF
เครื่องยนต์เปิดอยู่ (EON) เวลา 10:45:55 UTC และบันทึก Bแสดงตำแหน่ง 49:45.333 N 11:32.444 E ที่ระดับความสูงความกดอากาศ 1,337 เมตร และระดับความสูง GNSS 1,567 เมตร

อี 1 0 4 7 3 3 ซีจีดี 1 0 3 ซีอาร์แอลเอฟ
ข้อมูลภูมิสารสนเทศถูกเปลี่ยนเป็น Bessel (หมายเลข IGC 103 ดูย่อหน้า 8) เมื่อเวลา 10:47:33 น. UTC ซึ่งจะทำให้การบันทึกข้อมูลสำหรับวัตถุประสงค์ IGC ไม่ถูกต้อง ซึ่งต้องใช้ WGS84

4.3 F RECORD - กลุ่มดาวเทียม

นี่เป็นบันทึกบังคับอย่างไรก็ตาม ไม่จำเป็นต้องอัปเดตบันทึก F ในช่วงเวลาน้อยกว่า 5 นาที เพื่อป้องกันการเปลี่ยนแปลงชั่วคราวของดาวเทียมที่ได้รับเนื่องจากการเปลี่ยนมุมเอียง การบินในหุบเขา ฯลฯ ไม่ให้ทำให้เกิดเส้นบันทึก F บ่อยครั้ง สำหรับระบบ GPS ของสหรัฐอเมริกา รหัสดาวเทียมสำหรับดาวเทียมแต่ละดวงคือ PRN ของดาวเทียมที่ต้องการ สำหรับระบบดาวเทียมอื่นๆ รหัสจะถูกกำหนดโดย GFAC ตามความจำเป็น ในกรณีที่ใช้ข้อมูล NMEA ภายในบันทึก F ควรนำรหัสมาจากประโยค GSA ที่ระบุรหัสของดาวเทียมที่ใช้ในการกำหนดจุด ซึ่งบันทึกไว้ในบันทึกBบันทึก F จะไม่ถูกบันทึกอย่างต่อเนื่อง แต่จะบันทึกในช่วงเริ่มต้นของการกำหนดจุด และจะบันทึกเฉพาะเมื่อตรวจพบการเปลี่ยนแปลงของดาวเทียมที่ใช้ ( AL4 )

รูปแบบของบันทึก F:
ฟ เอช ​​เอ็ม ดับเบิ้ลยู เอส เอส เอ เอ บี บี ซีซี ดีดี อี เอฟ จี จี อาร์ เอฟ เอฟ
F record - คำอธิบาย	ขนาด	องค์ประกอบ	หมายเหตุ
เวลา UTC	6 ไบต์	ฮึ่มมมส์	อักขระที่ถูกต้อง 0-9
รหัสดาวเทียม	2 ไบต์ต่อดาวเทียมหนึ่งดวงที่ใช้	AABBCC หรือ 01, 02 เป็นต้น	อักขระที่ถูกต้องคือตัวอักษรและตัวเลข
การบันทึก 4.4 K - ข้อมูลที่ต้องการน้อยกว่าการแก้ไข

เรคคอร์ด K ใช้สำหรับข้อมูลที่อาจต้องการน้อยกว่าเรคคอร์ด B ที่กำหนดไว้ เรคคอร์ด K ควรมีช่วงเวลาเริ่มต้นที่ 20 วินาที ตัวอย่างเช่น หากเรคคอร์ดBบันทึกทุก 5 วินาที เรคคอร์ด K สามารถตั้งค่าให้บันทึกทุก 20 วินาทีได้ เช่น บันทึกส่วนหัวจริง (HDT) เนื้อหาของเรคคอร์ด K จะแสดงอยู่ในเรคคอร์ดJ เรคคอร์ด Jต่อไปนี้ระบุข้อมูลในเรคคอร์ด K ในบรรทัดถัดไป:

เจ 0 8 1 2 เอชดีที ซีอาร์ แอลเอฟ
KHHMMSS 0 0 0 9 0 CR LF
บันทึก K นี้ระบุว่าหัวเรื่องที่แท้จริง (TLC = HDT) คือ 090 (ตะวันออก)

4.5 L RECORD - LOG BOOK/COMMENTSสามารถวาง L-Record ไว้ที่ใดก็ได้ในไฟล์หลังจาก H, I และ J records แต่ก่อนG record L-Record อนุญาตให้เพิ่มบรรทัดข้อความรูปแบบอิสระหลายบรรทัดลงในบันทึกข้อมูลการบินได้ตลอดเวลาในลำดับเวลา แม้ว่าตัวบันทึกนี้จะไม่ได้ประทับเวลาไว้ก็ตาม สามารถเริ่มต้นโดยโปรแกรมใน FR โดยนักบินหรือผู้สังเกตการณ์อย่างเป็นทางการ และคำว่า "comment record" อาจอธิบายได้ชัดเจนกว่า "logbook" ควรใช้รหัสสามตัวอักษรของผู้ผลิต FR (ย่อหน้า 2.5) ในกรณีที่ข้อมูลเริ่มต้นโดย FR และในกรณีนี้ผู้ผลิตควรระบุวิธีการตีความ L-Record ประเภทนี้เพื่อประโยชน์ของผู้เขียนซอฟต์แวร์สำหรับรูปแบบ IGC ในกรณีอื่นๆ ช่องนี้ (MMM ด้านล่าง) จะเป็นช่องว่างสามช่องเช่นกัน โดยนักบิน (รหัส PLT) หรือ OO (OOI) ตามที่กำหนด ในกรณีของเที่ยวบินฟรีที่นักบินอ้างสิทธิ์จุดอ้างอิงหลังการบิน จะใช้รหัส PFC (Post-Flight Claim) ตามด้วยจุดอ้างอิงในรูปแบบเดียวกับC Record (Pre-flight declaration) คาดว่าข้อมูลนี้จะถูกแทรกโดยโปรแกรมซอฟต์แวร์ (เช่น หลังจากถ่ายโอนข้อมูลการบินไปยังคอมพิวเตอร์ทันทีหลังการบิน โดยโปรแกรมภายนอก FR) แทนที่จะเพิ่มด้วยตนเอง เพื่อให้ข้อมูลอยู่ในรูปแบบที่ถูกต้องและสามารถรับรู้ได้โดยโปรแกรมวิเคราะห์ที่ออกแบบมาเพื่ออ่านข้อมูล Post-Flight Claim และแสดงเที่ยวบินบนหน้าจอพร้อมกับจุดอ้างอิง PFC โปรดทราบว่าบันทึก L เมื่อสร้างโดยนักบินหรือ OO จะต้องไม่ส่งผลกระทบต่อการตรวจสอบ VALI สำหรับข้อมูลไฟล์ที่เหลือ รูปแบบของบันทึก L มีดังนี้: ( AL5 )

L MMM สตริงข้อความ CR LF
L PLT TEXTSTRING CR LF
L PFC ข้อความเป็น C บันทึก CR LF
L record - คำอธิบาย	ขนาด	องค์ประกอบ	หมายเหตุ
ข้อมูลผู้ผลิต	3 ไบต์	เอ็มเอ็มเอ็ม	รหัสของผู้ผลิต ดูข้อ 2.5
อินพุตของนักบิน	3 ไบต์	พีแอลที	สตริงข้อความหลัง PLT
อินพุต OO	3 ไบต์	โอไอ	สตริงข้อความหลัง OOI
หลังจากนักบินป้อนข้อมูลเที่ยวบิน	3 ไบต์	พีเอฟซี	สำหรับเที่ยวบินฟรีหลังเที่ยวบินเลือกหลักสูตร
บันทึก L ที่มีรหัส MMM ของผู้ผลิต FR จะต้องรวมอยู่ในลายเซ็นดิจิทัล (ระบบรักษาความปลอดภัย) ของไฟล์ บันทึก L อื่นๆ (เช่น บันทึกที่ใส่โดยนักบิน (PLT) หรือ OO (OOI)) จะไม่ครอบคลุมอยู่ในลายเซ็นดิจิทัลของไฟล์ โปรดดูย่อหน้าที่ 3.2 ตัวอย่างของอินพุตนักบิน:

LPLT เที่ยวบินนี้เป็นความพยายามครั้งที่สองของฉันในการบิน 1,000 กม.
LPLT จากสนามอีเกิลฟิลด์
4.6 D RECORD - ระบบ GPS เชิงอนุพันธ์

สิ่งนี้บ่งชี้ว่ากำลังใช้ GPS แบบดิฟเฟอเรนเชียล และสามารถบันทึกแบบหลายอินสแตนซ์ได้ หากระหว่างการบินมีการใช้บีคอนแบบดิฟเฟอเรนเชียลมากกว่าหนึ่งตัว บันทึกนี้จะถูกวางไว้ในไฟล์ IGC ก่อนบันทึก B แรก หลังจาก บันทึก H , I , JและCรูปแบบของบันทึก D มีดังนี้ ( AL8 )

DQSSSS CR LF
L record - คำอธิบาย	ขนาด	องค์ประกอบ	หมายเหตุ
ตัวระบุ GPS	1 ไบต์	คิว	ใช้ 1=GPS, 2=DGPS
รหัสสถานี DGPS	4 ไบต์	สสสส	 
พารามิเตอร์เหล่านี้สอดคล้องกับการระบุคุณภาพ GPS ของ NMEA GGA การไม่มีบันทึก Dแสดงว่าไม่ได้ใช้ GPS แบบดิฟเฟอเรนเชียล การใช้งาน DGPS ใดๆ จะต้องได้รับการอนุมัติจาก GFAC และต้องแสดงให้เห็นว่าการใช้ GPS ช่วยรักษาความสมบูรณ์ของข้อมูลละติจูด/ลองจิจูดพื้นฐานและข้อมูลการบินอื่นๆ

5. คำจำกัดความ

ความเร็วอากาศ - ความเร็วอากาศจริงของเครื่องบินเป็นกิโลเมตรต่อชั่วโมง สำหรับระบบที่มีข้อมูลอากาศป้อนเข้า
ตัวอักษรและตัวเลข - อักขระตัวอักษรและ/หรือตัวเลขที่ถูกต้องจากรายการอักขระที่ถูกต้อง (ย่อหน้าที่ 6)
ระดับการแข่งขัน - ระดับการแข่งขัน IGC/FAI ของเครื่องบิน
กลุ่มดาว - ดาวเทียมที่แม่นยำซึ่งใช้ข้อมูลเพื่อกำหนดจุด GNSS ซึ่งอาจใช้เพื่อตรวจสอบความถูกต้องของข้อมูลการบิน
เส้นทาง - ทิศทางระหว่างสองจุดแสดงเป็นองศาแม่เหล็กหรือองศาจริง
ข้อมูลอ้างอิง - ข้อมูลอ้างอิง GNSS (ระบบพิกัด) ที่ใช้งานอยู่
เครื่องยนต์ดับ - ระบบขับเคลื่อน (MoP) (เช่น เครื่องยนต์และใบพัด) ถูกเก็บไว้และไม่อยู่ในตำแหน่งที่จะสร้างแรงขับ ระดับ
เสียงรบกวนเครื่องยนต์ (ENL) - เสียงแวดล้อมที่ FR แสดงเป็นตัวเลขสามตัว สูงสุด 999 พารามิเตอร์ที่บันทึกอย่างต่อเนื่องนี้จะบันทึกระดับพื้นฐานเป็นบวก (กล่าวคือ ไม่ใช่ระดับศูนย์) แม้ว่า MoP จะไม่ได้ทำงาน และทำให้สามารถตรวจสอบความสมบูรณ์ของระบบบันทึก MoP ได้อย่างต่อเนื่อง
เครื่องยนต์ดับ - ระบบขับเคลื่อน (MoP) อยู่ในสภาวะที่ไม่สามารถสร้างแรงขับได้
เครื่องยนต์เปิด - ระบบขับเคลื่อน (MoP) อยู่ในสภาวะที่สามารถสร้างแรงขับได้
รอบเครื่องยนต์ - เป็นพารามิเตอร์ที่เกี่ยวข้องกับรอบเครื่องยนต์ ดูรหัส 3 ตัวอักษร RPM
เครื่องยนต์ขึ้น - เสาส่งกำลังของชุดขับเคลื่อนยื่นออกมา หรือประตูเครื่องยนต์หรือใบพัดเปิดอยู่ ในสภาวะที่สามารถสร้างแรงขับได้เมื่อสตาร์ทเครื่องยนต์
เหตุการณ์อุปกรณ์ - เหตุการณ์เหล่านี้สร้างขึ้นโดย FR เท่านั้น (เช่น การตรวจจับการขึ้นบิน) ตรงกันข้ามกับเหตุการณ์ที่สร้างขึ้นหลังจากการบินโดยการวิเคราะห์ข้อมูลการบินของ FR (เช่น การสร้างสถานะในเขตสังเกตการณ์จุดเลี้ยว หรือการข้ามเส้นเริ่มต้นหรือเส้นชัย)	
เสร็จสิ้น - จุดสิ้นสุดของภารกิจ เช่น การข้ามเส้นชัย การเข้าสู่เขตสังเกตการณ์เส้นชัย หรือ (สำหรับเที่ยวบินระยะทางบางเที่ยว) การลงจอด คำจำกัดความ รหัสกีฬา (SC3) ปริมาตรหลัก
ความแม่นยำของจุดคงที่ - ความแม่นยำของจุดคงที่ที่เกี่ยวข้อง แสดงเป็น EPE เป็นเมตร โดยปกติมีความน่าจะเป็น 2 ซิกมา (95.45%) ดู EPE ในอภิธานศัพท์
หมายเลขประจำเครื่อง fr - ตัวอักษรและตัวเลขสามตัวที่ไม่ซ้ำกันใน FR ทุกประเภทจากผู้ผลิตนั้น และกำหนดโดยผู้ผลิตเพื่อระบุ FR แต่ละเครื่อง ใช้ในบันทึกแรก (A) (ดูภาคผนวกนี้ ย่อหน้า 3.1) และในชื่อไฟล์ IGC (ย่อหน้า 2.5)
รหัสเครื่องร่อน - ตัวอักษรและตัวเลขสำหรับการลงทะเบียนเฉพาะของเครื่องบินแต่ละลำ
ประเภทเครื่องร่อน - ผู้ผลิตและหมายเลขรุ่นที่แน่นอนของเครื่องบิน
ระดับความสูง gnss - กลุ่มอักขระตัวเลขห้าตัวที่ระบุระดับความสูง GNSS เป็นเมตรเหนือทรงรี
การเชื่อมต่อ gnss - ในกรณีที่ใช้หน่วย GNSS แยกต่างหาก จะแสดงการเชื่อมต่อ GNSS กับโมดูล FR
การเชื่อมต่อ gnss - ในกรณีที่ใช้หน่วย GNSS แยกต่างหาก จะแสดงการตัดการเชื่อมต่อ GNSS จากโมดูล FR
ความเร็วภาคพื้นดิน - ความเร็วเหนือพื้นดินเป็นกิโลเมตรต่อชั่วโมง
ทิศทาง - ทิศทางที่เครื่องบินชี้ (แกนตามยาว) เป็นองศาจริงหรือองศาแม่เหล็ก
ละติจูด - กลุ่มตัวอักษรและตัวเลขเจ็ดตัวอักษร แสดงเป็นสองตัวเลขแทนองศา สองตัวเลขแทนนาที และสามตัวเลขแทนเลขทศนิยมสิบ หนึ่งร้อย และหนึ่งพันของนาที ตามด้วยอักขระ N หรือ S ในกรณีที่แทรกค่านี้ลงใน FR เช่น เป็นส่วนหนึ่งของการประกาศเที่ยวบิน อักขระ N/S ต้องสามารถป้อนได้ทั้งตัวพิมพ์ใหญ่และตัวพิมพ์เล็ก สำหรับวัตถุประสงค์ของ IGC ละติจูด/ลองจิจูดต้องอ้างอิงถึงข้อมูลภูมิสารสนเทศ WGS84
ลองจิจูด - กลุ่มตัวอักษรและตัวเลขแปดตัว แสดงเป็นตัวเลขสามตัวสำหรับองศา สองตัวสำหรับนาที และสามตัวสำหรับเลขทศนิยมสิบ หนึ่งร้อย และหนึ่งพันของนาที ตามด้วยอักขระ E หรือ W ในกรณีที่แทรกค่านี้ลงใน FR เช่น เป็นส่วนหนึ่งของการประกาศเที่ยวบิน อักขระ N/S จะต้องสามารถป้อนเป็นตัวพิมพ์ใหญ่หรือตัวพิมพ์เล็กได้ สำหรับวัตถุประสงค์ของ IGC ละติจูด/ลองจิจูดต้องอ้างอิงกับข้อมูลภูมิสารสนเทศ WGS84	
on task - นักบินกำลังพยายามทำภารกิจ
oo id - ชุดตัวอักษรและตัวเลขที่นักบิน OO ป้อนลงใน FR ก่อนทำการบิน ประกอบด้วยอักขระอย่างน้อยสี่ตัวและเป็นความลับของนักบิน
photo - มีการถ่ายภาพ เช่น ภาพจุดเลี้ยว
Pilot Event (รหัส PEV) - เมื่อนักบินได้ทำเครื่องหมายเวลาเฉพาะไว้ ซึ่งอาจหมายถึงเหตุการณ์หรือเหตุการณ์ต่างๆ ที่แตกต่างกัน เช่น การข้ามเส้นเริ่มต้น (หรือการทำเครื่องหมายความตั้งใจที่จะข้ามในอีกไม่ช้า) หรือการมาถึง ณ จุดใดจุดหนึ่ง ลำดับการแก้ไขอย่างรวดเร็วมีดังนี้ (ย่อหน้า 2.6.7.3) ( AL8 )
pressure altitude - กลุ่มตัวเลขห้าชุดที่ระบุค่า pressure altitude เป็นเมตรเหนือระดับน้ำทะเล 1013.25 HPa และ ICAO ISA ข้างต้น
raim - Receiver Autonomous Integrity Monitoring (เมื่อใช้) - ใช้เพื่อระบุคุณภาพของข้อมูลการนำทาง GNSS โปรดดูส่วนอภิธานศัพท์
ส่วนขยายบันทึก - อนุญาตให้เพิ่มข้อมูลเพิ่มเติมลงในบันทึกข้อมูลแบบคงที่ (B) และแบบขยาย (K)
ข้อมูลความปลอดภัย (ลายเซ็นดิจิทัล) - ใช้เพื่อตรวจสอบว่าข้อมูลการบินไม่มีการเปลี่ยนแปลงระหว่างหรือหลังจากเที่ยวบิน
เริ่มต้น - การเริ่มต้นของการแสดงการบินอย่างเป็นทางการ สำหรับคำจำกัดความ โปรดดู Sporting Code (SC3)
ข้อมูลเพิ่มเติม แก้ไข - การใช้ข้อมูลภายนอกที่ไม่ใช่ดาวเทียมเพื่อช่วยหน่วย GNSS กำหนดตำแหน่ง เช่น
งาน ส่งสัญญาณภาคพื้นดิน - จุดสำคัญของเที่ยวบินที่ตั้งใจไว้ โดยปกติคือจุดเริ่มต้น จุดเลี้ยว และจุดสิ้นสุดที่ตั้งใจไว้
พลังงานรวม ระดับความสูง - การรวมกันของศักย์ของเครื่องร่อนและพลังงานจลน์ที่แสดงเป็นเมตรของระดับความสูงจริง
เส้นทาง - เส้นทางจริง (เส้นทางการบิน) เหนือพื้นดินที่เครื่องบินบินได้
การตรวจสอบจุดเลี้ยว - หลักฐานการปรากฏตัวในเขตสังเกตการณ์ที่เกี่ยวข้องสำหรับจุดที่เกี่ยวข้อง
6. อักขระที่ถูกต้อง
อักขระเหล่านี้ประกอบด้วยอักขระ ASCII ที่พิมพ์ได้ทั้งหมดตั้งแต่เลขฐานสิบหก 20 ถึงเลขฐานสิบหก 7E ยกเว้นอักขระที่สงวนไว้ในตารางด้านล่าง สตริงข้อความคือลำดับของอักขระที่ถูกต้อง ตารางต่อไปนี้แสดงอักขระก่อน จากนั้นจึงแสดงรหัสเลขฐานสิบหก และตารางที่สองแสดงข้อมูลเดียวกันตามลำดับเลขฐานสิบหก:

ตัวเลข	จดหมาย	สัญลักษณ์
Res = สงวนไว้	
ตัวอักษรสงวน
ตัวพิมพ์ใหญ่	ตัวพิมพ์เล็ก

0 = เลขฐานสิบหก 30
1 = 31
2 = 32
3 = 33
4 = 34
5 = 35
6 = 36
7 = 37
8 = 38
9 = 39	
A = เลขฐานสิบหก 41
B = 42
C = 43
D = 44
E = 45
F = 46
G = 47
H = 48
I = 49
J = 4A
K = 4B
L = 4C
M = 4D	
ยังไม่มีข้อความ = 4E
O = 4F
P = 50
Q = 51
R = 52
S = 53
T = 54
U = 55
V = 56
W = 57
X = 58
Y = 59
Z = 5A	
a = เลขฐานสิบหก 61
b ​​= 62
c = 63
d = 64
e = 65
f = 66
g = 67
h = 68
i = 69
j = 6A
k = 6B
l = 6C m
= 6D	
n = 6E
o = 6F
p = 70
q = 71
r = 72
s = 73
t = 74
u = 75
v = 76
w = 77
x = 78
y = 79
z = 7A	
ช่องว่าง = Hex 20
Res = 21
" = 22
# = 23
Res = 24
% = 25
& = 26
' = 27
( = 28
) = 29
@ = 40
` = 60
Res = 2A
+ = 2B
Res = 2C
- = 2D
. = 2E	
, = 2C
/ = 2F
: = 3A
; = 3B
< = 3C
= = 3D
> = 3E
? = 3F
[ = 5B
ความละเอียด = 5C
] = 5D
ความละเอียด = 5E
_ = 5F
{ = 7B
| = 7C
} = 7D
ความละเอียด = 7E	
CR = 0D
LF = 0A
$ = 24
* = 2A
! = 21
\ = 5C
^ = 5E
~ = 7E
อักขระเหล่านี้ถูกสงวนไว้ (ห้ามใช้) เนื่องจากอาจทำให้เกิดความสับสนหากใช้ในสตริงข้อความ เช่น เนื่องจากความหมายอื่นหรือการกดแป้นพิมพ์อื่น
7. รหัสสามตัวอักษร (TLC)
สิ่งเหล่านี้จะแสดงเป็น CCC ในรูปแบบก่อนหน้าในภาคผนวกนี้ ความหมายของสิ่งเหล่านี้แสดงไว้ด้านล่างพร้อมกับบันทึกในไฟล์ IGC ที่สามารถใช้งานได้ หากผู้ผลิตต้องการเพิ่มเหตุการณ์ประเภทใหม่ ควรขอ TLC ใหม่จาก GFAC ผู้ผลิตควรให้คำจำกัดความที่ชัดเจนของเหตุการณ์และรหัสที่เสนอ

รหัส	จดหมายบันทึก TLC ใช้กับ	ความหมายของ TLC พร้อมหมายเหตุการใช้งาน
เอซีเอ็กซ์
เอซี
วาย เอซีแซด	ฉัน , บี	ความเร่งเชิงเส้นในแกน X, Y และ Z สำหรับเครื่องบินผาดโผนที่ติดตั้งเซ็นเซอร์ที่เหมาะสมซึ่งส่งไปยังเครื่องบันทึกและไฟล์ IGC X = ตามยาว, Y = ตามขวาง, Z = แนวตั้ง (เรียกว่า "G")
ANX
ANY
ANZ	ฉัน , บี	ความเร่งเชิงมุมในแกน X, Y และ Z สำหรับเครื่องบินผาดโผนที่ติดตั้งเซ็นเซอร์ที่เหมาะสมซึ่งป้อนไปยังเครื่องบันทึกและไฟล์ IGC ระยะพิทช์ = X, ม้วน = Y, หัน = Z หน่วยเป็นองศาต่อวินาที
เอโอพี เอ
โออาร์	ฉัน , บี	มุมเอียง มุมเอียงเอียง/มุมเอียงเป็นองศา (สำหรับมุมจมูกคว่ำหรือมุมเอียงซ้าย ให้เริ่มด้วย "-") (AL8)
เอทีเอส	เขา​​	การตั้งค่าความดันของเครื่องวัดความสูงเป็นหน่วยเฮกโตปาสกาล โดยมีตัวเลข 4 ตัวและจุดทศนิยมหนึ่งตำแหน่ง (เช่น 1013.2, 0995.7) แม้ว่าการตั้งค่าความดันของเครื่องวัดความสูงอาจถูกบันทึกไว้ (เช่น เมื่อ FR ส่งข้อมูลไปยังจอแสดงผลในห้องนักบิน) แต่ห้ามใช้เพื่อเปลี่ยนระดับความสูงของความดันที่บันทึกในแต่ละจุด ซึ่งต้องคงไว้ตามข้อมูลอ้างอิงระดับน้ำทะเล ISA ที่ 1013.25 มิลลิบาร์ ตลอดเวลา ( AL8 )
ที่	ชม	ระบบ GNS BeiDou 2 จากสาธารณรัฐประชาชนจีน
บีเอฟไอ	ชม	เครื่องมือบินแบบตาบอด บันทึกเป็น ON หรือ OFF ในรูปแบบ BFION หรือ BFIOFF ตามด้วยช่องว่าง ตามด้วย AH (Artificial Horizon) สำหรับเครื่องมือที่แสดงเส้นขอบฟ้า หรือ TI (Turn Indicator) สำหรับเครื่องมือที่แสดงอัตราการเลี้ยว การเปลี่ยนทิศทาง หรืออื่นๆ ที่คล้ายกัน หากสถานะ ON/OFF ไม่แน่นอน ให้ใช้รูปแบบ BFIUN (สำหรับสถานะที่ไม่ทราบ) อาจมีสตริงข้อความ (ไม่บังคับ) ต่อท้ายเพื่อให้รายละเอียดเพิ่มเติมเกี่ยวกับเครื่องมือและสถานะ สถานะเริ่มต้นจะถูกรายงานในระเบียน E ณ เวลาที่บันทึก B แรกในไฟล์ IGC โดยตั้งค่าไบต์ Fix Validity เป็น A (3D Fix ดูตาราง A4.1.2 ภายใต้ Fix Validity)
ซีซีแอล	ชม	ระดับการแข่งขัน
ซีซีเอ็น	และ	การเชื่อมต่อกล้อง
ซีซีโอ	เจ , เค	เส้นทางเข็มทิศ (จากเซ็นเซอร์เข็มทิศของเครื่องบิน) ตัวเลขสามตัวที่คำนวณจากองศาตามเข็มนาฬิกาจาก 000 ทิศเหนือ ( AL8 )
CDC	และ	การตัดการเชื่อมต่อกล้อง
ซีจีดี	และ	การเปลี่ยนแปลงข้อมูลอ้างอิงทางภูมิศาสตร์
ตำรวจสันติบาล	ชม	รหัสการแข่งขัน
คลับ	ชม	สโมสรหรือองค์กร และประเทศที่บินหรือดำเนินการ (เช่น Elmira สหรัฐอเมริกา, Lasham สหราชอาณาจักร) สำหรับประเทศ ให้ใช้รหัสสองตัวอักษร ISO 3166 ซึ่งบางส่วนระบุไว้ในวรรค3.3.3ของภาคผนวก A
ซีเอ็ม2	ชม	ชื่อลูกเรือคนที่สอง นามสกุล (ชื่อจริง) ตามด้วยชื่อ (ตามที่กำหนด) (รูปแบบเดียวกับ PLT สำหรับนักบินผู้รับผิดชอบ) สำหรับเครื่องบินที่มีลูกเรือมากกว่าสองคน ให้ใช้ CM3 และอื่นๆ หากจำเป็น ( AL8 )
คอต	เจ , เค	ตัวควบคุมอุณหภูมิ (เช่น สำหรับ FES) เป็นองศาเซลเซียส AL5
เคิร์ก	เจ , เค	กระแสไฟฟ้า, แอมแปร์. AL5
ซียู1	เจ , เค	กระแสไฟฟ้า แอมแปร์ของแบตเตอรี่ขับเคลื่อนตัวแรกที่มีการติดตั้งแบตเตอรี่ 2 ก้อน (AL8)
ซียู2	เจ , เค	กระแสไฟฟ้า แอมแปร์ของแบตเตอรี่ขับเคลื่อนตัวที่สองที่ติดตั้งแบตเตอรี่ 2 ก้อน (AL8)
วัน	ฉัน , บี , เจ , เค	การกระจัดทิศตะวันออก เมตร สำหรับทิศตะวันตกใช้เครื่องหมายลบ
และ	ฉัน , บี , เจ , เค	การกระจัดทิศเหนือ เมตร สำหรับทิศใต้ใช้เครื่องหมายลบ
ดีบี1	ชม	วันเดือนปีเกิดของนักบินผู้ควบคุม (ผู้บังคับเครื่องบิน) ในบรรทัดก่อนหน้าของ บันทึก H (DDMMYY) ( AL8 )
ดีบี2	ชม	วันเกิดของลูกเรือคนที่สองในรูปแบบ DDMMYY สำหรับเครื่องบินที่มีลูกเรือมากกว่าสองคน ให้ใช้ DB3 และอื่นๆ หากจำเป็น ( AL8 )
วันเกิด	ชม	รหัสล้าสมัย ตอนนี้ใช้ DB1 วันเกิดของนักบินในบรรทัดก่อนหน้าของบันทึก H (DDMMYY) ( AL8 )
ดีทีอี	ชม	วันที่ แสดงเป็น DDMMYY DTM H Geodetic Datum ที่ใช้บันทึกละติจูด/ลองจิจูด (สำหรับวัตถุประสงค์ของ IGC ต้องตั้งค่าเป็น WGS84)
อีดีเอ็น	และ	เครื่องยนต์ดับ ดูหมายเหตุในบรรทัดสำหรับ EON
อีเอ็นแอล	ฉัน , บี	ระดับเสียงเครื่องยนต์ บันทึกตั้งแต่ 000 ถึง 999 นี่เป็นวิธีการบันทึก MoP ที่ต้องการเนื่องจากไม่ต้องใช้สายเคเบิลหรือเซ็นเซอร์ภายนอก FR และสามารถยืนยันตัวเองได้ โดยบันทึกค่าบวกในการแก้ไขแต่ละครั้ง
อีโอเอฟ	และ	เครื่องยนต์ดับ ดูหมายเหตุในบรรทัดสำหรับ EON
กัป	และ	เครื่องยนต์ติด หมายเหตุ: หากไม่ได้ใช้ ENL หรือ RPM เป็นตัวบ่งชี้หลักของการทำงานของ MoP ให้ใช้บันทึกเหตุการณ์และรหัส EON/EOF หรือ EUP/EDN อาจใช้วิธีทั้งสองวิธีร่วมกันได้ เช่น EON/EOF อิงตามพารามิเตอร์ต่างๆ เช่น การเปิด/ปิดจุดระเบิด, กำลังไฟฟ้าออกต่ำสุดของเครื่องกำเนิดไฟฟ้า, EUP/EDN สำหรับประตูห้องเครื่องยนต์เปิด/ปิด หรือการเปิด/ปิดเสาเครื่องยนต์ขึ้น/ลง บวกกับ RPM อิงตามรอบเครื่องยนต์หรือใบพัด หรือENLสำหรับระดับเสียงที่ด้านหน้า
อียูพี	และ	เครื่องยนต์กำลังขึ้น ดูหมายเหตุบนบรรทัดสำหรับ EON
จบ	และ	เสร็จ
เฟล	เจ , เค	ระดับน้ำมันเชื้อเพลิง เซ็นติลิตร AL5
เอฟเอฟแอล	เจ , เค	อัตราการไหลของเชื้อเพลิง ลิตรต่อนาที (AL8)
เอฟแอลพี	และ	ตำแหน่งแฟลป อักขระสามตัว เช่น FLP060 สำหรับแฟลปด้านบวก 60 องศา หากเป็นลบ ให้ใช้เครื่องหมายลบนำหน้าตัวเลข เช่น FLP-20 สำหรับแฟลปด้านลบ 20 องศา ( AL8 )
เอฟอาร์เอส	ชม	ระบบรักษาความปลอดภัยของเครื่องบันทึกการบิน ใช้สำหรับกรณีที่ตรวจพบข้อบกพร่องด้านความปลอดภัย เช่น ระบบรักษาความปลอดภัยภายในเครื่องบันทึกการบิน (ไมโครสวิตช์) ทำงาน ( AL6 )
เอฟทีวาย	ชม	ประเภท FR (ชื่อผู้ผลิต, หมายเลขรุ่น FR)
เอฟเอ็กซ์เอ	ฉัน , บี , เจ , เค	ความแม่นยำคงที่ เมื่อใช้ในบันทึก B (fix)นี่คือตัวเลข EPE (Estimated Position Error) เป็นเมตร (MMMM) สำหรับจุดที่กำหนดแต่ละจุด โดยมีความน่าจะเป็น 2-Sigma (95.45%) ( AL8 )
เอฟเอ็กซ์เอ	ชม	หมวดหมู่ความแม่นยำของข้อมูลคงที่ เมื่อใช้ในบันทึกส่วนหัว จะเป็นตัวบ่งชี้ทั่วไปถึงความแม่นยำของการแก้ไขที่อาจเกิดขึ้น และระบุหมวดหมู่ของความสามารถของเครื่องรับ แทนที่จะเป็นตัวเลขที่แน่นอน เช่น ตัวเลขที่ใช้กับการแก้ไขแต่ละรายการที่บันทึกไว้ในบันทึก B, I, J หรือ K (ดูด้านบน) หากมีข้อสงสัย ให้ใช้กลุ่มตัวเลขสามหลักในหน่วยเมตร ซึ่งอ้างอิงถึงรัศมี EPE ทั่วไปที่เครื่องรับทำได้ในสภาพการรับสัญญาณที่ดี ( AL3 )
กัล	ชม	กาลิเลโอ (ระบบ GNSS ของยุโรป) ตามด้วยผู้ผลิตเครื่องรับ ประเภท และตัวอักษร/หมายเลขรุ่น ดู3.3.1ข้างต้น ( AL11 )
จีซีเอ็น	และ	GNSS (โมดูลแยก) เชื่อมต่อ
จีดีซี	และ	GNSS (โมดูลแยก) ตัดการเชื่อมต่อ
จีไอดี	ชม	รหัสเครื่องร่อน
เชื่อ	ชม	GLONASS (ระบบ GNSS ของรัสเซีย) ตามด้วยผู้ผลิตเครื่องรับ ประเภท และตัวอักษร/หมายเลขรุ่น ดู3.3.1ข้างต้น ( AL11 )
จีพีเอส	ชม	GPS (ระบบ GNSS ของสหรัฐอเมริกา) ตามด้วยผู้ผลิตเครื่องรับ ประเภท และตัวอักษร/หมายเลขรุ่น ดู3.3.1ข้างต้น ( AL11 )
จีเอสพี	ฉัน , บี , เจ , เค	ความเร็วภาคพื้นดิน สามตัวเลขเป็นกิโลเมตรต่อชั่วโมง ( AL8 )
จีทีวาย	ชม	ประเภทเครื่องร่อน, ผู้ผลิต, รุ่น
เอชดีเอ็ม	ฉัน , บี , เจ , เค	ทิศทางแม่เหล็ก สามตัวเลขตามองศาตามเข็มนาฬิกาจาก 000 สำหรับทิศเหนือ ( AL8 )
เอชดีที	ฉัน , บี , เจ , เค	หัวข้อจริง สามตัวเลขตามองศาตามเข็มนาฬิกาจาก 000 สำหรับทิศเหนือ ( AL8 )
ไอเอเอส	ฉัน , บี , เจ , เค	ความเร็วอากาศ สามตัวเลขเป็นกิโลเมตรต่อชั่วโมง ( AL8 )
เจพีที	เจ , เค	อุณหภูมิท่อไอพ่น สำหรับเครื่องยนต์ไอพ่น AL5
ฮัม	เจ , เค	ความชื้นสัมพัทธ์, เปอร์เซ็นต์ (AL8)
เลบ	เจ , เค	แบตเตอรี่ - สถานะการชาร์จ, เปอร์เซ็นต์ AL5
เล1	เจ , เค	แบตเตอรี่ 1 - สถานะการชาร์จ เปอร์เซ็นต์ แบตเตอรี่ขับเคลื่อนก้อนแรกที่ติดตั้งแบตเตอรี่ 2 ก้อน (AL8)
เลทู	เจ , เค	แบตเตอรี่ 2 - สถานะการชาร์จ เปอร์เซ็นต์ แบตเตอรี่ขับเคลื่อนตัวที่สองที่ติดตั้งแบตเตอรี่ 2 ก้อน (AL8)
แอลเอดี	ฉัน , บี	ตำแหน่งสุดท้ายของนาทีทศนิยมของละติจูด ซึ่งละติจูดจะถูกบันทึกด้วยความแม่นยำมากกว่าสามนาทีทศนิยมที่อยู่ในเนื้อหาหลักของเรกคอร์ด Bตำแหน่งนาทีทศนิยมตำแหน่งที่สี่และตำแหน่งทศนิยมอื่นๆ จะถูกบันทึกเป็นส่วนขยายของเรกคอร์ด Bโดยตำแหน่งในแต่ละ บรรทัด ของเรกคอร์ด Bจะถูกระบุไว้ในเรกคอร์ด I ( AL8 )
แอลซียู	ล.	ข้อมูลจากระบบ SeeYou หลังเที่ยวบิน ไม่จำเป็นสำหรับการตรวจสอบความถูกต้อง แต่ใช้ในระบบวิเคราะห์เที่ยวบินบางระบบ
ล็อด	ฉัน , บี	ตำแหน่งสุดท้ายของนาทีทศนิยมของลองจิจูด ซึ่งลองจิจูดจะถูกบันทึกด้วยความแม่นยำมากกว่าสามนาทีทศนิยมที่อยู่ในเนื้อหาหลักของ Brecord ตำแหน่งทศนิยมที่สี่และตำแหน่งทศนิยมถัดไปจะถูกบันทึกเป็นส่วนขยายของเรกคอร์ด Bโดยตำแหน่งในแต่ละ บรรทัดของ เรกคอร์ด Bจะระบุไว้ใน เรกคอร์ด I ( AL8 )
กฎ	และ	แรงดันไฟฟ้าต่ำ ต้องตั้งค่าแรงดันไฟฟ้าต่ำสุดที่ FR จะทำงาน โดยที่ FR แต่ละตัวจะไม่สูญเสียข้อมูลที่บันทึกไว้เนื่องจากระดับแรงดันไฟฟ้า ห้ามใช้เพื่อยกเลิกเที่ยวบินหากข้อมูลการบินปรากฏว่าถูกต้องเมื่อตรวจสอบตามปกติ แต่เป็นการเตือนให้ตรวจสอบข้อมูลที่ถูกต้องอย่างละเอียด (AL1)
แม็ค	และ	การตั้งค่า MacCready สำหรับอัตราการไต่ระดับ/ความเร็วในการบิน (ม./วินาที) ( AL8 )
เอ็มซียู	ล.	ข้อมูลจากระบบ SeeYou หลังเที่ยวบิน ไม่จำเป็นสำหรับการตรวจสอบความถูกต้อง แต่ใช้ในระบบวิเคราะห์เที่ยวบินบางระบบ
MP2,
MP3 ฯลฯ	ฉัน , บี	ระบบขับเคลื่อนที่ติดตั้งเพิ่มเติมนอกเหนือจากระบบ MOP พื้นฐาน ดู MOP ด้านล่าง
ขัดต่อ	เจ , เค	อุณหภูมิมอเตอร์ องศาเซลเซียส
ซับ	ฉัน , บี	ระบบขับเคลื่อน สัญญาณจากฟังก์ชันที่เกี่ยวข้องกับเครื่องยนต์จากเซ็นเซอร์ที่แยกจากระบบ ENL ใน FR ให้ตัวเลขสามตัว
สุทธิ	เจ , เค	NETTO - NETT (=โดยรวม) การเคลื่อนที่ของอากาศในแนวตั้ง ความเร็วแนวตั้งของอากาศเป็นเมตรต่อวินาที (AL8)
OA1 OA2 OA3 ฯลฯ	และ	ตำแหน่งของเครื่องบินลำอื่น (หากระบบบันทึกข้อมูลนี้) โดยช่องข้อมูลหลังรหัสจะคั่นด้วยเครื่องหมายโคลอน รูปแบบหลังรหัสสามตัวอักษรคือการระบุเครื่องบินที่เกี่ยวข้อง (หากระบบบันทึกข้อมูลนี้ไว้ มิฉะนั้นให้ใส่ NK สำหรับไม่ทราบค่า) ตามด้วยเครื่องหมายโคลอน ตัวอักษร P สำหรับขั้วโลก หรือ C สำหรับคาร์ทีเซียน ตามด้วยพิกัด พิกัดขั้วโลกจะอ้างอิงกับเครื่องบันทึก รูปแบบคือตัวเลขสำหรับระยะทางแนวนอนเป็นเมตรจากเครื่องบันทึก ตามด้วยเครื่องหมายโคลอน ตามด้วยตัวเลข 3 องศาตามเข็มนาฬิกาจาก 000 สำหรับทิศเหนือ ตามด้วยเครื่องหมายโคลอนและระยะทางแนวตั้งเป็นเมตรจากเครื่องบันทึก โดยมีเครื่องหมายลบนำหน้าตัวเลขหมายถึงระยะทางแนวตั้งเป็นลบ หลังจากตัวเลขสำหรับระยะทางแนวตั้ง ควรใช้ตัวอักษร G สำหรับข้อมูล GNSS และ P สำหรับความดันและความสูง ซึ่งสามารถใช้ได้ทั้งสองอย่างหากมีข้อมูล หรืออีกวิธีหนึ่งคือ พิกัดคาร์ทีเซียนสามารถใช้กับตำแหน่งสามมิติของเครื่องบินลำอื่นได้ (เช่น จาก ADS-B และระบบรายงานตำแหน่งที่คล้ายกัน) รูปแบบคือละติจูด/ลองจิจูด ตามด้วยความดันอากาศและระดับความสูง GPS (หากระบบบันทึกข้อมูลเหล่านี้) ในลำดับและรูปแบบเดียวกันกับบันทึก B (ย่อหน้า 4.1) โดยละเว้นอักขระความถูกต้องคงที่ หากไม่ได้บันทึกระดับความสูงประเภทใด ควรแทนที่ด้วยศูนย์ ( AL10 )
โอเอที	เจ , เค	อุณหภูมิอากาศภายนอก (เซลเซียส) หากเป็นลบ ให้ใช้เครื่องหมายลบนำหน้าตัวเลข
มี	และ	On Task � กำลังพยายามทำภารกิจ
โอไอ	ชม	OO ID � การสังเกตอุปกรณ์ OO
พีอีวี	และ	Pilot EVent - การดำเนินการเริ่มต้นของ Pilot เช่น การกดปุ่ม ลำดับการแก้ไขอย่างรวดเร็วมีดังนี้ (ย่อหน้า 2.6.7.3) ( AL8 )
พีเอฟซี	ล.	การเคลมหลังเที่ยวบิน สำหรับเที่ยวบินฟรีที่เคลมจุดแวะพักหลังเที่ยวบิน ( AL5 )
โฟ	และ	ถ่ายภาพ (กดชัตเตอร์)
พีแอลที	ชม	นักบินผู้รับผิดชอบ (ผู้บังคับเครื่องบิน) นามสกุลก่อน แล้วจึงตั้งชื่อตามที่กำหนด ( AL8 )
พีอาร์เอส	ชม	เซ็นเซอร์วัดความดันความสูง ผู้ผลิต รุ่น ฯลฯ ( AL3 )
ไร่	ฉัน , บี , เจ , เค	RAIM - พารามิเตอร์ GPS ดูคำศัพท์
เร็กซ์	ฉัน , บี , เจ , เค	ส่วนขยายเรกคอร์ด - ข้อมูลที่กำหนดโดยผู้ผลิตซึ่งกำหนดไว้ในเรกคอร์ด I หรือJตามความเหมาะสม โดยปกติจะอยู่ในรูปแบบ TLC (ซึ่งหากตกลงตัวแปรใหม่ อาจเป็น TLC ใหม่ที่ GFAC จัดสรรให้ในขณะนั้น) การใช้งานใดๆ จะต้องได้รับการอนุมัติจาก GFAC และเผยแพร่เพื่อให้ไม่มีข้อสงสัยใดๆ เกี่ยวกับวิธีการใช้งาน ( AL4 )
เอฟอาร์ดับบลิว	ชม	เวอร์ชันแก้ไขเฟิร์มแวร์ของ FR
อาร์เอชดับบลิว	ชม	เวอร์ชันแก้ไขฮาร์ดแวร์ของ FR
รอบต่อนาที	ฉัน , บี	กลุ่มตัวเลขสามตัวตั้งแต่ 000 ถึง 999 ที่เกี่ยวข้องกับการสร้างแรงขับไปข้างหน้า ตัวอย่างเช่น ค่ารอบต่อนาทีของใบพัดหรือเครื่องยนต์ หรือตัวแปร MoP อื่นๆ ที่สอดคล้องกับ GFAC ซึ่งมีการเปลี่ยนแปลงในลักษณะเดียวกัน ตัวแปรนี้ต้องได้รับการบันทึกอยู่เสมอ และนักบินต้องไม่สามารถปิดการทำงานได้ เช่น ผ่านสวิตช์ห้องนักบิน เบรกเกอร์ หรือฟิวส์ ควรใช้ตัวเลขทั้งหมดจนถึง 999 ตัวอย่างเช่น หากบันทึกค่ารอบต่อนาทีและค่ารอบต่อนาทีสูงสุดคือ 3000 จะต้องบันทึกค่านี้ในบันทึกBเป็น 999 หรือใกล้เคียง ค่าต่ำสุดพื้นฐานต้องแสดงค่ารอบต่อนาทีเป็นบวกแต่ต่ำในไฟล์ IGC (เช่น 010 แต่ไม่เกิน 025) เพื่อตรวจสอบอย่างต่อเนื่องว่าวงจรยังคงทำงานอยู่ GFAC จะพิจารณาการบันทึกกำลังเครื่องยนต์ต่ำที่ให้แรงขับไปข้างหน้าเป็นพิเศษ และตรวจสอบให้แน่ใจว่าค่าเหล่านี้แสดงค่าที่สูงเพียงพอที่จะแสดงการใช้งานเครื่องยนต์ได้อย่างชัดเจน ( AL10 )
เอสซีเอ็ม	ชม	รหัสล้าสมัย ตอนนี้ใช้ CM2 เดิมชื่อลูกเรือคนที่สอง ( AL8 )
วินาที	จี	ความปลอดภัย - บันทึกข้อมูลความปลอดภัย
นั่ง	ชม	สถานที่, ชื่อ, ภูมิภาค, ประเทศ ฯลฯ
ซิว	ฉัน , บี	ดาวเทียมที่ใช้งานอยู่ ฟิลด์สองอักขระจากประโยค NMEA GGA หรือ GNS ตามความเหมาะสม หรือข้อมูลเทียบเท่าที่ตกลงโดย GFAC ( AL4 )
STA	และ	เริ่มกิจกรรม
ที่	ฉัน , บี , เจ , เค	ความเร็วอากาศ จริง ให้หน่วย (kt, kph, ฯลฯ)
ทีดีเอส	ฉัน , บี , เจ , เค	วินาทีทศนิยมของเวลา UTC สำหรับใช้กับระบบที่บันทึกเวลาด้วยความแม่นยำนี้ เวลาเป็นวินาทีจะถูกบันทึกในส่วนเนื้อหาหลักของเรกคอร์ด Bและวินาทีทศนิยมจะถูกบันทึกเป็นส่วนขยายของเรกคอร์ด Bโดยตำแหน่งในแต่ละ บรรทัดของ เรกคอร์ด Bจะระบุไว้ในเรกคอร์ด Iเช่นเดียวกับเรกคอร์ด K และ J ( AL8 )
สิบ	ฉัน , บี , เจ , เค	ความสูงพลังงานรวมเป็นเมตร
ทีพีซี	และ	การยืนยันจุดเปลี่ยน - เหตุการณ์ที่สร้างโดยอุปกรณ์ (ไม่สามารถใช้สำหรับการตรวจสอบการบินซึ่งต้องมีการตรวจสอบจุดแก้ไขและโซนสังเกตการณ์ที่เกี่ยวข้องอย่างอิสระ)
ทีอาร์เอ็ม	ฉัน , บี , เจ , เค	ติดตามแม่เหล็ก สามตัวเลขตามองศาตามเข็มนาฬิกาจาก 000 สำหรับทิศเหนือ ( AL8 )
ทีอาร์ที	ฉัน , บี , เจ , เค	ติดตามความจริง สามตัวเลขที่อิงตามองศาตามเข็มนาฬิกาจาก 000 สำหรับทิศเหนือ ( AL8 )
TZN	ชม	โซนเวลาออฟเซ็ต ชั่วโมงจาก UTC ถึงเวลาท้องถิ่น
และ	และ	ช่วงล่าง (ล้อลงจอด) บันทึกเป็น UP หรือ DN ในรูปแบบ UNDUP หรือ UNDDN( AL8 )
ยูเอ็นที	ชม	หน่วยวัด
ของเรา	เจ , เค	ความเร็วแนวตั้งของวาริออมิเตอร์แบบไม่ชดเชย (ไม่ใช่พลังงานรวม) เป็นเมตรและเมตรทศนิยม หากเป็นลบ ให้ใช้เครื่องหมายลบหน้าตัวเลข ( AL8 )
ภาษีมูลค่าเพิ่ม	เจ , เค	ความเร็วแนวตั้งของวาริออมิเตอร์แบบชดเชย (พลังงานรวม/เน็ตโต) เป็นเมตรและหน่วยทศนิยม หากเป็นลบ ให้ใช้เครื่องหมายลบหน้าตัวเลข ( AL8 )
เล่มที่	เจ , เค	โวลต์ไฟฟ้า
VO1	เจ , เค	แรงดันไฟฟ้าของแบตเตอรี่แรกที่มีการติดตั้งแบตเตอรี่ขับเคลื่อนสองลูก (AL8)
VO2	เจ , เค	แรงดันไฟฟ้าของแบตเตอรี่ที่สองที่มีการติดตั้งแบตเตอรี่ขับเคลื่อนสองก้อน (AL8)
วีเอ็กซ์เอ	ฉัน , บี , เจ , เค	ความแม่นยำในการแก้ไขแนวตั้ง สามอักขระเป็นเมตรจากส่วน VDOP ของประโยค NMEA GSA หรือข้อมูลเทียบเท่าที่ตกลงโดย GFAC ( AL4 )
ดับเบิ้ลยูดีไอ	ฉัน , บี , เจ , เค	ทิศทางลม (ทิศทางที่ลมพัดมา) ตัวเลขสามตัวที่คำนวณจากองศาตามเข็มนาฬิกาจาก 000 สำหรับทิศเหนือ ( AL8 )
ดับบลิวเอสพี	ฉัน , บี , เจ , เค	ความเร็วลม สามตัวเลขเป็นกิโลเมตรต่อชั่วโมง ( AL8 )
ดับเบิ้ลยูวีอี	เจ , เค	ความเร็วลม - ทิศทางลม (องศาจากทิศเหนือจริง) และความแรงลม (กม./ชม.) เช่น "27022" หมายถึง ทิศตะวันตก (270 องศา) ที่ความเร็ว 22 กม./ชม. (AL8)
เอ็กซ์เอ็น*	ตามความเหมาะสม	รหัสที่ผู้ผลิตเลือก โดยที่ N คือชื่อ IGC อักขระเดียวของผู้ผลิต (ภาคผนวก 1 ย่อหน้า 3.5.6) และ * สามารถเป็นอักขระใดก็ได้ ผู้ผลิตต้องระบุความหมายและการใช้งานไว้ในเอกสารประกอบของเครื่องบันทึก และการใช้งานต้องได้รับการอนุมัติจาก GFAC ก่อนการอนุมัติเครื่องบันทึกจาก IGC คำนำหน้า X มีวัตถุประสงค์เพื่อให้ทดลองใช้รหัสใหม่ชั่วคราวก่อนตัดสินใจว่าควรเพิ่มรหัสนี้ในรายการทั้งหมดหรือไม่ ( AL8 )
8. ข้อมูลพิกัดทางภูมิศาสตร์ GNSS
กฎการกีฬาสำหรับการร่อนระบุว่าต้องใช้ข้อมูลภูมิสารสนเทศ WGS 84 (หมายเลขลำดับ 100 ด้านล่าง) สำหรับพิกัดละติจูด/ลองจิจูดทั้งหมดที่บันทึกและถ่ายโอนจาก FR หลังจากเที่ยวบิน ข้อมูลภูมิสารสนเทศอื่นๆ ได้รับการกำหนดหมายเลขโดย IGC ดังต่อไปนี้

หมายเหตุจาก Ian Forster-Lewis: ฉันข้ามส่วนนี้ไป - ใช้เพียงรหัส WGS84 IGC 100

9. ตัวอย่างไฟล์รูปแบบ IGC
สำหรับตัวอย่างที่ซับซ้อนในโลกแห่งความเป็นจริง โปรดดู ไฟล์ IGC ที่ผลิตโดย LXN จากเที่ยวบินจริงในปี 2022

9.1 รูปแบบไฟล์ IGC เริ่มต้นด้วยระเบียน Aและตามด้วย H (ส่วนหัว) และระเบียนอื่นๆ ตัวอักษรของระเบียนจะอยู่ที่จุดเริ่มต้นของบรรทัดที่ถูกต้องในไฟล์เสมอเมื่อดูในรูปแบบข้อความ สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับรูปแบบสำหรับแต่ละระเบียน โปรดดูย่อหน้าที่เกี่ยวข้องก่อนหน้าในภาคผนวกนี้

9.2ในตัวอย่างนี้ มีการใช้ช่องว่างระหว่างช่องหัวเรื่องเพื่อให้เค้าโครงและลำดับชัดเจนขึ้นสำหรับผู้อ่าน ในไฟล์รูปแบบ IGC จริง ไม่ควรมีช่องว่างในระเบียนใดๆ ยกเว้นภายในสตริงข้อความเพื่อเป็นตัวคั่นคำ

9.3 CRLF = ตัวสิ้นสุดเส้นทาง ไม่ใช่ข้อมูลการบิน

9.4ในไฟล์จริงจะมีB เรคคอร์ด เพิ่มเติมอีกมากมาย ในช่วงการแก้ไขที่ตั้งไว้ล่วงหน้าสำหรับอัตราการล่องเรือและการแก้ไขอย่างรวดเร็ว

9.5ในตัวอย่างด้านล่าง มีหมายเหตุบางส่วนปรากฏในวงเล็บ ซึ่งไม่ได้เป็นส่วนหนึ่งของรูปแบบไฟล์ นอกจากนี้ เพื่อความชัดเจน มีการใช้ช่องว่างบางส่วนใน บรรทัด เรกคอร์ด Bระหว่างตัวแปรต่างๆ ที่ถูกบันทึก แต่ไม่ควรใช้ช่องว่างในไฟล์ IGC เอง

AXXXABC เที่ยวบิน:1
เอชเอฟเอฟเอ035
HFDTE160701
HFPLTPILOTINCHARGE: บล็อกส์ บิล ดี
HFCM2CREW2: สมิธ-แบร์รี่ จอห์น เอ
HFGTYGLIDERTYPE: Schleicher ASH-25
HFGIDGLIDERID: ABCD-1234
HFDTM100GPSDATUM: WGS-1984
HFRFWFIRMWAREVERSION:6.4
HFRHWHARDWARเวอร์ชัน:3.0
HFFTYFRTYPE: ผู้ผลิต, รุ่น
HFGPSMarconiCanada: Superstar,12 ช่อง, สูงสุด 10,000 เมตร
HFPRSPRESSALTSENSOR: Sensyn, XYZ1111, สูงสุด 11000m CR LF
HFCIDCOMPETITIONID: XYZ-78910
HFCCLCOMPETITIONCLASS: เครื่องร่อนมอเตอร์ 15 ม.
I033638FXA3940SIU4143ENL ( หมายเหตุ: ฉันแก้ไขคำพิมพ์ผิดจากเอกสารต้นฉบับที่มี RPM ในบันทึกนี้ )
J010812HDTCRLF
C150701213841160701000102 500K ไตร
C5111359N00101899W ลาแชมคลับเฮาส์
C5110179N00102644W Lasham สตาร์ท S สตาร์ท
C5209092N00255227W ซาร์เนสฟิลด์, TP1
C5230147N00017612W นอร์แมน ครอส, TP2
C5110179N00102644W Lasham สตาร์ท S จบ
C5111359N00101899W ลาแชมคลับเฮาส์
F160240040609123624221821
B1602405407121N00249342WA002800042120509950
D20331
E160245PEV
B1602455107126N00149300WA002880042919509020
B1602505107134N00149283WA002900043221009015
B1602555107140N00149221WA002900043020009012
F1603000609123624221821
B1603005107150N00149202WA002910043225608009
E160305PEVCRLF
B1603055107180N00149185WA002910043521008015
B1603105107212N00149174WA002930043519608024
K16024800090 ( AL7 )
B1602485107220N00149150WA 00494 00436 190 08 018
B1602525107330N00149127WA 00496 00439 195 08 015
LXXXวันชาติสหรัฐอเมริกา
LXXXเวลาบิน: 4:14:25, ความเร็วภารกิจ: 58.48 กิโลตัน
GREJNGJERJKNJKRE31895478537H43982FJN9248F942389T433T
GJNJK2489IERGNV3089IVJE9GO398535J3894N358954983O0934
GSKTO5427FGTNUT5621WKTC6714FT8957FGMKJ134527FGTR6751
GK2489IERGNV3089IVJE39GO398535J3894N358954983FTGY546
G12560DJUWT28719GTAOL5628FGWNIST78154INWTOLP7815FITN
```
