### Bugun biz lifecycle haqida gaplashamiz.Lifecycle bu inglizcha so’z bo’lib “life” – bu hayot va “cycle” – bu sikl,jarayon,davr deb tarjima qilinadi o’zbek tiliga.Shundan kelib chiqqan holda biz buni hayot sikli deb tarjima qilsak bo’ladi.Lifecyclega hayotda misollar juda ko’p,misol uchun insonning yashash davri(tug’ilishdan  vafotigacha ),kapalakning hayot davri  misol bo’la oladi.React da esa bu componenttalarning hayot sikli desak bo’ladi.Ya’ni componentlar ma’lum davrida , biron bir hodisani bajarib olish imkonini beradi.Masalan, render bo’lishidan oldin ma’lumotni tekshirib olishimiz yoki undagi jarayon davomida bo’lgan o’zgarishlarni tekshirish va bir-biri bilan solishtirish imkonini beradi.
Har bir componenttaning o’zining lifecycle bo’ladi va bu asosan uchta davrga bo’linadi : 1- Mounting,2-Updating,3-Unmounting.
Mounting – bu dastlabki davr bo’lib,bu component yaratilish davridir.Mounting da 1- constructor , keyin render ishlidi , ammo  ma’lumot return bo’lmay turadi, undan keyin esa lifecycle Mounting  maxsus metodi ya’ni hozirda keng qo’llaniladigan componentDidMount() ishlidi.Bu metod bizga render bo’lgandan keyin,ma’lum  bir ishni bajarish imkoni beradi.

Updating – bu o’zgarish davridir.Ushbu lifecycleda  esa avval render, keyin componentDidUpdate() metod ishlidi.Bu komponentada biz masalan,stateda bo’lgan o’zgarishlarni solishtirishimiz mumkin.Misol keltiradigan bo’lsak,agar bizda state Boolean qiymat bo’lib u tez-tez o’zgaradigan bo’lsa va u o’zgarishlar ketma – ket bir xil natijani ko’rsatishi mumkin bo’lsa, unda biz ko’p marta render bo’lish ehtimolini quyidagi kod orqali kamaytirishimiz mumkin : 

<img src="https://magenta-bublanina-52c5d3.netlify.app/images/code2.png" width="600px" >
Buning foydasi shundayki,bizga ma’lum ko’p marta render bo’lsa , u saytimizni qotishga olib keladi.Buni oldini olish uchun biz yuqoridagi koddan foydalanishimiz mumkin.

Unmounting – bu component reactdan o’chirilganda davridir ya’ni bu o’limga xoslash mumkin.ushbu lifecycleda biz componentWillUnMount() dan foydalanishimiz mumkin.Ushbu metod bizga o’chirilgan komponentdan qayta foydalanish imkonini beradi.Misol uchun bizda button bosganda componentta o’chirilsin va alert da component o’chirilgani haqida ma’lumot chiqsin.Buning uchun quyidagicha koddan foydalanamiz.
<img src="https://magenta-bublanina-52c5d3.netlify.app/images/code4.png" width="600px">
<img src="https://magenta-bublanina-52c5d3.netlify.app/images/code2.png" width="600px">
Buning natijasi shundayki agar button bosilsa,alert da bizga component unmount bo’lgani haqida ma’lumot chiqadi.
Men bu maqolamdan sizga lifecycle haqida kerakli ma’lumot bera olgan bo’lsam va ilmiz oshishiga sababchi bo’lgan bo’lsam xursandman.Men o’z niyatimga erishibman.Hudo hohlasa maqolalarimiz davom etadi! 
