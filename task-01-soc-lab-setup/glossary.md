# SOC Glossary — مصطلحات مركز العمليات الأمنية

This glossary contains 15 essential cybersecurity and SOC terms with simple definitions and practical examples.

## 1. SOC (Security Operations Center)

**Definition:** A team or department responsible for monitoring, detecting, analyzing, and responding to security threats.

**بالعربي:** مركز العمليات الأمنية، وهو الفريق المسؤول عن مراقبة الأنظمة واكتشاف التهديدات وتحليلها والاستجابة لها.

**Example:** A SOC analyst monitors company security alerts and investigates suspicious activities.

## 2. SIEM (Security Information and Event Management)

**Definition:** A system that collects and analyzes logs from different sources to detect suspicious activities and generate alerts.

**بالعربي:** نظام يجمع الـ Logs من أجهزة وأنظمة مختلفة ويحللها لاكتشاف الأنشطة المشبوهة وإصدار التنبيهات.

**Example:** A SIEM detects multiple failed login attempts from the same IP address.

## 3. EDR (Endpoint Detection and Response)

**Definition:** A security solution that monitors endpoint devices, detects suspicious behavior, and helps investigate and respond to threats.

**بالعربي:** أداة لمراقبة أجهزة المستخدمين مثل أجهزة الكمبيوتر، واكتشاف السلوك الضار والاستجابة له.

**Example:** EDR detects suspicious PowerShell activity and helps isolate the affected computer.

## 4. IOC (Indicator of Compromise)

**Definition:** An indicator that may suggest a system has been compromised.

**بالعربي:** علامة أو دليل قد يشير إلى تعرض النظام للاختراق.

**Examples:**
- Malicious IP address.
- Suspicious domain name.
- Malware file hash.

## 5. TTP (Tactics, Techniques, and Procedures)

**Definition:** Describes how attackers operate, including their goals, methods, and specific actions.

**بالعربي:**
- **Tactics:** هدف المهاجم.
- **Techniques:** الطريقة التي يستخدمها لتحقيق الهدف.
- **Procedures:** الخطوات أو الأسلوب العملي الذي ينفذه.

**Example:**
- Tactic: Credential Access.
- Technique: Phishing.
- Procedure: Sending a fake login page to steal credentials.

## 6. True Positive

**Definition:** An alert that correctly identifies real malicious activity.

**بالعربي:** تنبيه صحيح، والتحقيق يؤكد وجود نشاط ضار بالفعل.

**Example:** An alert detects malware, and the analyst confirms the file is malicious.

## 7. False Positive

**Definition:** An alert that incorrectly identifies normal activity as malicious.

**بالعربي:** تنبيه خاطئ، حيث يظهر نشاط طبيعي على أنه تهديد.

**Example:** A legitimate administrative tool triggers a suspicious activity alert.

## 8. Triage

**Definition:** The initial assessment of an alert to determine its validity, severity, priority, and required actions.

**بالعربي:** الفرز الأولي للتنبيه لتحديد مدى خطورته وهل يحتاج إلى تحقيق أو تصعيد.

**Example:** An analyst checks the source IP, affected user, and event details before deciding what to do.

## 9. Escalation

**Definition:** Transferring an alert or security case to a higher-level analyst or specialized team when additional expertise or authority is required.

**بالعربي:** تصعيد الحالة إلى محلل أعلى أو فريق متخصص لاستكمال التحقيق أو الاستجابة.

**Example:** A Tier 1 analyst escalates a confirmed malware incident to Tier 2.

## 10. Playbook

**Definition:** A predefined set of procedures that guides analysts through responding to a specific type of security event or incident.

**بالعربي:** خطة إجراءات جاهزة توضح للفريق كيفية التعامل مع نوع محدد من الحوادث الأمنية.

**Example:** A phishing response playbook explains how to investigate a suspicious email, block malicious links, and protect affected accounts.

## 11. Log

**Definition:** A recorded record of activities or operations performed by a system, application, or device.

**بالعربي:** سجل يسجل الأنشطة والعمليات التي تحدث داخل النظام أو التطبيق.

**Example:** A server records user login attempts in its authentication logs.

## 12. Event

**Definition:** An observable occurrence or activity recorded by a system.

**بالعربي:** حدث أو نشاط تم تسجيله داخل النظام، وقد يكون طبيعيًا أو مشبوهًا.

**Example:** A user successfully logs in to a Windows computer.

## 13. Alert

**Definition:** A notification generated when a security system detects activity that matches a suspicious condition or detection rule.

**بالعربي:** تنبيه يصدر عندما يكتشف نظام الحماية نشاطًا يطابق قاعدة أو شرطًا مشبوهًا.

**Example:** A SIEM generates an alert after detecting many failed login attempts.

## 14. Incident

**Definition:** A security event or group of events that requires investigation and response because it threatens the confidentiality, integrity, or availability of systems or data.

**بالعربي:** حادث أمني يحتاج إلى تحقيق واستجابة لأنه قد يؤثر على سرية البيانات أو سلامتها أو توافرها.

**Example:** An attacker gains unauthorized access to a company account and steals sensitive data.

## 15. Baseline

**Definition:** A reference of normal system, network, or user behavior used to identify unusual activities.

**بالعربي:** خط أساس يوضح السلوك الطبيعي للمستخدم أو النظام، ونستخدمه لاكتشاف أي سلوك غير معتاد.

**Example:** If an employee usually logs in from Egypt during working hours, a login from another country at 3 AM may be suspicious.

## 16. Threat Hunting

**Definition:** A proactive process of searching for hidden threats in systems and networks, even when no security alert has been generated.

**بالعربي:** البحث الاستباقي عن التهديدات داخل الأنظمة والشبكات حتى لو لم يصدر أي تنبيه أمني.

**Example:** An analyst searches network logs for suspicious outbound connections that were not detected by existing security rules.

---

## Key Takeaway

Understanding these terms helps SOC analysts monitor systems, investigate alerts, identify threats, and respond to security incidents effectively.
