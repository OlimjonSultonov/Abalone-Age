
# Qisqichbaqaning Yoshini Bashorat Qilish uchun Model

## Loyihaning tavsifi
Ushbu Jupyter Notebook qisqichbaqa yoshini bashorat qilish uchun regressiya modelini yaratishga qaratilgan. Loyihada **pandas**, **sklearn**, **seaborn**, va boshqa mashinani o'rganish uchun kerakli kutubxonalar ishlatiladi.

## Asosiy bosqichlar:
1. **Kutubxonalarni yuklash:** 
   - Pandas, numpy, seaborn, matplotlib va sklearn kabi kutubxonalar import qilinadi.
2. **Ma'lumotlarni yuklash:** 
   - `train.csv` fayli yordamida qisqichbaqalar haqidagi ma'lumotlar pandas DataFrame formatida yuklanadi va ustunlar ko'rib chiqiladi.
3. **Ma'lumotlarni kodlash:** 
   - Qisqichbaqa jinsiy ma'lumotlari `OneHotEncoder` yordamida kodlanadi.
4. **Pipeline yaratish:** 
   - Ma'lumotlarni oldindan qayta ishlash va regressiya modelini birlashtirish uchun **Pipeline** dan foydalaniladi.
5. **Stacking Regressor ishlatish:** 
   - Bir nechta regressiya modellarning natijalarini birlashtirish orqali umumiy bashoratni yaxshilovchi **Stacking Regressor** ishlatiladi.

## Model haqida:
Ushbu model qisqichbaqaning yoshi bilan bog'liq bo'lgan xususiyatlar asosida uning yoshini bashorat qilish uchun regressiya usulidan foydalanadi. Loyihada **Stacking Regressor** algoritmi qo'llaniladi, u bir nechta modellarning natijalarini birlashtiradi va umumiy bashoratni yaxshilaydi.

## Pipeline haqida:
**Pipeline** jarayoni modellarning ishlash tartibini avtomatlashtiradi. Bu ma'lumotlarni oldindan qayta ishlashdan tortib, modelni o'qitish va bashorat qilishgacha bo'lgan barcha bosqichlarni ketma-ket bajaradi. Masalan, avval ma'lumotlar miqyoslanadi, so'ngra modelga uzatiladi. Bu jarayon bir joyda boshqariladi va toza kod yozishga imkon beradi.

## Stacking Regressor haqida:
**Stacking Regressor** bir nechta modellarning kombinatsiyasidan foydalanadi. Har bir model ma'lumotlar ustida ishlaydi va yakuniy bashoratlarni hisoblashda ularning natijalari birlashtiriladi. Bu usul, odatda, alohida modellardan ko'ra yuqori aniqlikka ega bo'ladi, chunki turli modellarning kuchli tomonlari birlashtiriladi.

## Eng yaxshi parametrlarni topish:
Loyihada **RandomizedSearchCV** yordamida regressiya modellari uchun eng yaxshi parametrlarni topish amalga oshirildi. Bu usul turli xil parametrlarning kombinatsiyalarini sinab ko'radi va ma'lum maqsad ko'rsatkichlariga ko'ra eng yaxshi ishlashga ega parametrlarni aniqlaydi. Bu jarayon yordamida model yanada optimallashtirildi va aniqroq bashoratlar qilinishi ta'minlandi.

Parametrlarni tuning qilishda quyidagi modellar sinovdan o'tkazildi:
- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **ElasticNet Regression**
- **Huber Regressor**

Eng yaxshi parametrlarni topish orqali modellarning natijadorligi sezilarli darajada oshirildi va bashoratlarda aniqlik yuqori darajada saqlanib qolindi.

## Talablar:
- Python 3.x
- Quyidagi Python kutubxonalari:
  - pandas
  - numpy
  - seaborn
  - matplotlib
  - scikit-learn

## Foydalanish:
1. Loyihani klonlash yoki yuklab olish:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Kutubxonalarni o'rnatish:
   ```bash
   pip install -r requirements.txt
   ```
3. Jupyter Notebook ishga tushirish:
   ```bash
   jupyter notebook demo.ipynb
   ```

## Mualliflik huquqi:
Loyiha ochiq manba va uni erkin foydalanish mumkin.
