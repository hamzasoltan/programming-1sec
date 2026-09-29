# Programming Course

## الملفات الأساسية
- `index.html` — الموقع الرئيسي.
- `links.json` — جميع روابط المحتوى وإعدادات المراحل.
- `test1.html` ... `test13.html` — ملفات اختبارات الـ Chapters.
- اختبارات المراجعات لها أسماء منفصلة داخل `links.json`.

## نظام الفتح
- Chapter 1 مفتوح افتراضيًا.
- كل مرحلة تالية تُفتح بعد اجتياز المرحلة السابقة.
- درجة النجاح: 60%.
- حالة التقدم محفوظة في LocalStorage.

## تعديل الروابط
عدّل فقط القيم داخل `links.json`:
- `book`
- `summary`
- `video`
- `exam`

مثال:
```json
"chapter-1": {
  "title": "Chapter 1",
  "type": "chapter",
  "book": "Chapter 1.pdf",
  "summary": "Chapter 1 Summary.pdf",
  "video": "Chapter 1.mp4",
  "exam": "test1.html"
}
```

## ملاحظة مهمة
ملفات الاختبارات يجب أن تُحدّث حالة النجاح في LocalStorage بالمفتاح:
`programmingCourseProgress`

وقيمة المرحلة تكون مثل:
`{"passed": true, "score": 80}`
