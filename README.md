# نظام اللجان الامتحانية

نظام متكامل لإدارة درجات الطلاب في اللجان الامتحانية، مبني باستخدام Flask و SQLAlchemy.

## الميزات الرئيسية

- واجهة تسجيل دخول للتدريسيين والطلاب
- لوحة تحكم للتدريسيين لإدارة درجات الطلاب
- لوحة عرض للطلاب لمشاهدة درجاتهم
- إمكانية البحث عن طالب معين
- عرض ملخص الدرجات لكل كورس
- دعم للتصميم المتجاوب مع جميع الأجهزة
- تأثيرات حركية وواجهة مستخدم جذابة

## متطلبات التشغيل

- Python 3.8 أو أحدث
- متصفح ويب حديث

## طريقة الإعداد والتشغيل

1. قم بتثبيت المتطلبات:

```
pip install -r requirements.txt
```

2. قم بتشغيل التطبيق:

```
python app.py
```

3. افتح المتصفح على العنوان:

```
http://localhost:5000
```

## بيانات تسجيل الدخول الافتراضية

### تدريسي
- اسم المستخدم: instructor
- كلمة المرور: password

### طلاب
- اسم المستخدم: ahmed, fatima, ali, zainab, hassan, noor, mohammed, sara, omar
- كلمة المرور: password

## هيكل المشروع

- `app.py`: الملف الرئيسي للتطبيق
- `templates/`: قوالب HTML
- `static/`: الملفات الثابتة (CSS, JavaScript)
- `examination.db`: قاعدة البيانات

## قاعدة البيانات

يستخدم النظام قاعدة بيانات SQLite مع النماذج التالية:
- `User`: معلومات المستخدمين (تدريسيين وطلاب)
- `Student`: معلومات الطلاب
- `Course`: المواد الدراسية
- `Grade`: درجات الطلاب

## الواجهات

1. **واجهة تسجيل الدخول**: تتيح للمستخدم اختيار نوع الحساب (تدريسي أو طالب) وإدخال بيانات الدخول.
2. **لوحة التدريسي**: تعرض قائمة بالمراحل والكورسات، وتتيح تعديل درجات الطلاب.
3. **لوحة الطالب**: تعرض درجات الطالب في جميع المراحل والكورسات.
