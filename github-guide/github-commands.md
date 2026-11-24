# GitHub Guide — GitHub va Remote komandalar

## 1. GitHub nima?
**Ta’rif:** GitHub — Git repository’larini internetda saqlash, ulashish, ko‘rib chiqish va loyihalar ustida hamkorlik qilish platformasi.
**Vazifasi:** Loyihani onlayn saqlash va boshqalar bilan hamkorlik qilish.
**Qachon ishlatiladi:** Loyihani internetga joylash yoki jamoa bilan ishlashda.
```text
https://github.com/
```

## 2. Git va GitHub farqi
**Ta’rif:** Git — versiya nazorati tizimi; GitHub — Git repository’larini onlayn saqlash va boshqarish xizmati.
**Vazifasi:** Git o‘zgarishlarni kompyuterda kuzatadi, GitHub esa repository’ni masofadan saqlash va ulashishga yordam beradi.
**Qachon ishlatiladi:** Lokal ishni internetga yuborish kerak bo‘lganda.
```bash
git push
```

## 3. GitHub account nima?
**Ta’rif:** GitHub account — foydalanuvchining GitHub’dagi shaxsiy hisobidir.
**Vazifasi:** Repository yaratish, loyihalarni saqlash va platformadan foydalanish.
**Qachon ishlatiladi:** GitHub’da loyiha ochish va boshqarishda.
```text
https://github.com/signup
```

## 4. Repository nima?
**Ta’rif:** GitHub repository — loyiha fayllari, commitlar, branchlar va loyiha ma’lumotlari saqlanadigan masofaviy ombor.
**Vazifasi:** Loyihani onlayn saqlash.
**Qachon ishlatiladi:** GitHub’da yangi loyiha boshlaganda.
```bash
git clone https://github.com/USERNAME/REPOSITORY.git
```

## 5. Public va Private repository farqi
**Ta’rif:** Public repository hammaga ko‘rinadi; Private repository faqat egasi va ruxsat berilgan foydalanuvchilarga ko‘rinadi.
**Vazifasi:** Loyiha ko‘rinish huquqini boshqarish.
**Qachon ishlatiladi:** Repository yaratishda maxfiylik turini tanlashda.
```text
Repository yaratish oynasida Public yoki Private tanlanadi.
```

## 6. Remote nima?
**Ta’rif:** Remote — lokal Git repository bilan bog‘langan masofaviy repository manzili.
**Vazifasi:** Lokal va GitHub’dagi repository orasida ma’lumot almashish.
**Qachon ishlatiladi:** Lokal loyihani GitHub’ga ulashda.
```bash
git remote -v
```

## 7. `git remote add`
**Ta’rif:** Lokal repository’ga remote manzil qo‘shadi.
**Vazifasi:** GitHub repository’ni `origin` nomi bilan ulash.
**Qachon ishlatiladi:** Lokal loyiha GitHub’ga birinchi marta ulanayotganda.
```bash
git remote add origin https://github.com/USERNAME/REPOSITORY.git
```

## 8. `git remote -v`
**Ta’rif:** Ulangan remote repository’larning manzillarini ko‘rsatadi.
**Vazifasi:** Fetch va push manzillarini tekshirish.
**Qachon ishlatiladi:** Remote to‘g‘ri ulanganini tekshirishda.
```bash
git remote -v
```

## 9. `git push`
**Ta’rif:** Lokal commitlarni remote repository’ga yuboradi.
**Vazifasi:** Kompyuterdagi o‘zgarishlarni GitHub’da saqlash.
**Qachon ishlatiladi:** Commit tayyor bo‘lgandan keyin.
```bash
git push -u origin main
```

## 10. `git pull`
**Ta’rif:** Remote repository’dagi yangilanishlarni olib keladi va joriy branchga birlashtiradi.
**Vazifasi:** Lokal nusxani GitHub’dagi yangilanishlar bilan moslashtirish.
**Qachon ishlatiladi:** Ishni boshlashdan oldin yoki boshqa joydan yuborilgan yangilanishlarni olishda.
```bash
git pull origin main
```

## 11. `git clone`
**Ta’rif:** Masofaviy repository nusxasini kompyuterga yuklab, lokal Git repository yaratadi.
**Vazifasi:** Mavjud GitHub loyihasini kompyuterda ishlatish.
**Qachon ishlatiladi:** Boshqa kompyuterda loyiha bilan ishlashni boshlaganda.
```bash
git clone https://github.com/USERNAME/REPOSITORY.git
```

## 12. GitHub’da branch nima?
**Ta’rif:** Branch — repository ichidagi alohida ish yo‘nalishi.
**Vazifasi:** `main` branchni darhol o‘zgartirmasdan vazifa bajarish.
**Qachon ishlatiladi:** Alohida funksiya yoki mavzu ustida ishlaganda.
```bash
git switch -c new-feature
```

## 13. GitHub’da commit nima?
**Ta’rif:** Commit — repository tarixidagi saqlangan o‘zgarishlar to‘plami.
**Vazifasi:** O‘zgarishlar va ularning izohini tarixda saqlash.
**Qachon ishlatiladi:** O‘zgarishlar tayyor bo‘lganda.
```bash
git commit -m "Update documentation"
```

## 14. GitHub’da faylni tahrirlash
**Ta’rif:** GitHub saytidagi faylni Edit tugmasi orqali o‘zgartirish mumkin.
**Vazifasi:** Brauzer orqali fayl mazmunini yangilash.
**Qachon ishlatiladi:** Kichik o‘zgarishni kompyuterga repository yuklamasdan kiritishda.
**Amal:** Repository ichida faylni oching → Edit (qalam) tugmasini bosing → matnni o‘zgartiring → Commit changes ni bosing. To‘g‘ri branchni tanlang.

## 15. GitHub’da branchni o‘chirish
**Ta’rif:** Branch repository’dagi alohida ish yo‘nalishini olib tashlashdir.
**Vazifasi:** Ish tugagan branchlarni tozalash.
**Qachon ishlatiladi:** Odatda ish merge qilingandan keyin.
```bash
git push origin --delete branch-name
```
Ushbu amaliy topshiriqda branchlar o‘chirilmaydi.

## GitHub’da yangi repository yaratish — 5 bosqich
1. [github.com](https://github.com/) saytiga kiring va hisobingizga kiring.
2. Yuqoridagi `+` belgisini bosib, **New repository** ni tanlang.
3. Repository nomiga `git-github-master-guide` deb yozing.
4. Public yoki Private turini tanlang. Lokal README mavjud bo‘lsa, README, `.gitignore` va license avtomatik yaratish kataklarini belgilangmang.
5. **Create repository** tugmasini bosing va ko‘rsatilgan HTTPS manzilini nusxalang.

## Savol-javoblar
1. **GitHub nima?** — Git repository’larini onlayn saqlash va hamkorlik platformasi.
2. **Git va GitHub farqi nima?** — Git versiyalarni boshqaradi, GitHub esa repository’larni internetda saqlaydi.
3. **Public repository kimga ko‘rinadi?** — Internetdagi hammaga.
4. **`git push` nima qiladi?** — Lokal commitlarni remote’ga yuboradi.
5. **`git pull` nima qiladi?** — Remote yangilanishlarini olib keladi va joriy branchga qo‘shadi.
6. **`git clone` nima qiladi?** — Masofaviy repository nusxasini kompyuterga oladi.
