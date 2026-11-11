# Networking Diagnostic Test

**Date:** 2026-11-08

**Purpose:** Evaluate my networking knowledge from memory without external resources.

## 1. TCP vs UDP

### TCP

مناسب لنقل البيانات التي تحتاج إلى وصول موثوق، مع التأكد من وصول البيانات بالترتيب الصحيح، مثل نقل الملفات.

### UDP

مناسب للتطبيقات التي تحتاج إلى سرعة وتقليل التأخير، مثل البث المباشر والمكالمات الصوتية والمرئية.

### TCP Three-Way Handshake

هي عملية إنشاء اتصال بين جهازين باستخدام بروتوكول TCP، وتتكون من ثلاث مراحل:

**المرحلة الأولى — SYN**

يرسل جهاز العميل (Client) طلبًا إلى الخادم (Server) لبدء الاتصال.

**المرحلة الثانية — SYN-ACK**

يرد الخادم بالموافقة على الاتصال، ويؤكد استلام طلب العميل.

**المرحلة الثالثة — ACK**

يرسل جهاز العميل تأكيدًا باستلام رد الخادم، وبذلك يصبح الاتصال جاهزًا لنقل البيانات.

![TCP Three-Way Handshake](assets/tcp-handshake.svg)

## 2. Common Ports

| Port | Protocol / Service | Purpose |
|---|---|---|
| 22 | SSH |اتصال آمن بجهاز آخر والتحكم فيه عن بُعد |
| 53 | DNS | تحويل أسماء النطاقات إلى عناوين IP لتسهيل الوصول إلى المواقع والخدمات |
| 80 | HTTP | تبادل طلبات واستجابات الويب بين المتصفح والخادم دون تشفير افتراضيًا |
| 443 | HTTPS | تبادل بيانات الويب بشكل مشفر باستخدام TLS لحماية الاتصال |
| 445 | SMB | مشاركة الملفات والمجلدات والطابعات بين الأجهزة عبر الشبكة، خاصة في Windows |
| 3389 | RDP | التحكم في أجهزة Windows عن بُعد من خلال واجهة رسومية |
## 3. DNS Records (سجلات DNS)

سجلات DNS هي معلومات بتحدد إزاي الدومين يتعامل مع خدمات الإنترنت المختلفة.

- **A (Address Record):**
  - بيربط اسم الدومين بعنوان IP من نوع IPv4.
  - مثال: `example.com → 192.168.1.10`

- **MX (Mail Exchange Record):**
  - بيحدد سيرفر البريد الإلكتروني المسؤول عن استقبال الرسائل الخاصة بالدومين.
  - مثال: `example.com → mail.example.com`

- **TXT (Text Record):**
  - بيخزن معلومات نصية مرتبطة بالدومين.
  - من استخداماته:
    - SPF: تحديد السيرفرات المسموح لها بإرسال الإيميلات باسم الدومين.
    - DKIM: التحقق من صحة توقيع البريد الإلكتروني.
    - DMARC: تحديد سياسة التعامل مع رسائل البريد غير الموثوقة.
    - Domain Verification: التحقق من ملكية الدومين.

- **PTR (Pointer Record):**
  - بيربط عنوان IP باسم الدومين.
  - بيُستخدم في Reverse DNS Lookup.
  - مثال: `192.168.1.10 → example.com`

### Quick Comparison (مقارنة سريعة)

| Record | الوظيفة |
|---|---|
| A | Domain → IPv4 |
| MX | تحديد Mail Server |
| TXT | تخزين معلومات نصية |
| PTR | IP → Domain (Reverse DNS) |

## 4. ARP and NAT
- What is ARP?
- How does ARP work?
- What is NAT?
- Why is NAT used?

## 5. Network Devices
- Switch:
- Router:
- Firewall:

## 6. Self-Assessment
- Topics I understand well:
- Topics I find difficult:
- Topics I need to review:
