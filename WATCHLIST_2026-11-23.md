# فهرست دیده‌بانی اولیه — 2026-11-23

**تاریخ snapshot:** 23 Nov 2026  
**هدف:** ایجاد baseline برای مقایسه روزهای بعد؛ اعداد با داده جدید جایگزین شوند، نه اینکه بدون تاریخ روی هم انباشته شوند.  
**وضعیت:** تحقیق اولیه؛ هیچ‌کدام تأیید خرید نیستند.

---

## خلاصه اولویت

| اولویت تحقیق | پروژه | روایت | وضعیت اولیه | دلیل اصلی |
|---:|---|---|---|---|
| 1 | NEAR | Intents / solver economy | Research Priority با ریسک عملیاتی | استفاده و fee capture قابل مشاهده |
| 2 | NOS | GPU compute / DePIN | Watchlist | job و GPU-hour قابل مشاهده؛ مشتری پولی نیازمند اثبات |
| 3 | ACU | mobile compute / DePIN | Watchlist با هشدار شدید عرضه/نقدشوندگی | دستگاه و deployment فعال؛ unlock و spot liquidity ضعیف |
| 4 | ZAMA | FHE / privacy compute | Watchlist | فعالیت مهندسی؛ TVL و unlock ریسک دارند |
| 5 | NIGHT | privacy L1 | Discovery / Watch | توسعه node و SDK؛ استقلال اپراتورها هنوز محدود |

---

## 1. NEAR — Intents

### شواهد استفاده و اقتصاد
- 30D volume حدود $3.904B.
- 30D unique users حدود 197,025.
- حدود 1.77M swap طی 30 روز.
- 30D gross fees حدود $7.4M طبق NearStats/DefiLlama؛ gross fees را با درآمد خالص پروتکل اشتباه نگیریم.
- 30D net revenue حدود 433,541 NEAR طبق DefiLlama؛ مقدار دلاری آن باید با قیمت همان زمان محاسبه شود.
- Holders revenue/buyback در 30 روز نیز حدود 433,541 NEAR گزارش شده؛ خرید بازار با burn یکی نیست.
- TVL از حدود $201.5M در 24 اکتبر به $151.82M در 22 نوامبر رسیده؛ افت حدود 24.7%.

### ریسک و نکات منفی
- گزارش Reddit از exploit حدود $3.8M در اکتبر 2026 و توقف موقت برخی مسیرها منتشر شده؛ باید postmortem رسمی، جبران خسارت و وضعیت امنیتی را بررسی کرد.
- گزارش‌های کاربران درباره stuck swaps و پشتیبانی ضعیف وجود دارد؛ این‌ها ادعاهای کاربران‌اند و نیاز به تفکیک موارد تأییدشده از تجربه‌های موردی دارند.
- GitHub مخزن near/near-intents که در بررسی سریع دیده شد، عمدتاً landing-page است؛ activity آن را نباید به core protocol نسبت داد.
- افت TVL در نوامبر هشدار adoption/retention است.

### حکم
از نظر تقاضای قابل مشاهده و مسیر buyback جذاب‌ترین نامزد این snapshot است، اما امنیت cross-chain، شکایات تسویه و افت TVL باید قبل از هر تصمیم حل‌وفصل شوند.

منابع:
- DefiLlama: https://defillama.com/protocol/near-intents
- NearStats: https://nearstats.org/near-intents/fees
- NearStats monthly: https://nearstats.org/near-intents/monthly
- NEAR revenue dashboard: https://revenue.near.org/
- GitHub: https://github.com/near/near-intents
- Reddit incident discussion: https://www.reddit.com/r/CryptoCurrency/comments/1wv0qdd/near_intents_a_crosschain_swap_service_built_on/

---

## 2. NOS — Nosana

