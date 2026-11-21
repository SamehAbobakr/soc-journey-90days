
# Windows Logon Types
# أنواع تسجيل الدخول في ويندوز

## What is a Logon Type?
A Logon Type identifies the method used to establish a logon session in Windows.

نوع تسجيل الدخول يحدد الطريقة التي تم استخدامها لإنشاء جلسة تسجيل دخول في Windows.

## Common Logon Types

| Type | Name | English Description | الشرح بالعربية |
|---|---|---|---|
| 2 | Interactive | Local interactive logon | دخول مباشر على الجهاز |
| 3 | Network | Network-based logon | دخول عبر الشبكة |
| 4 | Batch | Batch job logon | دخول لتنفيذ مهمة مجدولة |
| 5 | Service | Service logon | دخول خاص بتشغيل خدمة |
| 10 | RemoteInteractive | Remote Desktop logon | دخول عن بُعد باستخدام RDP |

## SOC Investigation

When analyzing Event ID 4624 or 4625, check:

1. Logon Type — طريقة تسجيل الدخول.
2. Account Name — اسم الحساب.
3. Source Network Address — عنوان IP المصدر.
4. Workstation Name — اسم الجهاز المصدر، إذا توفر.
5. Timestamp — وقت الحدث.

## Important Note

A suspicious Logon Type does not automatically mean a security breach.

نوع تسجيل الدخول وحده لا يثبت حدوث اختراق. يجب ربطه بباقي الأحداث والسياق الأمني.

