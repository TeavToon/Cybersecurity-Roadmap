# Cybersecurity-Roadmap
**โครงสร้างระบบการเรียนรู้สาย Network & Offensive Security**

**1. หมวดเครือข่ายและโครงสร้างพื้นฐานระดับองค์กร (Networking & Infrastructure)**

* **Computer Networking: A Top-Down Approach (8th Edition, 2021)**
  * **เป้าหมาย:** ทำความเข้าใจโพรโทคอลเครือข่ายสมัยใหม่ วิเคราะห์ Traffic
  * **จุดเด่น:** ระเบียบวิธี Top-Down ตัดความซับซ้อนนามธรรมออก
  * **อ้างอิง:** [สไลด์ประกอบการสอน](https://gaia.cs.umass.edu/kurose_ross/ppt.php)


* **Site Reliability Engineering: How Google Runs Production Systems (1st Edition, 2016)**
  * **เป้าหมาย:** จัดการวงจรชีวิตโครงสร้างพื้นฐานด้วยข้อมูลและคณิตศาสตร์
  * **จุดเด่น:** การจัดการ Hybrid Cloud, การบังคับใช้ SLOs, Fault Tolerance
  * **อ้างอิง:** [อ่านออนไลน์ฟรี](https://sre.google/books/)


* **วิดีโอประกอบการศึกษา (YouTube):**
  * [Jeremy's IT Lab](https://www.youtube.com/@JeremysITLab) (เจาะลึกเครือข่าย/Cisco)
  * [NetworkChuck](https://www.youtube.com/@NetworkChuck) (ภาพรวมเทคโนโลยีและ IT)



**2. หมวดแพลตฟอร์มฝึกฝนความปลอดภัยทางไซเบอร์ (Cybersecurity Platforms)**

* **การอุดรอยรั่วและเว็บแอปพลิเคชัน (Web Security):**
  * **OWASP Top 10 Project:** มาตรฐานช่องโหว่เว็บระดับโลก [เอกสารอ้างอิง](https://owasp.org/www-project-top-ten/)
  * **PortSwigger Web Security Academy:** แพลตฟอร์มปฏิบัติการอันดับหนึ่งสำหรับ Web Penetration Tester ห้ามข้ามเด็ดขาด [ทดลองเจาะระบบ](https://portswigger.net/web-security)
  * **PentesterLab:** (มีค่าใช้จ่าย) เน้นทำ Web Vulnerability ตรงไปตรงมา ไม่ต้องเดาโจทย์แบบ CTF


* **การเจาะระบบเครือข่ายและสภาพแวดล้อมจำลอง (Infrastructure Hacking):**
  * **TryHackMe:** ปูพื้นฐานและทำความเข้าใจช่องโหว่เป็นขั้นตอน
  * **Hack The Box (HTB):** ฝึกเจาะระบบในสภาพแวดล้อมที่ซับซ้อนเทียบเท่าองค์กรจริง


* **การเจาะระบบระดับล่าง (Binary Exploitation / Reverse Engineering):**
  * **Pwnable.tw / Pwnable.kr:** โหดและลึกกว่า HTB เหมาะสำหรับสาย Low-level



**3. หมวดภาษาคอมพิวเตอร์ระดับล่าง (C & Assembly)**
*เป้าหมาย: อ่านโค้ดเพื่อหาจุดอ่อนการจัดการ Memory และเขียน Payload*

* **C Language:**
  * **The C Programming Language (Kernighan & Ritchie):** ตำราคลาสสิกสำหรับทำความเข้าใจแก่นของ C (Pointers, Memory Allocation)
  * **Hacking: The Art of Exploitation (Jon Erickson):** เรียน C ผ่านการทำ Buffer Overflow
  * **แหล่งฝึกฝน:** [Learn-C.org](https://www.learn-c.org/) (ฝึก Syntax รวดเร็ว)


* **Assembly (x86/x64 & ARM):**
  * **OpenSecurityTraining.info:** คอร์ส Introductory Intel x86
  * **Practical Reverse Engineering (Bruce Dang):** เจาะลึกกลไก Architecture
  * **เครื่องมือวิเคราะห์:** [Godbolt Compiler Explorer](https://godbolt.org/) (เทียบ C กับ Assembly แบบ Real-time)


* **ขั้นตอนการปฏิบัติ:** เขียน C ง่ายๆ -> Decompile ด้วย GDB หรือ Ghidra -> วิเคราะห์ Assembly Code

**4. หมวดสคริปต์และระบบอัตโนมัติ (Bash & Python for Security)**

* **Bash / Linux Command Line:**
  * **OverTheWire (Bandit):** Wargame บังคับเล่นสำหรับฝึก Linux CLI เอาตัวรอดระดับรากฐาน [เริ่มเล่นที่นี่](https://overthewire.org/wargames/bandit/)
  * **Linux Journey:** สรุปคำสั่งระบบปฏิบัติการอย่างเป็นระบบ [บทเรียน 1](https://labex.io/linuxjourney), [บทเรียน 2](https://linuxbasecamp.com/)
  * **FreeCodeCamp Bash Tutorial:** [พื้นฐานสำหรับผู้เริ่มต้น](https://www.freecodecamp.org/news/bash-scripting-tutorial-linux-shell-script-and-command-line-for-beginners/)


* **Python (Security Tooling):**
  * **Black Hat Python (2nd Edition):** สอนเขียนโทรจัน สนิฟเฟอร์ และเครื่องมือเครือข่าย (ใช้โมดูล `socket`, `requests`)
  * **Violent Python:** การใช้ `Scapy` จัดการ Packet, เขียนสคริปต์ Brute-force
  * **pwntools:** ไลบรารีอาวุธหลักสาย Pwn ใช้ส่ง Payload (C/Assembly) เข้าช่องโหว่
  * **Python Automation Basics:** [GeeksforGeeks](https://www.geeksforgeeks.org/python/python-automation/)



**5. ยุทธวิธีการผสานระบบและแผนปฏิบัติการ 30 วัน (Execution Strategy)**

* **The Integration (การทำงานร่วมกันของระบบ):**
  * **C/Assembly:** ค้นหาช่องโหว่ (เช่น Buffer Overflow) คำนวณ Memory
  * **Python (pwntools):** จัดการส่ง Shellcode โจมตีเป้าหมายแบบอัตโนมัติ
  * **Bash:** รับ Reverse Shell, สำรวจเครื่องเป้าหมาย, ยกระดับสิทธิ์ (Privilege Escalation)


* **แผน 30 วันสำหรับทะลวงคอขวด (Bash & Python):**
  * **สัปดาห์ที่ 1-2:** โฟกัส OverTheWire (Bandit) ให้ผ่านอย่างน้อย Level 20 ห้ามเปิดเฉลยทันที ให้อ่าน `man page` เพื่อสร้างกล้ามเนื้อความจำบนหน้า Terminal
  * **สัปดาห์ที่ 3-4:** ศึกษา Black Hat Python เน้น Network Modules พิมพ์โค้ดด้วยตัวเองทั้งหมด ห้ามคัดลอก/วาง เพื่อทำความเข้าใจโครงสร้างการเชื่อมต่อระดับ Socket

---

นี่คือการจัดระเบียบและวางโรดแมป (Roadmap) การศึกษาเชิงกลยุทธ์จากคลังข้อมูลที่คุณมี โดยเรียงลำดับจากรากฐานที่ต้องสร้าง ไปจนถึงทักษะขั้นสูงที่สุด การข้ามขั้นตอนจะทำให้เกิดช่องโหว่ในความเข้าใจและทำให้การศึกษาในระดับถัดไปล้มเหลว

---

### **Phase 1: Core Infrastructure & OS (รากฐานโครงสร้างและระบบปฏิบัติการ)**

คุณไม่สามารถโจมตีหรือป้องกันระบบที่คุณไม่เข้าใจกลไกการทำงานได้ นี่คือจุดเริ่มต้นที่บังคับต้องผ่าน

* **ทฤษฎีและการจัดการเครือข่าย:**
  * เริ่มต้นด้วย *Computer Networking: A Top-Down Approach (8th Edition)* เพื่อเข้าใจกลไกโปรโตคอลตั้งแต่ Application ลงมาถึง Physical
  * ต่อยอดด้วย *CCNA 200-301* เพื่อการคอนฟิกฮาร์ดแวร์จริง ควบคู่กับช่อง YouTube: *Jeremy's IT Lab* และ *NetworkChuck*


* **ระบบปฏิบัติการและการเอาตัวรอด (Linux/Bash):**
  * อ่าน *UNIX and Linux System Administration Handbook* เพื่อเข้าใจสถาปัตยกรรมเซิร์ฟเวอร์
  * ฝึกปฏิบัติทันทีผ่าน *OverTheWire (Bandit)* โดยใช้แหล่งอ้างอิงจาก *Linux Journey*, *Linuxbasecamp*, และ *FreeCodeCamp Bash Scripting Tutorial*


* **การจัดการระดับองค์กร:**
  * อ่าน *Site Reliability Engineering: How Google Runs Production Systems* เพื่อเข้าใจการสเกลระบบและกระบวนการทำงานระดับโลก



### **Phase 2: Security Architecture & Analysis (สถาปัตยกรรมความปลอดภัยและการวิเคราะห์)**

เมื่อเข้าใจระบบแล้ว ต้องเรียนรู้วิธีตรวจสอบและมาตรฐานการป้องกัน

* **มาตรฐานระดับสากล:**
  * ศึกษา *NIST Cybersecurity Framework* และ *NIST.CSWP.29*
  * ศึกษา *OWASP Top 10 Project* เพื่อทำความเข้าใจช่องโหว่ยอดฮิตระดับโลก


* **การวิเคราะห์พฤติกรรมเครือข่าย:**
  * ศึกษา *Practical Packet Analysis* เพื่อจับตาดูทราฟฟิกที่ผิดปกติผ่าน Wireshark



### **Phase 3: Offensive Scripting (การเขียนสคริปต์เชิงรุก)**

เปลี่ยนจากผู้ใช้ (User) เป็นผู้สร้างเครื่องมือ (Tool Creator)

* **การพัฒนา Python สู่ Security Tooling:**
   * ศึกษาบทความ *Python Automation (GeeksforGeeks)* เพื่อปรับพื้นฐาน
   * เจาะลึกผ่านหนังสือ *Black Hat Python, 2nd Edition* เพื่อสร้างเครื่องมือดักจับหรือโจมตี และ *Violent Python* สำหรับแนวทางประยุกต์ใช้เพิ่มเติม



### **Phase 4: Web Application Security (ความปลอดภัยระดับเว็บแอปพลิเคชัน)**

สนามทดสอบที่เข้าถึงง่ายที่สุดและเป็นรากฐานของสาย Bug Bounty

* **คู่มือและตำราเจาะระบบ:**
  * อ่าน *The Web Application Hacker's Handbook* (ทฤษฎีคลาสสิก) ตามด้วย *Bug Bounty Bootcamp* (วิธีการทำเงินและเทคนิคสมัยใหม่)


* **แพลตฟอร์มฝึกฝนบังคับ:**
  * ลุยแล็บใน *PortSwigger Web Security Academy* ให้ครบทุกหัวข้อ



### **Phase 5: Infrastructure Penetration Testing (การเจาะระบบเครือข่ายระดับองค์กร)**

ยกระดับจากการเจาะเว็บ สู่การยึดเซิร์ฟเวอร์และเครือข่ายทั้งหมด

* **ยุทธวิธีการเจาะระบบ:**
  * ศึกษา *Network Security Assessment* เพื่อการประเมินความเสี่ยง และ *The Hacker Playbook 3* สำหรับแผนการรุกแบบ Red Team


* **แพลตฟอร์มจำลองสภาพแวดล้อมจริง:**
  * เริ่มที่ *TryHackMe* (สำหรับปูพื้นฐาน) และย้ายไป *Hack The Box (HTB)* (สำหรับสภาพแวดล้อมทางธุรกิจจริง)



### **Phase 6: Low-Level Exploitation & Reverse Engineering (ขั้นสุดยอด: เจาะระบบระดับล่าง)**

ศาสตร์ที่ยากที่สุด ต้องใช้ความเข้าใจหน่วยความจำภาษา C และ Assembly

* **ทำความเข้าใจโค้ดและหน่วยความจำ:**
  * อ่าน *Hacking - The Art of Exploitation* เล่มนี้จะเชื่อมโยง C, Assembly และการทำ Buffer Overflow เข้าด้วยกัน


* **การวิเคราะห์มัลแวร์:**
  * ศึกษา *Practical Malware Analysis* เพื่อทำ Reverse Engineering


* **แพลตฟอร์มฝึกฝน:**
  * ฝึกฝนผ่าน *Pwnable.tw* และ *Pwnable.kr*