### شواهد شبکه
- داشبورد رسمی: حدود 4,231,806 job تکمیل‌شده.
- حدود 1,010 job در حال اجرا و 475 در صف.
- مجموع job hours حدود 4,486,355.
- GPU compute hours در ماه گذشته حدود 208,810.
- CoinMarketCap snapshot: قیمت حدود $0.31، market cap حدود $22.93M، 24h volume حدود $463K، total supply حدود 99.99M و circulating حدود 73.97M؛ منابع دیگر 100M circulating نشان می‌دهند، بنابراین عرضه در منابع اختلاف دارد و باید on-chain تطبیق شود.
- سایت رسمی توکن: حدود 13,544 stakers و $3.78M ارزش استیک‌شده در یک snapshot دیگر؛ اعداد سایت با CMC/CG هم‌زمان نیستند و باید timestamp کنارشان ثبت شود.
- Kairos Signal: 11 GitHub contributors و حدود 25 روز از آخرین push در snapshot 21 نوامبر.

### شواهد مستقل سازنده
- Reddit، 14 نوامبر؟ یک سازنده مستقل در r/Nosana_AI گزارش کرده: 84 GPU hours، 57 jobs، 32 agents و 25 accounts از آگوست 2026. نمونه کوچک است، اما از نظر کیفیت شواهد از آمار کلی تبلیغاتی بهتر است؛ هنوز درآمد و پرداخت واقعی باید تأیید شود.

### ریسک و نکات منفی
- completed jobs و GPU hours به‌تنهایی اثبات مشتریان پولی و تکرار خرید نیست.
- مخزن GitHub که بررسی شد عمدتاً docs بود؛ برای ارزیابی engineering باید repoهای core/node/program را جدا پیدا کرد.
- تاریخچه قیمت نسبت به ATH بسیار افت کرده؛ این به معنی undervaluation نیست.

### حکم
نامزد microcap برای بررسی بیشتر؛ شرط ارتقا: اثبات هزینه‌کرد مشتریان مستقل، retention، GPU utilization و پرداخت واقعی به hostها. عرضه 100M در منابع رسمی تقریباً کامل آزاد شده، اما باید توزیع هولدر و قفل واقعی را بررسی کرد.

منابع:
- Explorer: https://explore.nosana.com/
- Token page: https://nosana.com/nosana-token/
- Token docs: https://learn.nosana.com/programs/token.html
- CoinMarketCap: https://coinmarketcap.com/currencies/nosana/
- Kairos Signal: https://kairossignal.com/network/NOS
- Reddit builder log: https://www.reddit.com/r/Nosana_AI/comments/1xsazf3/build_log_voight_agents_oneclick_ai_agents_on/

---

## 3. ACU — Acurast

### شواهد شبکه
- Acurast Pulse: 53.7K deployments در 30 روز، حدود 1,790 در روز.
- 54 deployer متمایز؛ این تمرکز تقاضا را نشان می‌دهد.
- 3,636 deployment در execution window جاری در snapshot.
- داشبورد شبکه در بررسی قبلی: 245,110 دستگاه شناخته‌شده، 37,518 دستگاه آنلاین، 15,557 دستگاه دارای deployment؛ این ارقام باید روزانه refresh شوند.

### توکنومیکس و نقدشوندگی
- عرضه اولیه کل 1B ACU.
- مدل رسمی: 5% تورم ثابت سالانه؛ 70% به Staked Compute Pool، 10% Compute Pool، 15% Treasury و 5% Collators.
- Tokenomics.com: unlock بعدی 20 دسامبر 2026؛ 26.7M ACU، معادل 2.7% عرضه کل و حدود 5.5% market cap؛ recipientها Foundation، insiders، investors و community.
- CoinGlass snapshot: market cap حدود $49.3M، FDV حدود $113M، spot volume حدود $79.6K و futures volume حدود $1.57M؛ futures تقریباً 20 برابر spot. این وضعیت برای ورود/خروج موقعیت جدی نامناسب است.
- CoinGecko order-book data نیز عمق ±2% پایین در چند venue نشان می‌دهد.

### حکم
از نظر رشد اپراتور/دستگاه جذاب؛ اما فعلاً hard gate نقدشوندگی و unlock را رد نمی‌کند. تا پس از unlock و بهبود عمق spot، فقط Watchlist.

منابع:
- Pulse: https://www.acurastpulse.com/analytics/workload
- Tokenomics official: https://docs.acurast.com/tokenomics/
- Unlock schedule: https://app.tokenomics.com/tokenomics/acurast/unlocks
- CoinGlass: https://www.coinglass.com/currencies/ACU/spot
- CoinGecko: https://www.coingecko.com/en/coins/acurast
- Reddit device operator research: https://www.reddit.com/r/Nordic_Crypto/comments/1xw5sei/updated_list_of_compatible_phones_for_acurast/

