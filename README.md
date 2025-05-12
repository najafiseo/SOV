

# Analyzing Website Rankings and Share of Voice in Google Search Using Serper.dev

This project uses the [Serper.dev](https://serper.dev) API to analyze the position and Share of Voice (SOV) of different websites in Google search results for a set of keywords.

---

## 📌 Features

- Analyze website rankings in the top 20 Google results  
- Support for multiple API keys  
- Calculate true Share of Voice (SOV) using CTR and search volume  
- Export results to Excel format  
- Pie chart visualization of competitors' share

---

## 🚀 How to Use

1. **Prepare your Excel file**. It must contain at least one column titled `Keyword`. The `Search Volume` column is optional but required for calculating **SOV**.

2. **Open the [Google Colab notebook](https://colab.research.google.com/drive/1xedEmK67jWu0kbZLa6mCPTFHZoNzF51D?usp=sharing)**.

3. **Upload your Excel file and run the code**.

4. After processing, an output file named `keyword_results_with_positions.xlsx` will be generated.

5. **At the end, the Share of Voice will be displayed both numerically and visually**.

---

## 📝 Input Excel File Format

The Excel file must contain at least one column named `Keyword` and one column for `Search Volume`.

## 🌐 Domains to Analyze

At the beginning of the code, there’s a list of domains whose rankings will be checked in the search results. You can modify this list as needed:

```python
sites_to_check = [
    "site1.com",
    "site2.com",
    "site3.com",
    "site4.com",
    "site5.com",
    "site6.com",
    "site7.com"
]
```

## 🔑 Using API Keys

To use Serper.dev, valid API keys are required. These are defined in the code as follows:

```python
API_KEYS = [
    "first_key",
    "second_key",
    ...
]
```

Each key supports up to 1,200 requests. If the limit is reached, the code will automatically switch to the next key.

---

## 📤 Final Output

After processing, an Excel file named `keyword_results_with_positions.xlsx` will be generated. This file includes:

- Website positions for each keyword: Information about where each site appears in the search results.
- Share of Voice (SOV) for each site: Calculated based on site position and search volume.
- Pie chart: Visual representation of competitors’ Share of Voice.



# بررسی موقعیت و سهم نمایش سایت‌ها در نتایج جستجوی گوگل با استفاده از Serper.dev

این پروژه با استفاده از API سرویس [Serper.dev](https://serper.dev) موقعیت (Position) و سهم نمایش (SOV - Share of Voice) سایت‌های مختلف را در نتایج جستجوی گوگل برای مجموعه‌ای از کلمات کلیدی تحلیل می‌کند.

---

## 📌 امکانات

- بررسی موقعیت سایت‌ها در ۲۰ نتیجه اول گوگل
- پشتیبانی از چند کلید API
- محاسبه سهم نمایش واقعی (SOV) با استفاده از CTR و سرچ ولوم
- خروجی به فرمت Excel
- نمودار دایره‌ای برای نمایش سهم رقبا

---

## 🚀 نحوه استفاده

1 . **فایل اکسل خود را آماده کنید**. این فایل باید حداقل دارای یک ستون با عنوان `کلمه کلیدی` باشد. ستون `سرچ ولوم` نیز اختیاری است اما برای محاسبه **SOV** مورد استفاده قرار می‌گیرد.
   
2 . **وارد  [Google Colab](https://colab.research.google.com/drive/1xedEmK67jWu0kbZLa6mCPTFHZoNzF51D?usp=sharing) شوید**.

3 . **فایل اکسل را آپلود کرده و کد را اجرا کنید**.

4 . پس از پردازش، فایل خروجی با نام `نتایج_کلمات_کلیدی_با_پوزیشن.xlsx` در اختیار شما قرار خواهد گرفت.

5 . **در پایان، سهم نمایش سایت‌ها به‌صورت عددی و نموداری نمایش داده خواهد شد**.

---

## 📝 فرمت فایل اکسل ورودی

فایل اکسل باید حداقل شامل یک ستون با نام `کلمه کلیدی` و یک ستون `سرچ ولوم` باشد،

## 🌐 دامنه‌های بررسی‌شده
در ابتدای کد، لیستی از دامنه‌ها مشخص شده که موقعیت آن‌ها در نتایج جستجو بررسی می‌شود. این لیست را می‌توانید به دلخواه تغییر دهید:

```
sites_to_check = [
    "site1.com",
    "site2.com",
    "site3com",
    "site4.com",
    "site5.com",
    "site6.com",
    "site7.com"
]
```
## 🔑 استفاده از کلیدهای API
برای استفاده از Serper.dev باید API Keyهای معتبر وارد کنید. این کلیدها به صورت زیر در کد تعریف می‌شوند:

```
API_KEYS = [
    "کلید اول",
    "کلید دوم",
    ...
]
```
هر کلید تا ۱۲۰۰ درخواست را پشتیبانی می‌کند. در صورت رسیدن به سقف، کد به‌صورت خودکار به کلید بعدی سوییچ می‌کند.


## 📤 خروجی نهایی
پس از پردازش، فایل اکسل با نام نتایج_کلمات_کلیدی_با_پوزیشن.xlsx تولید خواهد شد. این فایل شامل موارد زیر است:
-  موقعیت سایت‌ها برای هر کلمه کلیدی: اطلاعات مربوط به اینکه هر سایت در کجا در نتایج جستجو قرار دارد.
-  سهم نمایش (SOV) به‌ازای هر سایت: محاسبه سهم نمایش سایت‌ها بر اساس موقعیت آن‌ها و حجم جستجو.
-  نمودار دایره‌ای: نمایش سهم نمایش رقبا به صورت تصویری.



