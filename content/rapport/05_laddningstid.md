---
---
Laddningstid
=======================

Denna rapport handlar om att undersöka, jämföra och analysera webbplatser utifrån laddningstid och vad som kan tänkas förbättra den.

Urval
-----------------------

Jag har valt att utgå ifrån ett bekvämlighetsurval, detta i sin tur innebär att urvalet har gjorts efter webbsidor jag på förhand haft vetskapen om samt vilka på ett målinriktat sätt kan belysa kontraster webbsidorna emellan(Bryman 2011). Rent praktiskt innebär detta att jag försökt jämföra sidor som är mer eller mindre lika varandra för att eventuella skillnader i laddningstid, resurser, storlek och PSI score skall vara av intresse att jämföra. Det känns orimligt att välja en sida med video/mycket bilder och sedan jämföra den mot en sida med få eller inga bilder. Därför har jag i största möjliga mån valt att jämföra sidor som är så lika som möjligt i form utav upplägg.

Jag valde att jämföra de tre största webbplatserna för streaming av spel just nu: [youtube.com/gaming](http://www.youtube.com/gaming), [twitch.tv](http://www.twitch.tv/) och [mixer.com](http://mixer.com/).

Metod
-----------------------

De verktyg som använts är [Google PageSpeed Insights](http://developers.google.com/speed/pagespeed/insights) samt network-tabben i Mozilla firefox devtools.

Värt att notera är att webbsidorna har besökts 2019-12-10 och det faktum att webbsidor är något som befinner sig i konstant förändring påverkar rapportens replikerbarhet (Bryman, 2011). Därför har även ett så kallat "snapshot" (en bild) tagits från respektive webbplats för att belysa sidornas utforming vid det aktuella tillfället.

Resultat
-----------------------

All insamlad data återfinns i detta [Google spreadsheet](http://docs.google.com/spreadsheets/d/1_8b1M-eSrI1Bfuqs7tvk4Wj031Iqc-atJU42d5UTI6E/edit?usp=sharing).

#### Youtube Gaming ####

[FIGURE src=image/youtubegamingh328.webp?h=328 caption="Youtube Gaming"]

**De tre sidorna**

[youtube.com/gaming](http://www.youtube.com/gaming)  
[youtube.com/gaming/games](http://www.youtube.com/gaming/games)  
[youtube.com/gaming/live](http://www.youtube.com/gaming/live)

**Laddningstid**

Gaming: 6.2+ s  
Games: 4.9s  
Live: 5.9s  

**Antal resurser**

Gaming: 81  
Games: 50  
Live: 64  

**Total storlek**

Gaming: 7670kb  
Games: 7830kb  
Live: 6590kb  

**PageSpeed Insight score**

**Mobil**  
Gaming: 43  
Games: 46  
Live: 51  


**Desktop**  
Gaming: 48  
Games: 54  
Live: 49  

**Förbättringsmöjlighet**

Enligt Google PSI finns en rad förbättringsmöjligheter och de främsta är att läsa in viktiga resurser i förväg, att tillhandahålla en del av JavaScript koden inline samt att förbättra serverns svarstid. Huruvida det är värt att skriva JavaScript kod inline för att spara tid samtidigt som underhåll kommer försvåras är en fråga som behöver tas i åtanke. Intressant att notera är även att det på hem/gaming-sidan var roterande videos i en typ av banner, dessa laddas kontinuerligt in med ett visst intervall, således kommer sidan med tiden förbruka en stor mängd data i bakgrunden. Nu är detta dock en streaming-sida så hög användning av data är att räkna med. PSI påpekade även att bilder i rätt storlek och med modernt format är en viktig förbättringsmöjlighet, framför allt på mobilen. Mobila varianten av sidan har ingen löpande uppspelning av video förens man trycker på någon som sänder live, det innebär att just bilderna har stor påverkan på den mobila sidans laddningstid.  

#### Twitch ####

[FIGURE src=image/twitchtvh328.webp?h=328 caption="Twitch"]

**De tre sidorna**

[twitch.tv](http://www.twitch.tv)  
[twitch.tv/directory](http://www.twitch.tv/directory)  
[twitch.tv/p/en/about](http://www.twitch.tv/p/en/about/)

**Laddningstid**

Hem: 7.9+ s  
Directory: 5.2s  
About: 1.5s  

**Antal resurser**

Hem: 159  
Directory: 71  
About: 38  

**Total storlek**

Hem: 8540kb  
Directory: 6050kb  
About: 5160kb  

**PageSpeed Insight score**

**Mobil**  
Hem: 46  
Directory: 68  
About: 75  


**Desktop**  
Hem: 59  
Directory: 62  
About: 99  

**Förbättringsmöjlighet**

Enligt PSI så hade Twitch främst två områden där de hade förbättringsmöjligheter, bilder i form utav att använda sig av rätt storlek och av mordernare bildformat med bättre komprimering som således tar upp mindre data samt att använda sig utav lazy loading. Även att använda viss kod som inline code kom upp som ett förslag men det kan diskuteras utöver andra aspekter om det är någonting man skall fokusera på. Det var främst på mobilsidan som stora vinster kunde göras med hjälp utav moderna bildformat och rätt storlek och det är generelt också mobilen som har störst begränsningar när det kommer till data. Angående lazy-loading så laddade twitch hem profilbilder och spelbilder som låg utanför bild och där hade tid kunnat sparats genom att ladda dessa efter behov. Intressant att nämna är att även deras about-sida fick nedslag i just bilderna även om sidan i övrigt får avsevärt bättre PSI score, dock får dessa scores ta i beaktning vad för typ av sida vi jämför. Just twitch.tv/p/en/about har betydligt färre bilder och mediainnehåll än övriga.

#### Mixer ####

[FIGURE src=image/mixerh328.webp?h=328 caption="Mixer"]

**De tre sidorna**

[mixer.com](http://mixer.com/)  
[mixer.com/browse/games](http://mixer.com/browse/games)  
[mixer.com/browse/all](http://mixer.com/browse/all)  

**Laddningstid**

Hem: 7.9+ s  
Games: 3.4s  
All: 3.9s  

**Antal resurser**

Hem: 179  
Games: 79  
All: 123  

**Total storlek**

Hem: 22180kb  
Games: 11800kb  
All: 10370kb  

**PageSpeed Insight score**

**Mobil**  
Hem: 5  
Games: 7  
All: 7  


**Desktop**  
Hem: 47  
Games: 60  
All: 53  

**Förbättringsmöjlighet**

Återigen återfinns tipset om att använda nyare format när det kommer till bilder men just mixer verkar få extremt dåligt betyg på mobilen, hur kan det komma sig? Enligt PSI skulle den största tidsbesparingen vara att använda sig av preload, det vill säga att saker som är viktiga att ladda in snabbt eller direkt kan hämtas tidigare än vad de annars hade gjort. Som att hämta t.ex. ett stylesheet innan ett block med JavaScript körs. Det blir då cachat och är tillgängligt direkt när det behövs. Dessutom är Mixer väldigt stort så det finns mycket data att ta hem vilket kan vara ytterligare ett problem för mobilanvändare där mixers sidor i snitt tar ca dubbelt så mycket data att ladda jämnfört med youtube gaming och twitch.

Analys
-----------------------

**Slutsats**

Återkommande för samtliga sidor och i synnerhet när det kom till mobiler var bilder i form utav storlekar och format. Samtliga sidor fick nedslag på att de kunde valt att använda modernare bildformat samt att de borde använda sig utav rätt bildstorlek till mobilen för att på så sätt både spara data och får en snabbare laddningstid. Mobiler är dessutom mest känsliga för dataanvändning.

Utöver det var sådant som att skriva inline code för vissa mer kritiska kodsegment rekommenderat men frågan är om det laddningstid man vinner på det innebär en merkostnad i form utav underhåll av koden som gör det hela till något som inte är av intresse för respektive sida.

Även lazy-loading var ett återkommande inslag i förbättringsmöjligheterna, det innebär att man laddar in saker när de behövs istället för att ladda in allt på en gång. Det känns som en rimlig förbättring för dessa sidor då de laddar in spelbilder/profilbilder för hundratals spel och användare som alla inte får plats på skärmen samtidigt, många av vilka vi aldrig kommer att besöka. Men det måste erkännas att jag inte kan nog om lazy-loading för att sia om varför detta inte använts i större utsträckning.

Samtliga sidor levererar dessutom en ganska dålig upplevelse på mobilen, en brasklapp till deras försvar kan här dock vara att deras huvudfokus när det kommer till mobilanvänding är att leverera sitt innehåll till användare genom appar vars upplevelse är markant mycket bättre. Det kan vara en aspekt av de dåliga mobilresultaten, de fokuserar helt enkelt inte på sidorna i mobilens browser.

Det skall dessutom medges att dessa sidor kanske inte var de bästa att jämföra till den här uppgiften även om jag fann det mycket intressant. De är samtliga väldig stora sidor även om mixer är extremt i sammanhanget. De har alla mycket bilder och dessutom är hela tanken med dessa sidor att streama video (eller rättare sagt "gameplay"). Detta kommer i stor grad påverka verktyg som PSI och således kommer deras betyg där aldrig stå sig mot mer statiska sidor med lite bilder och ingen video. Även om valet inte var optimalt så tycker jag ändå att resultatet varit givande och det sidornas natur till trots även gett insikter som kan vara bra att ha i åtanke till icke streamingsidor. Trots allt var mycket av förbättringsförslagen relaterade till bilder och bildformat.

**Ranking**

1. Twitch (Avg. size: 6.5mb, load time: 6.6s, PSI score: 59)*  
2. Youtube (Avg. size: 7.4mb, load time: 5.7s, PSI score: 49)  
3. Mixer (Avg. size: 14.8mb, load time: 5.1s, PSI score: 30)

Vinnare i testet är Twitch som i snitt har minst sidor och bäst PSI score, samtidigt är twitch den långsammaste sidan att ladda överlag men det är inget som upplevs som en markant skillnad i verkligheten då samtliga sidor är väldigt långsamma att ladda. Youtube är bra överlag och tar därmed en andraplats medans Mixer kommer på sista plats sin snabba(relativt) laddningstid till trots, Mixer får sämst PSI score och är i snitt dubbelt eller mer än dubbelt så stor att ladda hem jämfört med sina konkurrenter.

*\*Twitch har inte fått sina hastigheter och PSI-poäng medräknade från sin mer traditionella sida då den skilde sig markant från de övriga sidorna och hade fått twitch att framstå bättre än vad de är när lika ställs mot lika.*

**Vad är snabbt eller långsamt?**

Vad som är snabbt eller långsamt är egentligen till viss del något som är relativt. Personligen tycker jag att mer än några sekunder är irriterande långsamt så någonting under 2-3 sekunder tycker jag ändå är snabbt. Med det sagt så måste man ha en viss förståelse för sidans innehåll när man sätter sina förväntningar. Jag hade blivigt ordentligt exalterad om någon av de ovanstående sidorna laddade så snabbt men jag kan i ärlighetens namn inte säga att jag förväntar mig det. Dock är det ju en potentiell aspekt som kan förbättras för att konkurrera ut de andra men frågan är då också vad hastigheten sker på bekostnad av. Just streaming-sidor handlar kanske i första hand om hög kvalitet och i andra hand om laddningstid, är då samtliga sidor långsamma att ladda så vänder sig troligen användarna till den sidan som kan erbjuda bäst innehåll. Samtliga sidor är dock i min smak fortfarande långsamma och de klarar inte mitt gränsvärde men vill jag se på en stream har jag inte mycket till val.


Referenser
-----------------------

Bryman, Alan (2011). *Samhällsvetenskapliga metoder*. 2., [rev.] uppl. Malmö: Liber

Blekinge Tekniska Högskola (2019, December 3). *Genomgång kmom05 design med Niklas* [Videofil]. Hämtad från https://www.youtube.com/watch?v=NRSXSrdK1Ew

Övrigt
-----------------------

Rapporten är skriven av Patrik Arvius.