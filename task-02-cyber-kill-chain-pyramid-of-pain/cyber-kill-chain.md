# Cyber Kill Chain | سلسلة مراحل الهجوم السيبراني

## 1. Definition | التعريف

**English:**

The Cyber Kill Chain is a cybersecurity model developed by Lockheed Martin. It describes the seven stages of a cyberattack, from initial reconnaissance to achieving the attacker's objectives.

**العربية:**

سلسلة مراحل الهجوم السيبراني هي نموذج طورته شركة Lockheed Martin، ويشرح المراحل السبعة التي يمر بها الهجوم السيبراني، بدايةً من جمع المعلومات عن الهدف وحتى تحقيق المهاجم لهدفه النهائي.

## 2. The Seven Stages | المراحل السبعة

### 1. Reconnaissance | الاستطلاع وجمع المعلومات

**Definition – التعريف:**

- **English:** Gathering information about the target before launching an attack.
- **العربية:** جمع المعلومات عن الهدف قبل تنفيذ الهجوم.

**Example – مثال:**

- **English:** An attacker searches for employee emails, company domains, and exposed services.
- **العربية:** يبحث المهاجم عن عناوين البريد الإلكتروني للموظفين ونطاقات الشركة والخدمات المكشوفة.

**SOC Detection – الاكتشاف الأمني:**

- **English:** Monitor suspicious scanning activities and unusual information-gathering attempts.
- **العربية:** مراقبة عمليات فحص الشبكة المشبوهة ومحاولات جمع المعلومات غير المعتادة.

### 2. Weaponization | تجهيز السلاح

**Definition – التعريف:**

- **English:** Preparing a malicious payload or exploit to target the victim.
- **العربية:** تجهيز ملف ضار أو استغلال أمني لاستخدامه ضد الضحية.

**Example – مثال:**

- **English:** An attacker creates a malicious document containing malware.
- **العربية:** ينشئ المهاجم مستندًا ضارًا يحتوي على برمجية خبيثة.

**SOC Detection – الاكتشاف الأمني:**

- **English:** Analyze suspicious files, malware signatures, and threat intelligence indicators.
- **العربية:** تحليل الملفات المشبوهة وبصمات البرمجيات الخبيثة ومؤشرات التهديدات.

### 3. Delivery | توصيل الهجوم

**Definition – التعريف:**

- **English:** Transmitting the malicious payload to the target.
- **العربية:** إيصال الملف أو المحتوى الضار إلى الهدف.

**Example – مثال:**

- **English:** Sending a phishing email containing a malicious attachment.
- **العربية:** إرسال رسالة تصيد احتيالي تحتوي على مرفق ضار.

**SOC Detection – الاكتشاف الأمني:**

- **English:** Monitor suspicious emails, attachments, and malicious URLs.
- **العربية:** مراقبة رسائل البريد الإلكتروني والمرفقات والروابط المشبوهة.

### 4. Exploitation | استغلال الثغرة

**Definition – التعريف:**

- **English:** Triggering a vulnerability or exploiting a weakness in the target system.
- **العربية:** استغلال ثغرة أمنية أو نقطة ضعف في النظام المستهدف.

**Example – مثال:**

- **English:** A victim opens a malicious document that exploits a software vulnerability.
- **العربية:** يفتح الضحية مستندًا ضارًا يستغل ثغرة في أحد البرامج.

**SOC Detection – الاكتشاف الأمني:**

- **English:** Investigate exploit alerts, unusual processes, and suspicious system behavior.
- **العربية:** التحقيق في تنبيهات استغلال الثغرات والعمليات غير المعتادة وسلوك النظام المشبوه.

### 5. Installation | التثبيت

**Definition – التعريف:**

- **English:** Installing malware or another malicious component on the compromised system.
- **العربية:** تثبيت برمجية خبيثة أو مكون ضار على النظام الذي تم اختراقه.

**Example – مثال:**

- **English:** Malware installs itself and establishes persistence.
- **العربية:** تثبت البرمجية الخبيثة نفسها داخل النظام وتحاول ضمان استمرار وجودها حتى بعد إعادة التشغيل.

**SOC Detection – الاكتشاف الأمني:**

- **English:** Monitor suspicious file creation, registry modifications, and persistence mechanisms.
- **العربية:** مراقبة إنشاء الملفات المشبوهة وتعديلات سجل Windows وآليات الاستمرارية.

### 6. Command and Control (C2) | القيادة والتحكم

**Definition – التعريف:**

- **English:** Establishing communication between the compromised system and the attacker's infrastructure.
- **العربية:** إنشاء اتصال بين الجهاز المخترق والبنية التحتية التي يستخدمها المهاجم للتحكم فيه.

**Example – مثال:**

- **English:** Malware communicates with an external server to receive commands.
- **العربية:** تتصل البرمجية الخبيثة بخادم خارجي لاستقبال أوامر المهاجم.

**SOC Detection – الاكتشاف الأمني:**

- **English:** Monitor unusual outbound connections, suspicious DNS queries, and abnormal network traffic.
- **العربية:** مراقبة الاتصالات الصادرة غير المعتادة واستعلامات DNS المشبوهة وحركة مرور الشبكة غير الطبيعية.

### 7. Actions on Objectives | تنفيذ الأهداف

**Definition – التعريف:**

- **English:** Performing the attacker's intended actions after gaining access.
- **العربية:** تنفيذ المهاجم للأهداف التي يسعى إليها بعد نجاحه في الوصول إلى النظام.

**Example – مثال:**

- **English:** Stealing sensitive data, encrypting files, or disrupting services.
- **العربية:** سرقة البيانات الحساسة أو تشفير الملفات أو تعطيل الخدمات.

**SOC Detection – الاكتشاف الأمني:**

- **English:** Monitor data exfiltration, unusual account activity, and suspicious access to sensitive resources.
- **العربية:** مراقبة تسريب البيانات ونشاط الحسابات غير المعتاد والوصول المشبوه إلى الموارد الحساسة.

## 3. My Understanding | فهمي الشخصي

**English:**

Cyber Kill Chain helps me understand how a cyberattack progresses through multiple stages. As a SOC Analyst, understanding these stages helps me identify suspicious activities early and respond before the attacker achieves their objectives.

**العربية:**

يساعدني نموذج Cyber Kill Chain على فهم كيفية تطور الهجوم السيبراني عبر مراحل متعددة. وبصفتي محلل SOC، فإن فهم هذه المراحل يساعدني على اكتشاف الأنشطة المشبوهة مبكرًا والاستجابة لها قبل أن يحقق المهاجم أهدافه.

## 4. Key Takeaways | أهم النقاط

- **English:** Early detection can prevent an attacker from progressing to later stages.
- **العربية:** الاكتشاف المبكر يمكن أن يمنع المهاجم من الانتقال إلى المراحل التالية.

- **English:** Each stage provides an opportunity for security teams to detect and disrupt an attack.
- **العربية:** كل مرحلة توفر فرصة لفرق الأمن لاكتشاف الهجوم وتعطيله.

## 5. Reference | المصدر

- Lockheed Martin – Cyber Kill Chain: https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html
