<div dir="rtl">

# قالب پایان‌نامهٔ کارشناسی دانشگاه زنجان | مهندسی برق

این قالب نقطهٔ شروع نگارش گزارش پروژهٔ کارشناسی گروه مهندسی برق دانشگاه زنجان است. ترتیب سند شامل جلد، صفحهٔ آغاز، چکیدهٔ فارسی، فهرست مطالب، فصل‌ها، پیوست و منابع است. این قالب یک نمونهٔ قابل ویرایش برای دانشجویان است. جزئیات جلد و صفحه‌آرایی را می‌توان با آخرین دستورالعمل گروه تطبیق داد.

## نمونه‌های قالب

[مشاهدۀ PDF نمونه](examples/znu-ee-bsc-sample.pdf) · [دانلود نمونۀ قابل‌ویرایش Word](examples/znu-ee-bsc-sample.docx?raw=true)

نمونۀ PDF با قلم‌های **B Nazanin** و **Times New Roman** از همین قالب LaTeX ساخته شده است. برای حفظ ظاهر نسخۀ Word، هر دو قلم روی رایانه نصب شوند. فهرست مطالب Word پس از ویرایش متن از گزینۀ **Update Table** به‌روزرسانی می‌شود.

## شروع

1. در گیت‌هاب گزینهٔ **Use this template** را انتخاب کنید، یا سورس را از **Code → Download ZIP** دریافت کنید.
2. عنوان پروژه، نام دانشجو، نام استاد راهنما، گرایش و تاریخ دفاع را در [مشخصات جلد](texFiles/Info.tex) وارد کنید.
3. متن نمونهٔ فایل‌های [چکیده و فصل‌ها](texFiles/) را با متن پروژه جایگزین کنید و منابع را در [فایل BibTeX](texFiles/References.bib) ثبت کنید. برای هر ارجاع از `\cite{کلید}` استفاده کنید.
4. برای درج نشان دانشگاه روی جلد، فایل PDF آن را با نام `figures/university-logo.pdf` در پروژه قرار دهید.

## ساخت PDF

یک توزیع به‌روز TeX Live یا MiKTeX با XePersian و سبک کتاب‌نامهٔ `unsrt-fa` لازم است. فرمان‌های زیر در پوشهٔ اصلی پروژه اجرا می‌شوند و خروجی `thesis.pdf` را می‌سازند. در Overleaf فایل اصلی `thesis.tex` و کامپایلر **XeLaTeX** انتخاب می‌شوند.

</div>

```sh
xelatex thesis.tex
bibtex thesis
xelatex thesis.tex
xelatex thesis.tex
```

<div dir="rtl">

## قلم‌های قالب

**B Nazanin** برای متن فارسی و **Times New Roman** برای متن لاتین پیش‌فرض هستند. برای ساخت روی رایانه، هر دو قلم و نسخۀ پررنگ B Nazanin را نصب کنید.

در Overleaf، فایل‌های قلم را که مجاز به استفاده از آن‌ها هستید در پوشۀ `fonts/local/` بارگذاری کنید. نام فایل‌ها باید به این صورت باشد.

| قلم | نام فایل‌ها در `fonts/local/` |
| --- | --- |
| B Nazanin | `BNazanin.ttf`، `BNazanin-Bold.ttf` |
| Times New Roman | `TimesNewRoman.ttf`، `TimesNewRoman-Bold.ttf`، `TimesNewRoman-Italic.ttf`، `TimesNewRoman-BoldItalic.ttf` |

برای ساخت با قلم‌های جایگزین **Amiri** و **Latin Modern Roman**، خط فراخوانی سبک در `thesis.tex` را به `\usepackage[portablefonts]{style/znu-ee}` تغییر دهید. قلم Amiri و مجوز آن در [پوشۀ قلم‌ها](fonts/) قرار دارند.

## ساختار فایل‌ها

| مسیر | کاربرد |
| --- | --- |
| [`thesis.tex`](thesis.tex) | فایل اصلی و ترتیب بخش‌ها |
| [`texFiles/Info.tex`](texFiles/Info.tex) | اطلاعات صفحهٔ عنوان |
| [`texFiles/`](texFiles/) | چکیده، فصل‌ها، پیوست و فایل منابع |
| [`style/znu-ee.sty`](style/znu-ee.sty) | صفحه‌آرایی، قلم‌ها و دستورهای فارسی |
| [`figures/`](figures/) | محل نشان دانشگاه و شکل‌های پروژه |

این قالب با الهام از [قالب LaTeX دانشگاه زنجان اثر بهمن میرزاخانی](https://github.com/bahman-mirzakhani/znu-thesis-LaTeX-template) آماده شده است. قلم فارسی جایگزین از [پروژهٔ Amiri](https://github.com/aliftype/amiri/releases/tag/1.003) دریافت شده است.

</div>
