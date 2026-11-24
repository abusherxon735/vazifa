# Git Guide — Git asoslari va Git komandalar

## 1. Git nima?
**Ta’rif:** Git — fayllardagi o‘zgarishlarni kuzatish va loyiha versiyalarini boshqarish uchun ishlatiladigan taqsimlangan versiya nazorati tizimi. U loyiha tarixini saqlaydi.

**Vazifasi:** Fayllar tarixini saqlash va o‘zgarishlarni nazorat qilish.
**Qachon ishlatiladi:** Yangi loyiha boshlaganda yoki mavjud loyihadagi o‘zgarishlarni kuzatishda.
```bash
git init
```

## 2. Git nima uchun kerak?
**Ta’rif:** Git loyiha ustida bajarilgan ishlarning tarixini saqlaydi.
**Vazifasi:** Oldingi holatlarni ko‘rish, xatolarni aniqlash, branchlarda alohida ishlash va hamkorlik qilish.
**Qachon ishlatiladi:** Loyiha davomida har bir muhim o‘zgarishni qayd etishda.
```bash
git log --oneline
```

## 3. Repository nima?
**Ta’rif:** Repository — loyiha fayllari va ularning Git tarixini saqlaydigan joy.
**Vazifasi:** Fayllar hamda commitlar tarixini bir joyda saqlash.
**Qachon ishlatiladi:** Loyihani Git bilan boshqarishni boshlaganda.
```bash
git init my-project
```

## 4. Global va Local konfiguratsiya farqi
**Ta’rif:** Global sozlama foydalanuvchining barcha loyihalariga, local sozlama esa faqat joriy repository’ga tegishli.
**Vazifasi:** Commit muallifining ismi va emailini belgilash.
**Qachon ishlatiladi:** Git’dan birinchi marta foydalanishda yoki muallif ma’lumotlarini o‘zgartirganda.
```bash
git config --global user.name "Ism Familiya"
git config --global user.email "email@example.com"
git config user.name "Ism Familiya"
git config --list
```
Local qiymat mavjud bo‘lsa, shu repository’da global qiymatdan ustun turadi.

## 5. `git init`
**Ta’rif:** Joriy papkada yangi Git repository boshlaydi.
**Vazifasi:** Papkani Git kuzatadigan loyihaga aylantirish.
**Qachon ishlatiladi:** Yangi loyihani Git bilan boshqarishni boshlaganda.
```bash
git init
```

## 6. `git status`
**Ta’rif:** Repository holatini ko‘rsatadi.
**Vazifasi:** Yangi, o‘zgargan, stagingga qo‘shilgan va commit qilinmagan fayllarni ko‘rsatish.
**Qachon ishlatiladi:** Fayllarni qo‘shish yoki commit qilishdan oldin.
```bash
git status
```

## 7. `git add`
**Ta’rif:** Tanlangan fayllardagi o‘zgarishlarni staging area’ga qo‘shadi.
**Vazifasi:** Keyingi commitga qaysi o‘zgarishlar kirishini tanlash.
**Qachon ishlatiladi:** Faylni tahrirlagandan keyin.
```bash
git add README.md
git add .
```

## 8. `git commit`
**Ta’rif:** Staging area’dagi o‘zgarishlarni repository tarixida yangi commit sifatida saqlaydi.
**Vazifasi:** O‘zgarishlarni izoh bilan tarixga yozish.
**Qachon ishlatiladi:** Biror ish yoki vazifa yakunlanganda.
```bash
git add .
git commit -m "Add project files"
```

## 9. `git log`
**Ta’rif:** Repository’dagi commitlar tarixini ko‘rsatadi.
**Vazifasi:** Commit muallifi, sanasi va xabarlarini ko‘rish.
**Qachon ishlatiladi:** Loyiha tarixini tekshirishda.
```bash
git log
git log --oneline
```

## 10. `git branch`
**Ta’rif:** Branchlarni ko‘rish, yaratish va boshqarish buyrug‘i.
**Vazifasi:** Asosiy ish yo‘nalishidan alohida vazifa uchun branch ochish.
**Qachon ishlatiladi:** Yangi funksiya yoki mavzu ustida alohida ishlaganda.
```bash
git branch
git branch new-feature
```

## 11. `git switch`
**Ta’rif:** Mavjud branchga o‘tadi; `-c` bilan yangi branch yaratib, unga o‘tadi.
**Vazifasi:** Turli ish yo‘nalishlari orasida almashish.
**Qachon ishlatiladi:** Boshqa branchdagi vazifani bajarishda.
```bash
git switch main
git switch -c new-feature
```

## 12. `git merge`
**Ta’rif:** Boshqa branchdagi o‘zgarishlarni joriy branchga birlashtiradi.
**Vazifasi:** Alohida bajarilgan ishlarni bitta branchga jamlash.
**Qachon ishlatiladi:** Ish tugab, uni asosiy branchga qo‘shishga ruxsat berilganda.
```bash
git switch main
git merge new-feature
```
Ushbu amaliy topshiriqda o‘quvchi merge bajarmaydi; merge keyingi darsda o‘qituvchi tomonidan ko‘rsatiladi.

## 13. `git branch -d`
**Ta’rif:** Lokal branchni xavfsiz o‘chiradi.
**Vazifasi:** Ish tugagan va birlashtirilgan branchni tozalash.
**Qachon ishlatiladi:** Branchdagi ish kerakli joyga birlashtirilgandan keyin.
```bash
git switch main
git branch -d new-feature
```
Merge qilinmagan ish bo‘lsa, Git ogohlantirishi mumkin. Ushbu topshiriqda branchlar o‘chirilmaydi.

## Savol-javoblar
1. **Git nima?** — Versiyalarni boshqarish tizimi.
2. **Repository nima?** — Loyiha fayllari va Git tarixini saqlaydigan joy.
3. **`git add` nima qiladi?** — O‘zgarishlarni staging area’ga qo‘shadi.
4. **`git commit` nima qiladi?** — Stagingdagi o‘zgarishlarni tarixga saqlaydi.
5. **Branch nima uchun kerak?** — Alohida vazifani asosiy ishga ta’sir qilmasdan bajarish uchun.
6. **`git status` nimani ko‘rsatadi?** — Repository holatini.
