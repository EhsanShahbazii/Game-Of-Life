# Game-Of-Life
بازی زندگی معروف که یه مدلسازی از اتوماتای سلولی غیر قابل پیشبینی هست که با جاوا اسکریپت پیاده سازی شده.

### بازی زندگی یعنی چی؟
به زبون ساده بازی زندگی یه بازی بدون بازیکنه! مثل بقیه بازی ها نیست که یه حریف باشه و یه نفر دیگه. اینجا سلول هامون رشد و آیندشون فقط به وضعیت و شرایطی که به دنیا اومدن داره و اصلا نیازی نداره از اون بالا بهشون بگیم تو بیا اینور تو برو اونور! انگار چند تا سلول انداختی تو ظرف و داری نگاه میکنی و دخالتی توشون نداری.

### این ایده از کجا اومده؟
حدودا توی سال 1940 جناب جان فون نیومن زندگی رو به یه صورت مهندسی تعریف کرد:

![](https://files.virgool.io/upload/users/2468585/posts/k1wbbmtedodg/botwl4mjlgut.gif)

```زندگی به صورت مخلوقی (مثل یک ارگانیزم یا یک موجود) است که میتواند تولید مثل کرده و یک ماشین تورینگ را شبیه سازی کند.```
خیلی نمیخوام وارد بحث تکنیکیش بشم اگه علاقه داشتین تو لینک میتونید بخونید. خلاصه بعدش توی سال 1968 آقای جان کانوی ریاضیدان معروف خواست یه اتوماتای سلول (cellular automaton) بسازه که پیش بینی ناپذیر باشه.

![](https://files.virgool.io/upload/users/2468585/posts/k1wbbmtedodg/vkvlzguhublm.jpg)

به زبون عامیانه میخوایم یه مدلی بسازیم که المان های توش به صورت تصادفی کارایی انجام بدن بدون اینکه از بیرون بهشون وضعیت هایی رو تشریح کنیم. به قول معروف شلم شوربا به پا کنیم :)

![](https://files.virgool.io/upload/users/2468585/posts/k1wbbmtedodg/akkfgrelap9p.gif)

بعد ها مدل ایشون پیشرفت کرد و قوانین های پیچیده تری نوشته شدن. حتی مدل از دوبعدی به سمت سه بعدی هم رفت و پیاده سازی شد. الگو های زیادی بعد از ارائه کشف شده که تعدادشون زیاده و از معروف ترین هاش میشه به گلایدر (Glider) اشاره کرد

### قوانین بازی زندگی
قانون های خیلی ساده ای داره. قطعا میشه قانون هارو دستکاری کرد و چیزای پیچیده تری براشون نوشت ولی هدف ما اینجا اینه که یه مدلسازی خیلی ساده ای داشته باشیم.

- هر سلول زنده اگه کمتر از 2 تا همسایه داشته باشه دق میکنه و میمیره!
- هر سلول زنده اگه بیشتر از 3 تا همسایه داشته باشه جامعه گریز میشه و میمیره!
- هر سلول زنده اگه 2 یا 3 تا همسایه داشته باشه به زندگی سلولیش ادامه میده :)
- هر سلول فوت کرده اگه دقیقا 3 تا همسایه داشته باشه به طور موجزه آسایی یهوی زنده میشه!
