# Webprogramozás -- PHP csoportzh

## Tudnivalók

1. A feladat beküldésével **az alább leírtakat megértettnek és elfogadottnak tekintjük** annak a nevében, aki a megoldást beküldte.

    ```txt
    Kijelentem, hogy ez a megoldás a saját munkám. Nem másoltam vagy 
    használtam harmadik féltől származó megoldásokat. Nem továbbítottam 
    megoldást hallgatótársaimnak, és nem is tettem közzé. Az Eötvös Loránd 
    Tudományegyetem Hallgatói Követelményrendszere (ELTE szervezeti és 
    működési szabályzata, II. Kötet, 74/C. §) kimondja, hogy mindaddig, 
    amíg egy hallgató egy másik hallgató munkáját - vagy legalábbis annak 
    jelentős részét - saját munkájaként mutatja be, az fegyelmi vétségnek számít. 
    A fegyelmi vétség legsúlyosabb következménye a hallgató elbocsátása az egyetemről.
    ```

2. A terminálban a `php -S localhost:1234` paranccsal tudtok szervert indítani.  

3. Töltsd le a `starter.zip` kezdőcsomagot. A mappákon belül a feladatokat az`index.php` állományban oldd meg!

4. A feladatok végeztével tömörítsd be a megoldásokat tartalmazó mappát (zip), és töltsd fel a Canvasre!

5. A feladatok megoldására **45 perc** áll rendelkezésre **+ 10 perc** az egyéb adminisztrációra (feladatok elolvasása, struktúra kialakítása, feltöltés).

6. A zh-hoz bármilyen írott segédanyag használható, azaz az órai munkák és a gyakorlati videók anyaga is. Zh közbeni humán segítség használata tilos!

## Feladatok

1. **Roxforti diákok névsora (4 pont)** A Roxfort egyes diákjainak névsora adott egy PHP adatszerkezetben.
    - a\. (1,5 pont) Jelenítsd meg a diákok nevét és a patrónusát egy táblázatban!
    - b\. (1 pont) A táblázat sorai legyenek olyan háttérszínűek, mint ami a háznak megfelelő szín a `colors`-ban!
    - b\. (1 pont) Keressd meg, melyik ház diákjaiból vannak a legtöbben, írd ki a ház nevét, és az oldal háttérszínét állítsd át az aszerinti értékre. (a `colors`-ban vannak az egyes színek) 
    - c\. (0,5 pont) A Táblázat alá írd ki a legtöbb karakterből álló patrónust!

2. **Felvétel a Roxfortba (6 pont)** Készíts egy regisztációs felületet, ahol meg tudsz adni egy nevet, egy emailcímet és ki tudod választani egy roxforti házat.
    - a\. (1 pont) Validáld a nevet: `legyen kitöltve és álljon minimum két részből amit vessző választ el - elég csak ezt validálni, kis és nagybetűkre nem kell figyelni`  *Tipp: Távolítsd el a felesleges szóközöket, majd `,` alapján vágd szét a stringet és nézd meg, hogy az elemeinek hosszúsága nagyobb-e mint 0*
        - példa helyes formátumra: `Random,Név` `random,név`
        - példa helytelen formátumra: `Random Név` , `      ,    ` , `random név,  `, 
    - b\. (0,5 pont) Validáld az email címet: `legyen kitöltve és legyen valid emailcím` *Tipp: használd a FILTER_VALIDATE_EMAIL-t*
    - c\. (1 pont) Validáld a házat: `ki van-e választva valami és az helyes-e`
    - d\. (0,5 pont) A form legyen állapottartó!
    - e\. (0,5 pont) Elküldésnél, ha valami nincs helyesen kitöltve, jelenjenek meg a hibaüzenetek bárhol az oldalon  
    - f\. (0,5 pont) Elküldésnél, ha valami nincs helyesen kitöltve, jelenjenek meg a hibaüzenetek az egyes input mezők mellett
    - g\. (2 pont) Elküldésnél, ha minden helyesen van kitöltve, egészítsd ki a `data.json` fájlt az új adat mentésével:
        - (0,5 pont) Mentsd ki egy változóba a tartalmát!
        - (0,5 pont) Add hozzá az új adatot az eddigi adatokhoz!
        - (0,5 pont) Mentsd el helyesen, olvasható formátumban! *Tipp: Használd a JSON_PRETTY_PRINT-et*
        - (0,5 pont) Írd ki, hogy "Sikeres jelentkezés!" az oldalra!

