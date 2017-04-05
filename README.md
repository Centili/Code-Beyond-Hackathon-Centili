# Code Beyond Hackathon Centili
### &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;MPG - Mobile Payments Geotracking

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;[![N|Centili](https://s21.postimg.org/njuiuy3rb/centili-logo-min.png)](http://www.centili.com)


### O nama
Centili je globalni provajder tehnologija za mobilno plaćanje koji pomaže mobilnim operaterima i digitalnim kompanijama da omoguće svojim korisnicima brz pristup online uslugama, proizvodima i sadržaju, istovremeno pružajući mobilnim korisnicima jednostavan i siguran način online plaćanja. 
Fokus nam je podsticanje poslovnog rasta za mobilne operatere, online kompanije, developere mobilnih aplikacija i pružaoce digitalnog sadržaja, dok je glavna vizija koja nas pokreće to da svim ljudima koji nemaju pristup tradicionalnim načinima plaćanja omogućimo pristup i infrastrukturu za jednostavno online plaćanje putem njihovih prepaid ili postpaid računa.

### Zadatak
Uz ogromno tržište koje pokrivamo i brojem telekom operatera sa kojima smo povezani, ponekad je teško vizualizovati rad našeg sistema. Pojavila se potreba za mogućnošću praćenja transakcija i revenue-a koji se odvijaju u okviru naše platforme širom sveta u realtime mode-u, na intuitivan i interaktivan način.
Vaš zadatak je da napravite softversko rešenje koje obrađuje transakcije koje prolaze kroz našu platformu i omogućava real-time praćenje i prikazivanje svih transakcija na svetskoj mapi u okviru našeg sistema.
Kao izvor transakcija ćete dobiti generator podataka koji će simulirati rad naše platforme i obezbediti vam potrebne ulazne podatke za realizaciju rešenja. Broj transakcija koji obrađuje naša platforma je veliki, stoga generator može da simulira proizvoljan broj transakcija po minuti, pa je jedan od vaših zadataka da rešenje podrži što veći broj transakcija u jedinici vremena.
Jedna od mogućih primena ovakvog servisa je povezivanje ekrane kako bismo svakodnevno u office-u mogli da pratimo broj transakcija u celom svetu i imamo uvid u funkcionisanje platforme širom sveta.

### Tehnologija
Dozvoljeno je korišćenje bilo koje platforme i tehnologije za razvoj vašeg rešenja. Takođe je moguće koristiti kombinaciju više platformi i tehnologija. Dozvoljeno je korišćenje svih javno dostupnih API-ja.
Potrebno je koristiti bilo koji version control system (Git, SVN, GitHub) za upravljanje vašim rešenjem. Link ka repozitorijumu je potrebno dostaviti mentorima iz Centilija nakon kreiranja istog.

### GeoTrackingDataGenerator
Za potrebe generisanja podataka napravili smo vam malu klijentsku aplikaciju koja generiše nasumične podatke koji reprezentuju realne podatke sa kojima radi naša platforma.

Generator je napisan u Javi i stoga vam je potrebna Java 8 kako biste ga pokrenuli na vašoj mašini. On generiše nasumične podatke i HTTP POST request-om šalje JSON objekat na adresu koju specificirate kao argument prilikom pokretanja aplikacije iz komandne linije. Takođe, generator prima još jedan ulazni argument, koji predstavlja broj request-ova po minuti. Oba parametra su obavezna.
Generator se pokreće izvršavanjem komande u komandnoj liniji.
Generator možete preuzeti na sledećem [link-u](https://github.com/Centili/Code-Beyond-Hackathon-Centili/raw/master/GeoTrackingDataGenerator/GeoTrackingDataGenerator.jar).
##### Primer:
Ukoliko se GeoTrackingDataGenerator.jar nalazi na **C** particiji u folderu Centili, za pokretanje se koristi komanda:
```sh
java -jar C:\Centili\GeoTrackingDataGenerator.jar http://localhost:8080/receive 60
```
**Obavezno je koristiti podatke koje stvara generator podataka.**

### Komunikacija
Sva komunikacija sa mentorima i kompanijom Centili se vršiti preko Slack platforme. Kreiran je zaseban tim za svrhu ovog hakatona. Poziv za Slack tim ste dobili na vašu email adrese. Ohrabrujemo vas da slobondo kontaktirate mentore i pitate za sve nedoumice, a mi ćemo se potrudi da vam u što kraćem roku odgovorimo. Tim sadži javni kanal #general koji preporučujemo za FAQ kako bi svi članovi i timovi videli sadržaj i kako bi izbegli redundantnost. Ako imate pitanje koje je specifično samo za vas možete ga postaviti u privatnom kanalu koji će biti dodeljen svakom timu.
