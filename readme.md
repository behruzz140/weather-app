Technical Interview
Meta teglar vazifasi ?
Meta teglar brauzerlarga sahifaning mazmuni, struktura, va boshqa ma'lumotlar haqida ma'lumot berishga yordam beradi. Bu ma'lumotlar esa brauzerlarda sahifani ko'rish, qidirish, va boshqa funktsiyalarni bajarish uchun ishlatiladi. Meta teglar to'plami HTML <head> elementi ichiga joylashtiriladi.
Pesudo class va pseudo element farqi?
Pseudo-class (Pesudo-klass): Pseudo-classlar, HTML-elementlariga boshqa holatlarda (masalan, hover bo'lganda yoki active bo'lganda) ushbu elementlar uchun xususiyatlarni o'zgartirishga yordam beradi. Pseudo-classlar, : belgisi bilan ajratilgan bo'ladi. Masalan: :hover, :active, :focus.

a:hover {
    color: red;
}


button:active {
    background-color: green;
}
2. Pseudo-element (Pesudo-element): Pseudo-elementlar, HTML-elementlarining bazi qismlari uchun yangi elementlar qo'shishga imkon beradi. Ular, HTML struktura modifikatsiyasi uchun ishlatiladi. Pseudo-elementlar :: belgisi bilan ajratilgan bo'ladi. Masalan:  ::before, ::after.

p::before {
    content: "Before content";
}
Mixin vs Extend farqi ?
Mixin - kodimizda qayta ishlatmoqchi bo'lgan css deklaratsiyasi guruhlarini qayta ishlatish imkonini beradi.
Extend - Css xususiyatlari to'plamini bir selektordan boshqasiga almashish imkonini beradi
Javascript data types ?
Primative and Non-primative(Reference)
Primative:
Number
String
Boolean
Undefined
Null
BigInt
Symbol
Non-primative(Reference):
Object
Array
Variables difference ?
var - qayta o'zgaruvchi yaratsa bo'ladi, qayta qiymat tayinlash va qayta e'lon qilish mumkun.
let - qayta qiymat tayinlash mumkun, yaratilgan o'zgaruvchini qayta yaratib bo'lmaydi.
const - o'zgarmas, qiymatni o'zgartirib bo'lmaydi, qayta qiymat e'lon qilish mumkun emas.
var - global
let - local
const - local
Number methods :
isIntegar → butun sonmi yoki yo'qmi tekshiradi
Number.isInteger(0); // true
Number.isInteger(-100000); // true
Number.isInteger(99999999999999999999999); // true
Number.isInteger(0.1); // false
Number.isInteger(NaN); // false
Number.isInteger(Infinity); // false
Number.isInteger("10"); // false
     
     2. isSafeIntegar → 'xavfsiz butun son' yoki yo'qligini tekshiradi. 
Number.isSafeInteger(3); // true
Number.isSafeInteger(2 ** 53); // false
Number.isSafeInteger(2 ** 53 - 1); // true
Number.isSafeInteger(NaN); // false
Number.isSafeInteger(Infinity); // false
Number.isSafeInteger("3"); // false
Number.isSafeInteger(3.0); // true
     3. parseInt → faqat butun qismini oladi.
Number.parseInt(13.4) // 13
Number.parseInt(1.4) // 1
Number.parseInt(13.33) // 13
     4. parseFloat → shundoqligicha olib beradi.
Number.parseFloat("3"); // 3
Number.parseFloat(3.1); // 3.1
Number.parseFloat(3.0); // 3.0
      5. toFixed → butun qismini oladi, lekin type o'zgarib qoladi
Number.toFixed(13.2); // 13 type - string
Number.toFixed(1.2) // 1
Number.toFixed(13.5) // 14
      
      6. toString → Stringga o'giradi.
123.toString(); // "123" 
true.toString(); // "true"
 
        7. toPrecision → to'g'ridan-to'g'ri olinadi lekin type string bo'ladi.
let num = 13.3714;
num.toPrecision(2); // Returns "13"
num.toPrecision(3); // Returns "13.4"
num.toPrecision(10); // Returns "13.3714"
         8. toLocaleString → davlar turiga qarab sonlarni xonalarga bo'ladi.
function eArabic(x) {
  return x.toLocaleString('ar-EG');
}

console.log(eArabic(123456.789));
// Expected output: "١٢٣٬٤٥٦٫٧٨٩"

console.log(eArabic('123456.789'));
// Expected output: "123456.789"

console.log(eArabic(NaN));
// Expected output: "ليس رقم"
Math object:

floor - kichik tomonga yaxlitlash.
ceil - katta tomonga yaxlitlash.
round - haqiqiy yaxlitlash.
abs - absolute yaxlitlash sonning moduli : manfiy bo'lsa musbatga aylanadi.
random - random()* nechidur son bersak 0 dan shu songacha bo'lgan sonni chiqarib beradi.
trunc - butun qismini oladi.
pow - daraja
sqrt - kvadrat ildiz : ildiz osti
String methods: 

slice - boshini va oxirini ko'rsatib bersa o'shatdan kesib oladi. Agar hech nima bermasa copy qilib qo'yadi.
substring - negative index qabul qilmaydi. slice bilan bir xil ishlaydi.
toUppercase - katta harfga aylantiradi.
toLowercase - kichik harfga aylanatiradi.
replace - textni boshqa text bilan almashtirish.
replaceAll - textda 2ta 3ta so'z bir xil bo'lsa o'zgartirib beradi.
concat - stringni stringga qo'shib beradi.
trim - spacelarni olib tashash uchun. boshidan va oxiridan olib tashidi.
trimStart - boshidan 
trimEnd - oxiridan
chartAt - o'zgaruvchiga biriktirilgan qiymatlarni indexini bersak o'sha qiymatni qaytarib beradi.
charCodeAt - ASCII tabledagi son yoki harfni kodini olib beradi.
split - textni bo'lib beradi va qaytgan qiymat array bo'ladi.
Undefined vs null  ?
Undefined - o'zgaruvchu ochib unga qiymat berilmasa, undefined hisoblanadi.
Null - o'zgaruvchi bor, nomi ham bor lekin ichi bo'shligini etsak, uni null deb yozamiz.
Truthy , Falthy  ?

