# جزوه آموزشی: طراحی محصول، UI/UX، کار با فیگما و اتصال به کد با هوش مصنوعی

---

## فصل اول: طراحی محصول (Product Design) چیست؟

* **تعریف کلان:** طراحی محصول فقط کشیدن شکل‌های زیبا نیست؛ فرآیند حل یک مشکل واقعی از کاربر است به شکلی که:


1. کارآمد و قابل استفاده باشد (کاربر در آن سردرگم نشود).


2. از نظر فنی و برنامه‌نویسی قابل پیاده‌سازی باشد.


3. به هدف تجاری یا کاربردی اپلیکیشن پاسخ دهد.




* **توسعه‌دهنده آگاه به محصول در برابر کدنویس صِرف:**
توسعه‌دهنده‌ای که منطق محصول و تجربه کاربر را بفهمد، کدهای بسیار تمیزتر، ماژولارتر و مطابق با نیاز کاربر می‌زند و برای طراحی صفحات، معطل طراح نمی‌ماند.



---

## فصل دوم: تفاوت UI و UX به زبان ساده

* **UX (User Experience - تجربه کاربری):**
* منطق، ساختار و نقشه راه تعامل کاربر با برنامه.


* پاسخ به سوال: «المان‌ها با چه ترتیبی چیده شوند تا کاربر به سریع‌ترین و راحت‌ترین شکل ممکن به هدفش برسد؟»


* مثال: تعیین اینکه دکمه اصلی کارت کجای صفحه باشد، اندازه آن متناسب با انگشت دست باشد و دسترسی به آن ساده باشد.




* **UI (User Interface - رابط کاربری):**
* ظاهر بصری، زیبایی، رنگ‌بندی، حاشیه‌ها، آیکون‌ها، فونت و فاصله‌گذاری‌ها.


* پاسخ به سوال: «صفحه چقدر تمیز، زیبا و چشم‌نواز دیده می‌شود؟»




* **وایرفریم (Wireframe):**
* نقشه و اسکلت اولیه و سیاه‌وسفید طرح روی کاغذ یا فیگما.


* هدف: مشخص کردن جایگاه اجزا قبل از ورود به جزییات رنگ و کدنویسی.





---

## فصل سوم: فیگما (Figma) چیست و ابزارهای کلیدی آن

فیگما ابزار استاندارد و ابری طراحی رابط کاربری است که طراحان و برنامه‌نویسان در سراسر جهان از آن استفاده می‌کنند.

### ابزارهای کلیدی فیگما برای برنامه‌نویسان:

1. **Frame (فریم):**
* کانتینر یا چارچوب اصلی صفحه یا بخش مشخصی از طرح (مانند صفحه موبایل یا کادر یک کارت).




2. **اشکال و متن (Shapes & Text):**
* رسم دایره (برای آواتار/عکس)، مستطیل (برای دکمه و پس‌زمینه) و نوشتن تیترها.




3. **Corner Radius و فواصل (Padding):**
* گرد کردن گوشه‌های کادرها و دکمه‌ها و تنظیم فاصله درونی متن‌ها.


4. **Auto Layout (بسیار مهم):**
* چینش خودکار عناصر به صورت افقی یا عمودی.
* **معادل برنامه‌نویسی:** اتولایوت افقی دقیقاً همان `Row` و اتولایوت عمودی همان `Column` در Jetpack Compose است.




5. **حالت توسعه‌دهنده (Dev Mode):**
* مشاهده فواصل پیکسلی، مقادیر کد رنگ‌ها (Hex)، اندازه فونت و وزن المان‌ها.



---

## فصل چهارم: روش‌های انتقال دیزاین فیگما به کد با هوش مصنوعی

برای تبدیل سریع و اصولی دیزاین فیگما به کدهای کاتلین و کامپوز، سه متد اصلی وجود دارد:

1. **روش اول: اسکرین‌شات + پرامپت ساختاریافته (رویکرد پیشنهادی کلاس)**
* گرفتن تصویر خروجی (PNG) از فریم فیگما و تحویل به ابزارهایی مثل Claude یا ChatGPT.
* **ساختار پرامپت:**
> "تو یک برنامه‌نویس ارشد اندروید هستی. این تصویر رابط کاربری را بدون تکست‌فیلد و با Jetpack Compose بنویس. فقط از کامپوننت‌های پایه مثل Card، Column، Row، Text و Button استفاده کن و مقادیر Modifier (فاصله‌ها، رنگ‌ها و گوشه‌ها) را طبق تصویر پیاده کن."
> 
> 




2. **روش دوم: پلاگین‌های فیگما به کد (Figma to Compose)**
* استفاده از پلاگین‌های آماده در فیگما برای خروجی گرفتن ساختار توابع کامپوز و بازبینی دستی کدهای تولیدشده توسط دانشجو.