---

## 4. ZAMA — Zama

### شواهد فنی
- مخزن FHEVM دارای commitهای فنی قابل مشاهده در connector بررسی‌شده بود؛ از جمله KMS connector tests، permissionless submit paths و pad-worker.
- نمونه مخزن: https://github.com/zama-ai/fhevm
- مخزن دوم: https://github.com/zama-ai/tfhe-rs

### توکنومیکس و ریسک
- tokenomics.com snapshot: 11B total supply؛ حدود 2.57B در گردش (23.4%).
- unlock بعدی 2 دسامبر 2026: 114.6M ZAMA؛ حدود 1% عرضه کل و 3.5% market cap.
- unlock فوریه 2027 در تقویم منبع حدود 19.2% market cap نشان داده شده؛ باید با اسناد رسمی و تعریف درصد دوباره تأیید شود.
- TVL در گزارش 22 نوامبر حدود $75.5M بوده و در یک ماه افت محسوس داشته است.

### حکم
فناوری و فعالیت توسعه‌دهنده جذاب؛ اما توکن با float پایین و unlockهای مهم روبه‌روست. در حال حاضر Watchlist، نه Entry Candidate.

منابع:
- GitHub FHEVM: https://github.com/zama-ai/fhevm
- GitHub TFHE-rs: https://github.com/zama-ai/tfhe-rs
- Unlocks: https://app.tokenomics.com/tokenomics/zama/unlocks
- DefiLlama: https://defillama.com/

---

## 5. NIGHT — Midnight

### شواهد فنی/اپراتوری
- مخازن رسمی node و JS SDK:
  - https://github.com/midnightntwrk/midnight-node
  - https://github.com/midnightntwrk/midnight-js
- بررسی GitHub نشان‌دهنده تغییرات واقعی در devnet chain-spec، runtime و Rust dependencies است.
- طبق برنامه اعلام‌شده، تولید بلاک در شروع به اپراتورهای مجاز محدود بوده و گسترش به اپراتورهای مستقل در Q1 2027 هدف‌گذاری شده است؛ برنامه را با اجرای واقعی اشتباه نگیریم.

### حکم
برای رصد توسعه privacy infrastructure مناسب است؛ اما تا اثبات استقلال اپراتورها، تقاضای واقعی و token value capture در وضعیت Discovery/Watch باقی بماند.

منابع:
- Node: https://github.com/midnightntwrk/midnight-node
- JS SDK: https://github.com/midnightntwrk/midnight-js
- Docs: https://docs.midnight.network/

---

## اصلاحات مهم نسبت به گزارش‌های اولیه

1. NEAR: رقم 433,541 در DefiLlama واحد NEAR است، نه دلار. Gross fees حدود $7.4M است و نباید با net revenue یا holders revenue یکی گرفته شود.
2. NOS: عدد job و GPU-hour به معنی revenue نیست. باید مشتری پرداخت‌کننده و invoice/payment اثبات شود.
3. ACU: داده‌های spot و futures اختلاف بزرگی دارند و unlock 20 دسامبر 2026 باید در تصمیم لحاظ شود.
4. GitHub: تعداد commitها بدون بررسی نوع مخزن گمراه‌کننده است؛ near/near-intents در نمونه بررسی‌شده landing page بود، درحالی‌که Zama FHEVM تغییرات فنی core داشت.
5. Social: نمونه‌های Reddit برای Nosana یک builder مستقل و برای NEAR شکایت/حادثه امنیتی را نشان می‌دهند؛ این دو نوع سیگنال باید هم‌زمان دیده شوند، نه فقط sentiment مثبت.

## اقدام بعدی

- بررسی postmortem و جبران خسارت NEAR Intents.
- یافتن repoهای core واقعی Nosana و بررسی آخرین commitهای فنی.
- بررسی مشتریان پرداخت‌کننده و اقتصاد واحد Nosana.
- مانیتور کردن ACU unlock و افزایش spot depth.
- تطبیق ZAMA unlockها با سند رسمی و بررسی ارزش‌گیری توکن.
