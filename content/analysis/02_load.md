---
Title: Load
Description: This is our loading times analysis page.
Template: report
---

# Webbplatsers laddningstid och användbarhet.

Rapportens syfte är att analysera och dokumentera laddningstiden och användbarheten bland mycket besökta webbplatser. Det skall undersökas hur laddningstiden påverkar användarupplevelsen bland webbplatserna.

Urval
-----------------------

<!-- Berätta vilka webbplatser du valt att undersöka och varför eller hur du gick tillväga när du gjorde ditt urval. -->

För analysen valdes tre hemsidor inom kategorin spelutgivare. Spelutgivare satsar på att publicera TV-spel, och därmed behövs en användarvänlig webbplats med korta laddningstider och välutvecklad responsivitet för att användaren ska kunna nå den givna informationen på ett smidigt sätt. Webbplatserna är följande:

[Xbox](https://www.xbox.com/sv-SE/)

[Playstation](https://www.playstation.com/sv-se/)

[Nintendo](https://www.nintendo.se/)

Xbox, Playstation, samt Nintendo är alla tre några av världens största spelutgivare. Därför har de en standard att uppehålla, och i denna analys skall det undersökas om spelutgivarna har snabba och användbara webbplatser.

Metod
-----------------------

<!-- Berätta kort om din "metod", hur du gör för att utföra undersökningen. Berätta om du använder något speciellt verktyg. -->

Undersökningen påbörjades med att webbplatserna besöktes, och det lades uppmärksamhet kring laddningstiderna och den övergripande känslan och responsiviteten noterades. För att notera de inledande laddningstiderna, samt för att få annan användbar information kring webbplatsernas användbarhet, användes verktyget [PageSpeed Insights](https://pagespeed.web.dev/). PageSpeed Insights är ett verktyg skapat av Google, och används för att få analysdata om den givna webbplatsen som användaren har matat in. I denna analys användes verktyget för att få ut webbplatsernas prestanda, som mäts i en skala från 0 - 100. Dessa värden noterades och dokumenterades därefter i ett Excel-ark.

Resultat
-----------------------

<!-- Dokumentera dina resultat från din studie. Berätta vad du kom fram till, vilka resultat du hittade och observerade. -->

Nedanför är informationen som har dokumenerats i denna analysen:

<div class="excel">
    <iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTtoTkUn17Y9Zq23hTeCxOCG7ICHoBcLL8mnYSGHHF_Rjz7Aio2m9cfWygXKwL1YSFj68LFM1Ml5odu/pubhtml?widget=true&amp;headers=false&scrolling=no" style="width: 100%; height: 100%; border: none; overflow: hidden;"></iframe>
</div>

Tabellen ovan visar hur lång tid de tre olika sidorna tar att ladda in data. Det går att se hur, till exempel, Xbox-webbsidan inte lyckas hålla ikapp med Nintendo- samt Playstation-sidan. Detta är eftersom Xbox-webbplatsen laddar in mycket fler resurser än de andra sidorna. Mer om detta nedan:

<img class="analysis_image" src="../assets/img/xbox.png" alt="xbox image">

Xbox-webbplatsen visar all information den behöver, med tydlig text och stora bilder. Det är dock på grund av det faktum att webbplatsen använder sig av många assets som gör att Xbox-webbplatsen hamnar sist i laddningstider mellan de tre webbplatserna. Webbplatsen prioriterar stora, mer synliga och högkvalitativa bilder, istället för div-element med text och beskrivningar. Därför behöver sidan ladda in mycket mer, vilket kan ses i sidans "resources" -column. Utöver detta så kunde en högre "total blocking time" och högre "transfer" loads observeras.

<img class="analysis_image" src="../assets/img/playstation.png" alt="playstation image">

Playstationsidan är snabbare i laddning, och visar bästa resultat i prestanda enligt [PageSpeed Insights](https://pagespeed.web.dev/). Sidan använder sig av mindre assets än Xboxsidan, med 19.9 MB i resources, jämfört med Xboxsidans 22.1 MB. Utöver detta är transfer;n lägre på Playstationsidan och total blocking time är lägre med, som i tur ger användaren möjligheten att interagera med webbplatsen snabbare. Sidans "Cumulative Layout Shift" är även lägre än de andra sidorna (på desktop). Detta innebär att sidan håller ihop och bryts inte mycket medan allt laddar in.

<img class="analysis_image" src="../assets/img/nintendo.png" alt="nintendo image">

Nintendos webbplats visar bäst resultat genomsnittligt när det kommer till laddning. Sidan laddar in snabbast på desktop och mobila enheter, och laddar in sina huvudsakliga assets snabbare. Detta är framför allt på grund av att Nintendo använder sig av få assets, och de assets som finns är oftast i lägre storlek. Det här leder till att Nintendos sida inte behöver ladda ner lika mycket, och kan fokusera på att visa upp det som finns snabbare. Sidans speed index är därmed också lägst, och detsamma med "Largest Contentful Paint".

Analys
-----------------------

<!-- Diskutera och analysera de resultaten du fann. -->

<!-- Vinnaren med bästa genomsnittliga resultat är Nintendos webbplats, följt av Playstation- och sedan Xbox webbplatserna. -->

Efter analysen var gjord, kunde slutsatsen om att assets, i form av bland annat bilder, spelar den större rollen i hur snabbt en sida kan ladda in och hur snabbt användaren får möjligheten att interagera med webbplatsen. Det gick att observera hur Xboxsidan laddade in sist, på grund av att sidan tog upp för många resources. På grund av detta tar det längre tid för användaren att börja interagera med sidan, som i sin tur bidrar till en sämre användarupplevelse. Vanliga åtgärder kring detta problem är att använda sig av lägre kvalitativa bilder. Bilder går att optimera väl utan att för mycket information går misto. Om Xbox optimerar bilderna mer, och använder fler lägre kvalitativa assets, kommer laddningstiderna och mängden data som behöver skickas minska.

En gräns för webbplatser och dess laddningstid bör ligga under 4 sekunder. Mer tid än detta kan stötta bort potentiella användare på grund av bristande intresse. Det gäller att fånga användaren med något snabbt för att skapa en välutvecklat användarupplevelse. Detta kan göras med att lägga större assets vid "above the fold", och mindre assets nedanför som är lättare för användaren att ladda in. Under analysen upplevdes det att de tre undersökta sidorna lyckades med att hamna inom denna gränsen, men att ändringar hade kunnat göras för att förbättra sidorna i framtiden.

För en bra användarupplevelse och användbarhet behövs optimering av webbplatser. Mindre kvalitativa assets, och en layout som inte behöver bero på tunga element går långt för att skapa en webbplats med låga laddningstider.


Referenser
-----------------------

<!-- Ange de eventuella referenser du använder dig av, om några. -->

Övrigt
-----------------------

<!-- Skriv ditt eget namn samt vilka gruppmedlemmar som deltog i att författa rapporten. -->

Andi Dupa