3. **روش سوم: ادغام از طریق ابزارهای ایجنتی و ادیتورها**
* اتصال ابزارهایی مثل Cursor یا ایجنت‌های هوش مصنوعی به فایل طراحی برای استخراج لایه‌ها و ساخت کامپوننت‌ها.





---

## فصل پنجم: کارگاه و تمرین عملی کلاس (کارت پروفایل کاربر)

در این تمرین، از فرم‌های ورودی و تکست‌فیلد صرف‌نظر می‌کنیم تا دانشجو مستقیماً چینش بصری، فاصله‌ها و لایه‌بندی کامپوز را یاد بگیرد.

### گام اول: طراحی در فیگما

* ایجاد یک **Frame** در ابعاد ۳۲۰ در ۲۲۰ پیکسل.


* قرار دادن یک **دایره** (برای آواتار کاربر).


* نوشتن **نام و نام‌خانوادگی** و **عنوان شغلی** (مثلاً «Android Developer»).


* ساخت یک **دکمه ساده** با متن «دنبال کردن» (Follow).


* اعمال **Auto Layout عمودی** تا اجزا به شکل منظم زیر هم قرار گیرند.


* اکسپورت گرفتن به صورت فایل تصویری (PNG).

---

### گام دوم: نمونه کد خروجی Jetpack Compose (معادل طرح)

کد زیر نمونه استاندارد خروجی هوش مصنوعی است که دانشجو در اندروید استودیو قرار می‌دهد و ساختار `Row` و `Column` و `Modifier`ها را بررسی می‌کند:

```kotlin
package com.example.profilecard

import androidx.compose.foundation.background
import androidx.compose.foundation.layout.*
import androidx.compose.foundation.shape.CircleShape
import androidx.compose.foundation.shape.RoundedCornerShape
import androidx.compose.material3.*
import androidx.compose.runtime.Composable
import androidx.compose.ui.Alignment
import androidx.compose.ui.Modifier
import androidx.compose.ui.draw.clip
import androidx.compose.ui.graphics.Color
import androidx.compose.ui.text.font.FontWeight
import androidx.compose.ui.tooling.preview.Preview
import androidx.compose.ui.unit.dp
import androidx.compose.ui.unit.sp

@Composable
fun UserProfileCard() {
    Card(
        modifier = Modifier
            .padding(16.dp)
            .fillMaxWidth(),
        shape = RoundedCornerShape(16.dp),
        colors = CardDefaults.cardColors(containerColor = Color(0xFFF8FAFC)),
        elevation = CardDefaults.cardElevation(defaultElevation = 4.dp)
    ) {
        Column(
            modifier = Modifier
                .padding(20.dp)
                .fillMaxWidth(),
            horizontalAlignment = Alignment.CenterHorizontally
        ) {
            // آواتار دایره‌ای (محل تصویر پروفایل)
            Box(
                modifier = Modifier
                    .size(72.dp)
                    .clip(CircleShape)
                    .background(Color(0xFF0284C7)),
                contentAlignment = Alignment.Center
            ) {
                Text(
                    text = "A",
                    color = Color.White,
                    fontSize = 28.sp,
                    fontWeight = FontWeight.Bold
                )
            }

            Spacer(modifier = Modifier.height(12.dp))

            // نام کاربر
            Text(
                text = "علی رضایی",
                fontSize = 18.sp,
                fontWeight = FontWeight.Bold,
                color = Color(0xFF0F172A)
            )

            Spacer(modifier = Modifier.height(4.dp))

            // عنوان شغلی
            Text(
                text = "Android Developer",
                fontSize = 13.sp,
                color = Color(0xFF64748B)
            )

            Spacer(modifier = Modifier.height(16.dp))

            // دکمه اکشن (Follow)
            Button(
                onClick = { /* رویداد کلیک */ },
                shape = RoundedCornerShape(8.dp),
                colors = ButtonDefaults.buttonColors(containerColor = Color(0xFF0F172A)),
                modifier = Modifier.fillMaxWidth(0.6f)
            ) {
                Text(
                    text = "دنبال کردن",
                    fontSize = 14.sp,
                    color = Color.White
                )
            }
        }
    }
}

@Preview(showBackground = true)
@Composable
fun PreviewUserProfileCard() {
    UserProfileCard()
}

```

---

### گام سوم: چالش تغییر و یادگیری در کلاس 
**تمرین اصلاح دستی کد:** تغییر رنگ دکمه، افزایش سایز فونت یا تغییر اندازه `RoundedCornerShape` توسط دانشجو تا لمس کند که هر ویژگی در فیگما دقیقاً به کدام `Modifier` در کامپوز متصل است.
