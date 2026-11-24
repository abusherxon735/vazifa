# Terminal Guide — Terminal komandalar

## 1. Terminal nima?
**Ta’rif:** Terminal — kompyuter bilan matnli buyruqlar orqali muloqot qilish imkonini beradigan dastur yoki interfeys.
**Vazifasi:** Buyruqlar orqali kompyuterni boshqarish.
**Qachon ishlatiladi:** Fayl boshqarish, dastur ishga tushirish va Git buyruqlarini bajarishda.
```bash
pwd
```

## 2. Terminal nima uchun kerak?
**Ta’rif:** Terminal buyruqlar yozib tizim bilan ishlash imkonini beradi.
**Vazifasi:** Fayl va papkalarni boshqarish, dasturlarni ishga tushirish va Git buyruqlarini bajarish.
**Qachon ishlatiladi:** Grafik oynadan ko‘ra buyruq bilan tezroq ishlash kerak bo‘lganda.
```bash
mkdir my-project
```

## 3. `pwd` — joriy joylashuvni ko‘rish
**Vazifasi:** Terminal qaysi papkada turganini to‘liq manzili bilan ko‘rsatadi.
**Qachon ishlatiladi:** Buyruqni qaysi papkada bajarayotganingizni tekshirishda.
```bash
pwd
```

## 4. `ls` — fayllarni ko‘rish
**Vazifasi:** Joriy papkadagi fayl va papkalar ro‘yxatini ko‘rsatadi.
**Qachon ishlatiladi:** Papka ichidagi narsalarni tekshirishda. Windows PowerShell’da `ls` alias sifatida ishlaydi.
```bash
ls
```

## 5. `cd` — papkaga kirish
**Vazifasi:** Ko‘rsatilgan papkaga o‘tadi.
**Qachon ishlatiladi:** Boshqa papkadagi fayllar bilan ishlashda.
```bash
cd documents
```

## 6. `cd ..` — yuqori papkaga chiqish
**Vazifasi:** Joriy papkaning bitta yuqori darajasiga qaytadi.
**Qachon ishlatiladi:** Ota papkaga qaytish kerak bo‘lganda.
```bash
cd ..
```

## 7. `mkdir` — papka yaratish
**Vazifasi:** Yangi papka yaratadi.
**Qachon ishlatiladi:** Loyihani bo‘limlarga ajratishda.
```bash
mkdir my-folder
```

## 8. `touch` — fayl yaratish
**Vazifasi:** Git Bash, macOS va Linux’da yangi bo‘sh fayl yaratadi.
**Qachon ishlatiladi:** Yangi matn yoki kod fayli kerak bo‘lganda.
```bash
touch notes.txt
```
PowerShell’da:
```powershell
New-Item notes.txt -ItemType File
```

## 9. `cat` — fayl mazmunini ko‘rish
**Vazifasi:** Matnli fayl ichidagi yozuvlarni terminalda chiqaradi.
**Qachon ishlatiladi:** Faylni ochmasdan matnini ko‘rishda.
```bash
cat notes.txt
```

## 10. `clear` — terminalni tozalash
**Vazifasi:** Terminal oynasidagi avvalgi matnlarni ekrandan tozalaydi; fayllarni o‘chirmaydi.
**Qachon ishlatiladi:** Terminal oynasini tartibga keltirishda.
```bash
clear
```

## 11. `cp` — nusxa olish
**Vazifasi:** Fayl yoki papkadan nusxa yaratadi.
**Qachon ishlatiladi:** Asl faylni saqlagan holda nusxa kerak bo‘lganda.
```bash
cp notes.txt notes-copy.txt
```

## 12. `mv` — ko‘chirish yoki nomini o‘zgartirish
**Vazifasi:** Fayl yoki papkani boshqa joyga ko‘chiradi yoki nomini o‘zgartiradi.
**Qachon ishlatiladi:** Faylni tartiblash yoki qayta nomlashda.
```bash
mv old.txt new.txt
```

## 13. `rm` — fayl o‘chirish
**Vazifasi:** Ko‘rsatilgan faylni o‘chiradi.
**Qachon ishlatiladi:** Keraksiz sinov faylini olib tashlashda. Faqat o‘zingiz yaratgan fayllarda ehtiyotkorlik bilan ishlating.
```bash
rm notes-copy.txt
```
**Xavfsizlik:** `rm -rf` kabi qaytarish qiyin bo‘lgan buyruqlarni ushbu topshiriqda ishlatmang.

## 14. `git init` — repository yaratish
**Vazifasi:** Joriy papkada yangi Git repository boshlaydi.
**Qachon ishlatiladi:** Yangi loyihani Git bilan kuzatishni boshlaganda.
```bash
mkdir my-project
cd my-project
git init
```

## 15. `git status` — Git holatini tekshirish
**Vazifasi:** Git repository’dagi yangi, o‘zgargan va stagingga qo‘shilgan fayllar holatini ko‘rsatadi.
**Qachon ishlatiladi:** Fayllarni commit qilishdan oldin holatni tekshirishda.
```bash
git status
```
