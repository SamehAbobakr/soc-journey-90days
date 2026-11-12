
# Pyramid of Pain

![Pyramid of Pain](assets
/pyramid-of-pain.svg)

## 1. Definition (التعريف)

**Pyramid of Pain** is a cybersecurity model introduced by David Bianco in 2013. It illustrates how difficult it is for attackers to change different types of Indicators of Compromise (IOCs) after defenders detect them.

هرم الألم هو نموذج في الأمن السيبراني قدمه David Bianco عام 2013، ويوضح مدى صعوبة تغيير المهاجم لأنواع مختلفة من مؤشرات الاختراق (IOCs) بعد اكتشافها بواسطة المدافعين.

**Core Idea (الفكرة الأساسية):**

The higher the indicator is in the pyramid, the more difficult and costly it becomes for the attacker to change it.

كلما ارتفع المؤشر في الهرم، أصبح تغييره أكثر صعوبة وتكلفة بالنسبة للمهاجم.

## 2. The Six Levels (المستويات الستة)

### 1. Hash Values (قيم التجزئة)

**Definition:** Unique digital fingerprints used to identify files.

بصمات رقمية تُستخدم للتعرف على الملفات، مثل MD5 وSHA-256.

**Example:** Blocking a malicious file using its SHA-256 hash.

**Pain Level:** Trivial (سهل جدًا).

### 2. IP Addresses (عناوين IP)

**Definition:** IP addresses used by attackers to communicate with compromised systems or host malicious infrastructure.

عناوين IP التي يستخدمها المهاجم للتواصل مع الأجهزة المخترقة أو استضافة البنية التحتية الخبيثة.

**Example:** Blocking a malicious IP address.

**Pain Level:** Easy (سهل).

### 3. Domain Names (أسماء النطاقات)

**Definition:** Domains used by attackers to host malicious websites or command-and-control infrastructure.

أسماء النطاقات التي يستخدمها المهاجم لاستضافة مواقع خبيثة أو بنية القيادة والتحكم.

**Example:** Blocking a malicious domain.

**Pain Level:** Simple (بسيط).

### 4. Network / Host Artifacts (آثار الشبكة والنظام)

**Definition:** Observable characteristics or behaviors left by malicious activity on a network or host.

الخصائص أو السلوكيات التي يمكن ملاحظتها نتيجة النشاط الخبيث داخل الشبكة أو الجهاز.

**Examples:**
- Registry modifications.
- Specific network traffic patterns.
- Unusual file paths.
- Suspicious system behavior.

**Pain Level:** Annoying (مزعج).

### 5. Tools (الأدوات)

**Definition:** Software or utilities used by attackers to perform malicious activities.

البرامج والأدوات التي يستخدمها المهاجم لتنفيذ الأنشطة الخبيثة.

**Examples:**
- Mimikatz.
- Cobalt Strike.
- Custom malware.

**Pain Level:** Challenging (صعب).

### 6. TTPs (Tactics, Techniques, and Procedures)

**Definition:** The tactics, techniques, and procedures that describe how an attacker operates.

الأساليب والتقنيات والإجراءات التي تصف طريقة عمل المهاجم وتنفيذه للهجمات.

**Examples:**
- Credential Dumping.
- Phishing.
- Lateral Movement.
- Persistence.

**Pain Level:** Tough (صعب جدًا).

## 3. My Understanding (فهمي الشخصي)

The Pyramid of Pain helps defenders understand that not all indicators have the same value when detecting and responding to threats.

يساعد هرم الألم فرق الأمن على فهم أن جميع المؤشرات ليست متساوية في قيمتها عند اكتشاف التهديدات والاستجابة لها.

Changing a file hash is usually easy for an attacker, but changing the techniques and procedures used to conduct an attack can require significant effort.

تغيير Hash لملف غالبًا سهل بالنسبة للمهاجم، لكن تغيير التقنيات والإجراءات التي يعتمد عليها في تنفيذ الهجوم قد يتطلب مجهودًا كبيرًا.

## 4. Practical Application (التطبيق العملي)

As a SOC Analyst, I can use the Pyramid of Pain to:

- Understand the value of different IOCs.
- Prioritize behavioral detection over relying only on file hashes.
- Identify attacker techniques and patterns.
- Improve threat detection and incident response.

كمحلل SOC، أستطيع استخدام هرم الألم لفهم قيمة مؤشرات الاختراق المختلفة، وإعطاء أهمية أكبر لاكتشاف السلوكيات والتقنيات بدل الاعتماد فقط على Hash، وتحسين اكتشاف التهديدات والاستجابة للحوادث.

## 5. Key Takeaways (أهم النقاط)

- The Pyramid of Pain contains six levels.
- Hash Values are at the bottom and are easy to change.
- TTPs are at the top and are difficult to change.
- Higher levels generally cause more effort and cost for attackers.
- Behavioral detection can provide more durable detection than relying only on static indicators.

- يتكون الهرم من ستة مستويات.
- Hash Values في القاعدة ويسهل تغييرها.
- TTPs في القمة ويصعب تغييرها.
- المستويات الأعلى تتطلب مجهودًا وتكلفة أكبر من المهاجم.
- اكتشاف السلوكيات قد يوفر حماية أكثر استمرارية من الاعتماد على المؤشرات الثابتة وحدها.

## 6. Reference (المصدر)

David Bianco – The Pyramid of Pain:

https://detect-respond.blogspot.com/2013/03/the-pyramid-of-pain.html
