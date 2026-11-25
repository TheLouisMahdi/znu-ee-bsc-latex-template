<div dir="rtl">

# قالب پایان‌نامهٔ کارشناسی دانشگاه زنجان | مهندسی برق

قالب قابل‌ویرایش گزارش پروژهٔ کارشناسی، شامل جلد، صفحۀ آغاز، چکیده، فهرست مطالب، پنج فصل، پیوست و منابع.

[دانلود سورس LaTeX](https://github.com/TheLouisMahdi/znu-ee-bsc-latex-template/archive/refs/heads/main.zip) · [مشاهدۀ PDF نمونه](examples/znu-ee-bsc-sample.pdf) · [دانلود نمونۀ Word](examples/znu-ee-bsc-sample.docx?raw=true)

## شروع سریع

1. سورس را از لینک بالا یا از **Code → Download ZIP** دریافت و از حالت فشرده خارج کنید. برای ساخت مخزن شخصی در گیت‌هاب، از **Use this template** استفاده کنید.
2. [مشخصات جلد](texFiles/Info.tex) و سپس [چکیده، فصل‌ها و منابع](texFiles/) را ویرایش کنید.
3. با **XeLaTeX** خروجی بگیرید. نام خروجی `thesis.pdf` است.

## ساخت آنلاین با Overleaf

1. در **New Project → Upload Project** فایل ZIP سورس را بارگذاری کنید. برای ساخت ZIP مخصوص Overleaf، `thesis.tex` و پوشه‌های `texFiles/`، `style/`، `fonts/` و `figures/` را در ریشۀ فایل فشرده بگذارید.
2. در تنظیمات پروژه، **Compiler** را روی **XeLaTeX** و **Main document** را روی `thesis.tex` بگذارید.
3. **Recompile** را بزنید. [راهنمای Overleaf](https://docs.overleaf.com/managing-projects-and-files/uploading-a-project)

## ساخت روی رایانه

[MiKTeX](https://miktex.org/download) یا [TeX Live](https://tug.org/texlive/) را نصب کنید. فرمان‌ها در پوشه‌ای اجرا می‌شوند که `thesis.tex` در آن قرار دارد.

</div>

```sh
xelatex thesis.tex
bibtex thesis
xelatex thesis.tex
xelatex thesis.tex
```

<div dir="rtl">

## قلم‌ها

- **B Nazanin** برای متن فارسی. [دریافت از برنا رایانه](https://www.bornaray.com/Content/downloads/fonts/BNAZANIN.rar). در ویندوز، پس از باز کردن آرشیو، `BNAZANIN.TTF` و `BNAZNNBD.TTF` را نصب کنید.
- **Times New Roman** برای متن لاتین. این قلم همراه محصولات سازگار Microsoft عرضه می‌شود. [مشخصات قلم](https://learn.microsoft.com/en-us/typography/font-list/times-new-roman)
- در غیاب هر قلم، قالب به‌صورت خودکار از **Amiri** برای فارسی یا **Latin Modern Roman** برای لاتین استفاده می‌کند. فایل‌های Amiri و [مجوز آن](fonts/OFL.txt) در بسته قرار دارند.

برای ساخت LaTeX با قلم‌های اصلی در Overleaf یا بدون نصب سیستمی، نسخه‌های دارای مجوز استفاده را در `fonts/local/` قرار دهید.

| قلم | نام فایل‌ها |
| --- | --- |
| B Nazanin | `BNAZANIN.TTF` و `BNAZNNBD.TTF` از آرشیو سازنده |
| B Nazanin، نام‌گذاری قبلی | `BNazanin.ttf` و `BNazanin-Bold.ttf` |
| Times New Roman | `TimesNewRoman.ttf`، `TimesNewRoman-Bold.ttf`، `TimesNewRoman-Italic.ttf`، `TimesNewRoman-BoldItalic.ttf` |

PDF نمونه با **B Nazanin** و **Times New Roman** ساخته شده است. برای همان ظاهر در Word، هر دو قلم باید روی دستگاه نصب باشند. پس از ویرایش Word، فهرست مطالب با **Update Table** به‌روز می‌شود.

## ساختار فایل‌ها

| مسیر | کاربرد |
| --- | --- |
| [`thesis.tex`](thesis.tex) | فایل اصلی و ترتیب بخش‌ها |
| [`texFiles/Info.tex`](texFiles/Info.tex) | مشخصات جلد و تاریخ دفاع |
| [`texFiles/`](texFiles/) | چکیده، فصل‌ها، پیوست و [منابع BibTeX](texFiles/References.bib) |
| [`style/znu-ee.sty`](style/znu-ee.sty) | صفحه‌آرایی و تنظیم قلم‌ها |
| [`figures/`](figures/) | شکل‌ها و نشان اختیاری جلد با نام `university-logo.pdf` |
| [`fonts/`](fonts/) | قلم فارسی همراه قالب و مجوز آن |
| [`examples/`](examples/) | نمونه‌های PDF و Word |

قالب با الهام از [قالب دانشگاه زنجان اثر بهمن میرزاخانی](https://github.com/bahman-mirzakhani/znu-thesis-LaTeX-template) آماده شده است. برای تحویل نهایی، شیوه‌نامۀ جاری گروه ملاک است.

## مجوز

کد LaTeX، راهنما و محتوای تألیفی نمونه‌ها با [مجوز MIT](LICENSE) منتشر شده‌اند. استفاده، ویرایش و بازنشر با حفظ اعلان حق نشر و متن مجوز مجاز است. فایل‌های قلم Amiri تابع [SIL Open Font License 1.1](fonts/OFL.txt) هستند. B Nazanin و Times New Roman تابع شرایط سازندگان خود هستند.

</div>
