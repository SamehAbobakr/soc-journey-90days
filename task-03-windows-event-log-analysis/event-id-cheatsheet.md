
# Windows Event ID Cheatsheet
# مرجع أحداث أمان ويندوز

## 1. Authentication Events | أحداث تسجيل الدخول

### Event ID 4624 — Successful Logon
**English:** Indicates that a user successfully logged into the system.

**العربية:** يشير إلى نجاح عملية تسجيل الدخول إلى نظام Windows.

**SOC Investigation:**
- Identify the account that logged in.
- Check the Logon Type.
- Check the source IP address when available.

**التحليل الأمني:**
- تحديد الحساب الذي سجل الدخول.
- معرفة نوع تسجيل الدخول (Logon Type).
- فحص عنوان IP المصدر إذا كان متاحًا.

---

### Event ID 4625 — Failed Logon
**English:** Indicates that a logon attempt failed.

**العربية:** يشير إلى فشل محاولة تسجيل الدخول، وقد يكون السبب كلمة مرور خاطئة أو حسابًا غير صالح أو سببًا آخر.

**SOC Investigation:**
- Check the target username.
- Examine the failure reason.
- Look for repeated attempts from the same source.

**التحليل الأمني:**
- تحديد اسم المستخدم المستهدف.
- فحص سبب فشل تسجيل الدخول.
- البحث عن محاولات فاشلة متكررة من نفس المصدر.

---

### Event ID 4634 — Logoff
**English:** Indicates that a logon session was terminated.

**العربية:** يشير إلى انتهاء جلسة تسجيل دخول المستخدم.

---

### Event ID 4648 — Explicit Credentials
**English:** Indicates that a process attempted to log on using explicitly supplied credentials.

**العربية:** يشير إلى استخدام بيانات اعتماد محددة صراحةً لمحاولة تسجيل الدخول، مثل تشغيل برنامج باستخدام حساب آخر.

---

## 2. Privilege and Account Events | أحداث الحسابات والصلاحيات

### Event ID 4672 — Special Privileges Assigned
**English:** Indicates that special privileges were assigned to a new logon session.

**العربية:** يشير إلى منح جلسة تسجيل دخول صلاحيات خاصة، مثل بعض صلاحيات المسؤولين.

**SOC Investigation:** Check whether the account should have these privileges.

**التحليل الأمني:** تحقق مما إذا كان الحساب من المفترض أن يمتلك هذه الصلاحيات.

---

### Event ID 4720 — User Account Created
**English:** Indicates that a new user account was created.

**العربية:** يشير إلى إنشاء حساب مستخدم جديد على النظام.

**SOC Investigation:** Identify who created the account and when.

**التحليل الأمني:** حدد من أنشأ الحساب ومتى تم إنشاؤه.

---

### Event ID 4732 — Member Added to Security Group
**English:** Indicates that a member was added to a security-enabled local group.

**العربية:** يشير إلى إضافة مستخدم أو مجموعة إلى مجموعة أمنية محلية، مثل Administrators.

**SOC Investigation:** Check who added the member and which group was modified.

**التحليل الأمني:** تحقق ممن قام بالإضافة، وما المجموعة التي تمت إضافته إليها.

---

## 3. Process and System Events | أحداث العمليات والنظام

### Event ID 4688 — Process Creation
**English:** Indicates that a new process was created.

**العربية:** يشير إلى تشغيل عملية جديدة (Process) على النظام.

**SOC Investigation:** Examine the process name, creator account, and command line when available.

**التحليل الأمني:** افحص اسم العملية والحساب الذي شغّلها وسطر الأوامر إذا كان متاحًا.

---

### Event ID 1102 — Audit Log Cleared
**English:** Indicates that the Security audit log was cleared.

**العربية:** يشير إلى مسح سجل التدقيق الأمني. قد يكون إجراءً إداريًا مشروعًا أو محاولة لإخفاء آثار نشاط ضار.

---

### Event ID 7045 — Service Installed
**English:** Indicates that a new service was installed on the system.

**العربية:** يشير إلى تثبيت خدمة جديدة على Windows.

**Important:** Event ID 7045 belongs to the System log, not the Security log.

**ملاحظة:** الحدث 7045 موجود في سجل System وليس Security.

---

## 4. Important Investigation Notes | ملاحظات التحقيق

- Event 4624 does not automatically indicate a security breach.
- Event 4625 does not automatically indicate an attack.
- Repeated failed logons followed by a successful logon may indicate a possible brute-force attack.
- Events should be correlated to understand the full activity.

- الحدث 4624 لا يعني بالضرورة حدوث اختراق.
- الحدث 4625 لا يعني بالضرورة وجود هجوم.
- تكرار محاولات الدخول الفاشلة ثم نجاح الدخول قد يشير إلى هجوم تخمين كلمات المرور (Brute Force).
- يجب ربط الأحداث ببعضها لفهم النشاط بالكامل.

## 5. Investigation Questions | أسئلة التحقيق

1. Who performed the action? | من قام بالنشاط؟
2. When did it happen? | متى حدث؟
3. Which account was involved? | ما الحساب المرتبط بالحدث؟
4. What was the source IP address? | ما عنوان IP المصدر؟
5. Was the activity legitimate or suspicious? | هل النشاط مشروع أم مشبوه؟

