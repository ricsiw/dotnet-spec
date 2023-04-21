# Rádiótelemetriás jelmegosztó és becslő program

## Feladat
Az alkalmazás feladata az, hogy a __rádiótelemetriás kézi vevők__* felhasználói egymással jelenidőben megosszhassák a méréseiket, illetve, hogy a mérésekből kiszámolt pozíció becsléseket kapjanak. Az eredmények az androidos segédprogram térképes nézetén jelennek meg, markerekként. A kilensalkalmazás egy már meglévő androidos program tovább fejlesztése. A felhasználók elsősorban biológiai kutatócsoportok, akik szervezetten, több vevőkészüléket használva nyomkövetnek állatokat.

<sub>**A kézi vevő és a segédprogram:* *https://drive.google.com/drive/folders/1YAxbeqqH35WtR4pAmcKD_bdEsaU-maZK?usp=share_link*</sub>

## A kisháziban elérhető funkciók
* A felhasználók azonosítása, szervezet szerint
* A kliensprogramban létrejövő becslések feltöltése, ellátva szervezeti és eszköz azonosítóval
* A szervezeten belüli egyéb felhasználók méréseinek lekérdezése (és megjelenítése)
* Pozícióbecslés a feltöltött adatok alapján (szerveroldali)
* Egyszerű konfiguráló, és térképes (Google Maps API, markerek) megjelenítő felület

## Adatbázis entitások
* irányított markerek - directionMarkers
* kézileg felvett markerek - manualMarkers
* jeladók - transmitters
* felhasználók - users

## Alkalmazott alaptechnológiák
- adatelérés: Entity Framework Core v6
- kommunikáció, szerveroldal: ASP.NET Core v6
- kliensoldal: Xamarin Android SDK 13

## Továbbfejlesztési tervek
- hosztolás linux szerveren service-ben
- szerver oldali autentikáció, hozzáférés szabályzás
- swagger dokumentáció
