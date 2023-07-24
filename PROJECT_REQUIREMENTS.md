# PROJECT_REQUIREMENTS

Assalomu alaykum! 
Java Spring dasturchisi uchun test loyihasini taqdim etish uchun, keling, Spring Boot yordamida oddiy veb-ilovani yarataylik. 
Bizning ilovamiz oddiy BLOGGING taqdim etadi.

### Texnologiyalar:
* Java 8+
* Spring Boot
* Spring Data JPA
* Thymeleaf (HTMLda ma'lumotlarni ko'rsatish uchun)
* PostgreSQL (yoki boshqa mos DBMS)
* Maven (bog'liqlarni boshqarish va loyihani yaratish uchun)

### Loyiha vazifalari:

**Maydonlar bilan blogni (Blog) ifodalash uchun ob'ekt yarating:**
* id (unikal identifikator)
* sarlavha (blog nomi)
* mavzu (mavzu nomi, olhida jadvalga olib chiqish mu’mkin)
* matn (blog mazmuni HTML formatta)
* yaratilgan sana (blog jadvalga yozilgan sana) 
* oqilishlar soni (blog ochib oqilishlar soni) 
* tekshirilgan (moderator tomonidan tekshirilganligi true/false)

**Maydonlar bilan blog uchun izohni (Comment) ifodalash uchun ob'ekt yarating:**
* id (unikal identifikator)
* blog_id(blog bilan bog’lanish kaliti)
* izoh (izoh matn korinishida uzunligi 400 dan oshmasligi shart)
* yaratilgan sana (izoh jadvalga yozilgan sana)
* foydaliligi (izoh foydaliligi soni)
* foydasizligi (izoh foydasizligi soni)
* tekshirilgan (moderator tomonidan tekshirilganligi true/false)

**Spring Data JPA yordamida ma'lumotlar bazasi aloqasini o'rnating.**

**HTTP so'rovlarini boshqarish uchun controllerlarni ishlab chiqing:**
* Barcha bloglar ro'yxatini ko'rsatish (jumladan, tekshirilgan va tekshirilmagan).
* Yangi blog qo'shish.
* Blogni toliq ko’rish 
* Blogni tekshirilgan deb belgilash. 
* Blogni o'chirish. 
* Blog uchun izohlar ro’yxatini ko’rsatish. 
* Blog uchun izoh kiritish . 
* Tasdiqlanmagan izohlar ro’yxatini ko’rsatish. 
* Izohni tasdiqlangan deb belgilash. 
* Izohni o’chirish.


**Malumotlarni akt ettirish haqida**
* Thymeleaf yordamida bloglar roʻyxatini ko’rsating
* Blog toliq ko’rinishini, tasdiqlanmagan izohlar ro’yxatini ko’rsating 
* Yangi blog qoʻshish uchun form (HTML sahifalari) yarating.

**Testlash haqida** 
* Controller va Service uchun testlarni yozing
* Barcha holatlarni qamrab olish shart emas, lekin hech bo'lmaganda asosiy funksional metodlar uchun test yozing.

**Buni bajarish majburiy emas:** 
* bloglar va tasdiqlanmagan izohlar roʻyxatlarida sahifada pagination amalga oshiring.

### Ishchi loyihani yaratish bo'yicha ko'rsatmalar:

* Spring Initializer (https://start.spring.io/) yordamida yangi Spring Boot loyihasini yarating. Pom.xml fayliga kerakli bog'liqliklarni (Spring Web, Spring Data JPA, Thymeleaf va boshqalar) qo'shing. 
* Kerakli maydonlar va JPA izohlari bilan Blog, Comment, (Mavzu) ob'ektini yarating. 
* application.properties yoki application.yml faylida ma'lumotlar bazasi ulanishini o'rnating. 
* HTTP so'rovlarini qayta ishlash uchun controller va blog, comment (mavzu)  bilan ishlash uchun serviceni amalga oshiring. 
* Bloglar ro'yxatini ko'rsatish va yangi blog shaklini qo'shish uchun Thymeleaf shablonlarini yarating. 
* Blogni oqish imkoniyatini beruvchi oyna (dialog ko’rinishida) yarating. Blog oqirida izohlar ro’yxati ko’rsatilgan (max 5 ta, agar undan ko’p bolsa ko’pligi haqida ma’lumot bolishi kerak) va izoh qoldirish uchun joy bolishi kerak. 
* Moderator uchun izohlarni tasdiqlash mumkin bolgan oynani Thymeleaf shablonlarini yarating. 
* Controller va Service uchun testlarni yozing. 
* Ilovani ishga tushiring va uning to'g'ri ishlashiga ishonch hosil qiling. 
* Ilova kodlarini https://gitlab.com/asamatdin92/test-for-candidats projectga o’zingizning ismfamilya (damirasamatdinov) ko’rinishidagi branchga yuklang.

### Qoshimcha ma'lumotlar
Bu test loyihasining asosiy versiyasi bo'lib, unda foydalanuvchi autentifikatsiyasi, blogni tahrirlash va hokazolar kabi qo'shimcha funktsiyalar bilan kengaytirishingiz mumkin. 
Tekshirishni osonlashtirish uchun kodingizni sharhlashni unutmang.

### Savol va murojaatlar haqida
Agar sizda biron bir savol bo'lsa, bemalol bizaga murojaat qilishingiz mumkin.

`
Test loyihangizga omad tilaymiz!
`