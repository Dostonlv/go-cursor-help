# 🚀 Cursor Bepul Sinov Muddatini Tiklash Vositasi

<div align="center">

[![Release](https://img.shields.io/github/v/release/yuaotian/go-cursor-help?style=flat-square&logo=github&color=blue)](https://github.com/yuaotian/go-cursor-help/releases/latest)
[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&logo=bookstack)](https://github.com/yuaotian/go-cursor-help/blob/master/LICENSE)
[![Stars](https://img.shields.io/github/stars/yuaotian/go-cursor-help?style=flat-square&logo=github)](https://github.com/yuaotian/go-cursor-help/stargazers)

[🌟 English](README.md) | [🌏 中文](README_CN.md) | [🌏 日本語](README_JP.md) | [🌏 O'zbek](README_UZ.md)

<img src="https://ai-cursor.com/wp-content/uploads/2024/09/logo-cursor-ai-png.webp" alt="Cursor Logo" width="120"/>

</div>

> ⚠️ **MUHIM ESLATMA**
> 
> Ushbu vosita hozirda quyidagilarni qo'llab-quvvatlaydi:
> - ✅ Cursor v0.45.x va undan pastroq versiyalar
> - ✅ Windows: Eng so'nggi 0.47.x versiyalari (Qo'llab-quvvatlanadi)
> - ✅ Mac/Linux: Eng so'nggi 0.47.x versiyalari (Qo'llab-quvvatlanadi, fikr-mulohazalar kutilmoqda)
>
> Iltimos, ushbu vositadan foydalanishdan oldin Cursor versiyangizni tekshiring.

<details open>
<summary><b>📦 Versiya tarixi va yuklab olishlar</b></summary>

<div class="version-card" style="background: linear-gradient(135deg, #6e8efb, #a777e3); border-radius: 8px; padding: 15px; margin: 10px 0; color: white;">

### 🌟 Eng so'nggi versiyalar
- v0.45.11 (2025-02-07) - Eng so'nggi reliz
- v0.45.x (2025-01-03) - Eng barqaror reliz

[To'liq versiya tarixini ko'rish](CursorHistoryDown.md)

</div>

### 📥 To'g'ridan-to'g'ri yuklab olish havolalari

**v0.45.x (Tavsiya etilgan barqaror versiya)**
- Windows: [Rasmiy](https://downloader.cursor.sh/builds/250103fqxdt5u9z/windows/nsis/x64) | [Zerkalo](https://download.todesktop.com/230313mzl4w4u92/Cursor%20Setup%200.44.11%20-%20Build%20250103fqxdt5u9z-x64.exe)
- Mac: [Apple Silicon](https://dl.todesktop.com/230313mzl4w4u92/versions/0.44.11/mac/zip/arm64)

</details>

⚠️ **MAC manzilini o'zgartirish haqida ogohlantirish**
> 
> Mac foydalanuvchilari uchun: Ushbu skript MAC manzilini o'zgartirish xususiyatini o'z ichiga oladi, bu:
> - Tarmoq interfeysining MAC manzilini o'zgartiradi
> - O'zgartirishdan oldin asl MAC manzillarini zaxiralaydi
> - Bu o'zgartirish vaqtincha tarmoq ulanishiga ta'sir qilishi mumkin
> - Skriptni ishga tushirish paytida so'ralganda, bu qadamni o'tkazib yuborishingiz mumkin
>
> 💾 **Cursor v0.45.x ni yuklab olish**
> 
> Windows:
> - [Cursor rasmiy saytidan yuklab olish](https://downloader.cursor.sh/builds/250103fqxdt5u9z/windows/nsis/x64)
> - [ToDesktop dan yuklab olish](https://download.todesktop.com/230313mzl4w4u92/Cursor%20Setup%200.44.11%20-%20Build%20250103fqxdt5u9z-x64.exe)
>
> Mac:
> - [Mac uchun yuklab olish (Apple Silicon)](https://dl.todesktop.com/230313mzl4w4u92/versions/0.44.11/mac/zip/arm64)

<details >
<summary><b>🔒 Avtomatik yangilash funksiyasini o'chirish</b></summary>

> Cursor dasturining qo'llab-quvvatlanmaydigan yangi versiyalariga avtomatik yangilanishini oldini olish uchun, avtomatik yangilash funksiyasini o'chirib qo'yishingiz mumkin.

#### 1-usul: O'rnatilgan skriptdan foydalanish (Tavsiya etiladi)

Tiklash vositasini ishga tushirganda, skript sizdan avtomatik yangilashlarni o'chirishni xohlaysizmi deb so'raydi:
```text
[Savol] Cursor avtomatik yangilash funksiyasini o'chirishni xohlaysizmi?
0) Yo'q - Standart sozlamalarni saqlash (Enter tugmasini bosing)
1) Ha - Avtomatik yangilashni o'chirish
```

Avtomatik o'chirish operatsiyasini yakunlash uchun `1` ni tanlang.

#### 2-usul: Qo'lda o'chirish

**Windows:**
1. Barcha Cursor jarayonlarini yoping
2. Quyidagi katalogni o'chiring: `%LOCALAPPDATA%\cursor-updater`
3. Xuddi shu joyda xuddi shu nomdagi fayl yarating (kengaytmasiz)

**macOS:**
```bash
# ESLATMA: Sinab ko'rilganidek, bu usul faqat 0.45.11 va undan pastroq versiyalar uchun ishlaydi.
# Cursor ni yoping
pkill -f "Cursor"
# app-update.yml faylini bo'sh/faqat o'qish uchun fayl bilan almashtirish
cd /Applications/Cursor.app/Contents/Resources
mv app-update.yml app-update.yml.bak
touch app-update.yml
chmod 444 app-update.yml

# Sozlamalar -> Ilova -> Yangilash bo'limiga o'ting, Rejimni "none" ga o'rnating.
# Bu Cursor ga yangilanishlarni tekshirishini oldini olish uchun qilinishi kerak.

# ESLATMA: cursor-updater ni o'zgartirish usuli endi samarali bo'lmasligi mumkin
# Har qanday holatda, yangilash katalogini o'chirib tashlang va bloklash faylini yarating
rm -rf ~/Library/Application\ Support/Caches/cursor-updater
touch ~/Library/Application\ Support/Caches/cursor-updater
```

**Linux:**
```bash
# Cursor ni yoping
pkill -f "Cursor"
# Yangilash katalogini o'chirib tashlang va bloklash faylini yarating
rm -rf ~/.config/cursor-updater
touch ~/.config/cursor-updater
```

> ⚠️ **Eslatma:** Avtomatik yangilashlarni o'chirgandan so'ng, yangi versiyalarni qo'lda yuklab olishingiz va o'rnatishingiz kerak bo'ladi. Yangi versiya mos kelishini tasdiqlangandan so'nggina yangilash tavsiya etiladi.


</details>

---

### 📝 Tavsif

> Quyidagi xabarlardan birini uchratganingizda:

#### Muammo 1: Sinov hisob qaydnomasi cheklovi <p align="right"><a href="#issue1"><img src="https://img.shields.io/badge/Yechimga%20o'tish-Blue?style=plastic" alt="Back To Top"></a></p>

```text
Too many free trial accounts used on this machine.
Please upgrade to pro. We have this limit in place
to prevent abuse. Please let us know if you believe
this is a mistake.
```

#### Muammo 2: API kalit cheklovi <p align="right"><a href="#issue2"><img src="https://img.shields.io/badge/Yechimga%20o'tish-green?style=plastic" alt="Back To Top"></a></p>

```text
[Yangi muammo]

[New Issue]

Composer relies on custom models that cannot be billed to an API key.
Please disable API keys and use a Pro or Business subscription.
Request ID: xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
```

#### Muammo 3: Sinov so'rovlari cheklovi

> Bu VIP bepul sinov davri mobaynida foydalanish chekloviga yetganingizni ko'rsatadi:

```text
You've reached your trial request limit.
```

#### Muammo 4: Claude 3.7 yuqori yuk <p align="right"><a href="#issue4"><img src="https://img.shields.io/badge/Yechimga%20o'tish-purple?style=plastic" alt="Back To Top"></a></p>

```text
High Load 
We're experiencing high demand for Claude 3.7 Sonnet right now. Please upgrade to Pro, or switch to the
'default' model, Claude 3.5 sonnet, another model, or try again in a few moments.
```

<br>

<p id="issue2"></p>

#### Yechim: Cursor ni to'liq o'chirib tashlang va qayta o'rnating (API kalit muammosi)

1. [Geek.exe Uninstaller[Bepul]](https://geekuninstaller.com/download) ni yuklab oling
2. Cursor ilovasini to'liq o'chirib tashlang
3. Cursor ilovasini qayta o'rnating
4. 1-Yechimga davom eting

<br>

<p id="issue1"></p>

> Vaqtinchalik yechim:

#### Yechim 1: Tezkor tiklash (Tavsiya etiladi)

1. Cursor ilovasini yoping
2. Mashina kodi tiklash skriptini ishga tushiring (quyidagi o'rnatish ko'rsatmalariga qarang)
3. Foydalanishda davom etish uchun Cursor ni qayta oching

#### Yechim 2: Hisob qaydnomasini almashtirish

1. Fayl -> Cursor Sozlamalari -> Chiqish
2. Cursor ni yoping
3. Mashina kodi tiklash skriptini ishga tushiring
4. Yangi hisob qaydnomasi bilan tizimga kiring

#### Yechim 3: Tarmoq optimizatsiyasi

Agar yuqoridagi yechimlar ishlamasa, quyidagilarni sinab ko'ring:

- Past kechikishli serverlarga o'ting (Tavsiya etilgan mintaqalar: Yaponiya, Singapur, AQSH, Gonkong)
- Tarmoq barqarorligini ta'minlang
- Brauzer keshini tozalang va qayta urinib ko'ring

#### Yechim 4: Claude 3.7 ga kirish muammosi (Yuqori yuk)

Agar Claude 3.7 Sonnet uchun "Yuqori yuk" xabarini ko'rsangiz, bu Cursor bepul sinov hisob qaydnomalarini kunning ma'lum vaqtlarida 3.7 modelidan foydalanishini cheklayotganini ko'rsatadi. Quyidagilarni sinab ko'ring:

1. Gmail orqali yaratilgan yangi hisob qaydnomasiga o'ting, balki boshqa IP manzil orqali ulanib ko'ring
2. Kam band soatlarda kirish uchun harakat qiling (odatda 5-10 ertalab yoki 3-7 kechqurun, cheklovlar ko'pincha yengilroq bo'lgan paytda)
3. Kafolatlangan kirish uchun Pro versiyaga yangilashni o'ylab ko'ring
4. Zaxira variant sifatida Claude 3.5 Sonnet dan foydalaning

> Eslatma: Cursor resurslarni taqsimlash siyosatini o'zgartirishi bilan bu kirish naqshlari o'zgarishi mumkin.

### 💻 Tizim qo'llab-quvvatlash

<table>
<tr>
<td>

**Windows** ✅

- x64 (64-bit)
- x86 (32-bit)

</td>
<td>

**macOS** ✅

- Intel (x64)
- Apple Silicon (M1/M2)

</td>
<td>

**Linux** ✅

- x64 (64-bit)
- x86 (32-bit)
- ARM64

</td>
</tr>
</table>

### 🚀 Bir marta bosish yechimi

<details open>
<summary><b>Global foydalanuvchilar</b></summary>

**macOS**

```bash
# Ikkinchi usul
curl -fsSL https://aizaozao.com/accelerate.php/https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_mac_id_modifier.sh -o ./cursor_mac_id_modifier.sh && sudo bash ./cursor_mac_id_modifier.sh && rm ./cursor_mac_id_modifier.sh
```

**Linux**

```bash
curl -fsSL https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_linux_id_modifier.sh | sudo bash 
```

**Windows**

```powershell
irm https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_win_id_modifier.ps1 | iex
```

<div align="center">
<img src="img/run_success.png" alt="Run Success" width="600"/>
</div>

</details>

<details open>
<summary><b>Xitoy foydalanuvchilari (Tavsiya etiladi)</b></summary>

**macOS**

```bash
curl -fsSL https://aizaozao.com/accelerate.php/https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_mac_id_modifier.sh -o ./cursor_mac_id_modifier.sh && sudo bash ./cursor_mac_id_modifier.sh && rm ./cursor_mac_id_modifier.sh
```

**Linux**

```bash
curl -fsSL https://aizaozao.com/accelerate.php/https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_linux_id_modifier.sh | sudo bash
```

**Windows**

```powershell
irm https://aizaozao.com/accelerate.php/https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_win_id_modifier.ps1 | iex
```

</details>

<details open>
<summary><b>Windows Terminal ishga tushirish va konfiguratsiya</b></summary>

#### Windows da administrator terminalni qanday ochish mumkin:

##### 1-usul: Win + X tugmachasidan foydalanish
```md
1. Win + X tugmachalar kombinatsiyasini bosing
2. Menyudan quyidagi variantlardan birini tanlang:
   - "Windows PowerShell (Administrator)"
   - "Windows Terminal (Administrator)"
   - "Terminal (Administrator)"
   (Variantlar Windows versiyasiga qarab farq qilishi mumkin)
```

##### 2-usul: Win + R ishga tushirish buyrug'idan foydalanish
```md
1. Win + R tugmachalar kombinatsiyasini bosing
2. Ishga tushirish oynasiga powershell yoki pwsh kiriting
3. Administrator sifatida ishga tushirish uchun Ctrl + Shift + Enter tugmalarini bosing
   yoki ochilgan oynaga quyidagini kiriting: Start-Process pwsh -Verb RunAs
4. Administrator terminaliga tiklash skriptini kiriting:

irm https://aizaozao.com/accelerate.php/https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_win_id_modifier.ps1 | iex
```

##### 3-usul: Qidiruvdan foydalanish
>![PowerShell qidirish](img/pwsh_1.png)
>
>Qidiruv maydoniga pwsh kiriting, o'ng tugmani bosing va "Run as administrator" (Administrator sifatida ishga tushirish) ni tanlang
>![Run as Administrator](img/pwsh_2.png)

Administrator terminaliga tiklash skriptini kiriting:
```powershell
irm https://aizaozao.com/accelerate.php/https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_win_id_modifier.ps1 | iex
```

### 🔧 PowerShell o'rnatish qo'llanmasi 

Agar PowerShell tizimingizga o'rnatilmagan bo'lsa, quyidagi usullardan biri orqali o'rnatishingiz mumkin:

#### 1-usul: Winget orqali o'rnatish (Tavsiya etiladi)

1. Command Prompt yoki PowerShell ni oching
2. Quyidagi buyruqni ishga tushiring:
```powershell
winget install --id Microsoft.PowerShell --source winget
```

#### 2-usul: Qo'lda o'rnatish

1. Tizimingiz uchun mos o'rnatuvchini yuklab oling:
   - [PowerShell-7.4.6-win-x64.msi](https://github.com/PowerShell/PowerShell/releases/download/v7.4.6/PowerShell-7.4.6-win-x64.msi) (64-bit tizimlar)
   - [PowerShell-7.4.6-win-x86.msi](https://github.com/PowerShell/PowerShell/releases/download/v7.4.6/PowerShell-7.4.6-win-x86.msi) (32-bit tizimlar)
   - [PowerShell-7.4.6-win-arm64.msi](https://github.com/PowerShell/PowerShell/releases/download/v7.4.6/PowerShell-7.4.6-win-arm64.msi) (ARM64 tizimlar)

2. Yuklab olingan o'rnatuvchini ikki marta bosing va o'rnatish ko'rsatmalarini bajaring

> 💡 Agar muammolarga duch kelsangiz, iltimos [Microsoft rasmiy o'rnatish qo'llanmasiga](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell-on-windows) murojaat qiling

</details>

#### Windows o'rnatish xususiyatlari:

- 🔍 Agar mavjud bo'lsa, PowerShell 7 ni avtomatik aniqlaydi va ishlatadi
- 🛡️ UAC so'rovi orqali administrator huquqlarini so'raydi
- 📝 Agar PS7 topilmasa, Windows PowerShell ga o'tadi
- 💡 Agar ko'tarish muvaffaqiyatsiz bo'lsa, qo'lda ko'rsatmalar taqdim etadi

Shu bilan tugadi! Skript quyidagilarni bajaradi:

1. ✨ Vositani avtomatik ravishda o'rnatadi
2. 🔄 Cursor sinov muddatingizni darhol tiklaydi

### 📦 Qo'lda o'rnatish

> Tizimingiz uchun mos faylni [relizlar](https://github.com/yuaotian/go-cursor-help/releases/latest) sahifasidan yuklab oling

<details>
<summary>Windows paketlari</summary>

- 64-bit: `cursor-id-modifier_windows_x64.exe`
- 32-bit: `cursor-id-modifier_windows_x86.exe`
</details>

<details>
<summary>macOS paketlari</summary>

- Intel: `cursor-id-modifier_darwin_x64_intel`
- M1/M2: `cursor-id-modifier_darwin_arm64_apple_silicon`
</details>

<details>
<summary>Linux paketlari</summary>

- 64-bit: `cursor-id-modifier_linux_x64`
- 32-bit: `cursor-id-modifier_linux_x86`
- ARM64: `cursor-id-modifier_linux_arm64`
</details>

### 🔧 Texnik tafsilotlar

<details>
<summary><b>Konfiguratsiya fayllari</b></summary>

Dastur Cursor ning `storage.json` konfiguratsiya faylini quyidagi joylarda o'zgartiradi:

- Windows: `%APPDATA%\Cursor\User\globalStorage\storage.json`
- macOS: `~/Library/Application Support/Cursor/User/globalStorage/storage.json`
- Linux: `~/.config/Cursor/User/globalStorage/storage.json`
</details>

<details>
<summary><b>O'zgartirilgan maydonlar</b></summary>

Vosita quyidagilar uchun yangi noyob identifikatorlarni yaratadi:

- `telemetry.machineId`
- `telemetry.macMachineId`
- `telemetry.devDeviceId`
- `telemetry.sqmId`
</details>

<details>
<summary><b>Avtomatik yangilashni qo'lda o'chirish</b></summary>

Windows foydalanuvchilari avtomatik yangilash funksiyasini qo'lda o'chirishlari mumkin:

1. Barcha Cursor jarayonlarini yoping
2. Ushbu katalogni o'chiring: `C:\Users\username\AppData\Local\cursor-updater`
3. Xuddi shu nom bilan fayl yarating: `cursor-updater` (kengaytmasiz)

macOS/Linux foydalanuvchilari o'z tizimlarida o'xshash `cursor-updater` katalogini topishga va xuddi shunday operatsiyani bajarishga harakat qilishlari mumkin.

</details>

<details>
<summary><b>Xavfsizlik xususiyatlari</b></summary>

- ✅ Xavfsiz jarayonlarni tugatish
- ✅ Atomik fayl operatsiyalari
- ✅ Xatolarni boshqarish va tiklash
</details>

<details>
<summary><b>Reestr o'zgartirish haqida eslatma</b></summary>

> ⚠️ **Muhim: Ushbu vosita Windows Reestrini o'zgartiradi**

#### O'zgartirilgan reestr
- Yo'l: `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Cryptography`
- Kalit: `MachineGuid`

#### Potentsial ta'sir
Ushbu reestr kalitini o'zgartirish quyidagilarga ta'sir qilishi mumkin:
- Windows tizimining noyob qurilma identifikatsiyasi
- Ba'zi dasturiy ta'minotlarning qurilmani tanish va avtorizatsiya holati
- Apparat identifikatsiyasiga asoslangan tizim xususiyatlari

#### Xavfsizlik choralari
1. Avtomatik zaxiralash
   - O'zgartirishdan oldin asl qiymat avtomatik ravishda zaxiralanadi
   - Zaxira joylashuvi: `%APPDATA%\Cursor\User\globalStorage\backups`
   - Zaxira fayl formati: `MachineGuid.backup_YYYYMMDD_HHMMSS`

2. Qo'lda tiklash qadamlari
   - Registry Editor (regedit) ni oching
   - Quyidagi yo'lga o'ting: `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Cryptography`
   - `MachineGuid` ustida o'ng tugmani bosing
   - "Modify" (O'zgartirish) ni tanlang
   - Zaxira faylidan qiymatni qo'ying

#### Muhim eslatmalar
- O'zgartirishdan oldin zaxira fayli mavjudligini tekshiring
- Kerak bo'lganda asl qiymatni tiklash uchun zaxira faylidan foydalaning
- Reestrni o'zgartirish uchun administrator huquqlari talab qilinadi
</details>

---

### 📚 Tavsiya etilgan o'qish

- [Cursor muammolari to'plami va yechimlar](https://mp.weixin.qq.com/s/pnJrH7Ifx4WZvseeP1fcEA)
- [AI universal dasturlash yordamchisi qo'llanmasi](https://mp.weixin.qq.com/s/PRPz-qVkFJSgkuEKkTdzwg)

---

##  Qo'llab-quvvatlash

<div align="center">
<b>Agar bu sizga foydali bo'lsa, minnatdorchilik sifatida menga achchiq kleykovinalik gazak (Latiao) sotib olishni o'ylab ko'ring~ 💁☕️</b>
<table>
<tr>

<td align="center">
<b>微信赞赏</b><br>
<img src="img/wx_zsm2.png" width="500" alt="微信赞赏码"><br>
<small>要到饭咧？啊咧？啊咧？不给也没事~ 请随意打赏</small>
</td>
<td align="center">
<b>支付宝赞赏</b><br>
<img src="img/alipay.png" width="500" alt="支付宝赞赏码"><br>
<small>如果觉得有帮助,来包辣条犒劳一下吧~</small>
</td>
<td align="center">
<b>Alipay</b><br>
<img src="img/alipay_scan_pay.jpg" width="500" alt="Alipay"><br>
<em>1 Latiao = 1 AI fikrlash sikli</em>
</td>
<td align="center">
<b>WeChat</b><br>
<img src="img/qun-10.jpg" width="500" alt="WeChat"><br>
<em>QR kod 7 kun ichida (15-aprelgacha) amal qiladi, muddati o'tgandan so'ng WeChat qo'shing</em>
</td>
<!-- <td align="center">
<b>ETC</b><br>
<img src="img/etc.png" width="100" alt="ETC Address"><br>
ETC: 0xa2745f4CD5d32310AC01694ABDB28bA32D125a6b
</td>
<td align="center"> -->
</td>
</tr>
</table>
</div>

---

## ⭐ Loyiha statistikasi

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=yuaotian/go-cursor-help&type=Date)](https://star-history.com/#yuaotian/go-cursor-help&Date)

![Repobeats analytics image](https://repobeats.axiom.co/api/embed/ddaa9df9a94b0029ec3fad399e1c1c4e75755477.svg "Repobeats analytics image")

</div>

## 📄 Litsenziya

<details>
<summary><b>MIT Litsenziyasi</b></summary>

Copyright (c) 2024

Ushbu dasturiy ta'minot va unga tegishli hujjat fayllarining nusxasini olgan har qanday shaxsga
bepul ruxsat beriladi, jumladan cheklovsiz foydalanish,
nusxalash, o'zgartirish, birlashtirish, nashr qilish, tarqatish, sublitsenziya berish va/yoki
dasturiy ta'minotning nusxalarini sotish huquqi,
va dasturiy ta'minot taqdim etilgan shaxslarga quyidagi shartlar asosida
ruxsat berish:

Yuqoridagi mualliflik huquqi bildirishnomasi va ushbu ruxsat bildirishnomasi
dasturiy ta'minotning barcha nusxalariga yoki muhim qismlariga kiritilishi kerak.

</details>
