# JMBAG
0036494620
#Pitanje 1
Primjećujem da su uz debug datoteke program.cs, također i ClassLibrary1 datoteke. Kada pokušamo pokrenuti executable datoteku, aplikacija nam se sruši i javlja da ne može učitati datoteku ClassLibrary1. Zato što se u datoteci ClassLibrary1.dll nalazi klasa s metodom PrintHelloWorld koju koristimo u nasoj aplikaciji. Ako me trazite da vam pošaljem aplikaciju poslao bih .dll i .exe datoteke.
#Pitanje 2
Kad promijenimo string u class library projektu, i pokrenemo aplikaciju pomocu exe datoteke ne mijenja se ispis, ali ukoliko probamo napraviti build same konzolne aplikacije bez class library, ne možemo, jer nam je class library referenciran i on se builda zajedno s nasim projektom konzolne aplikacije. U početnoj situaciji očito je da se neće promijeniti ispis jer tada exe datoteka koristi class library-ev .dll koji je zadnji buildan.
#pitanje 3
Pero: Hello World
#pitanje 4
Dodan nam je i PeroClassLibrary.dll file u mapu Debug.
#pitanje 5
Ako brišemo .dll aplikacija jos uvijek radi, i možemo raditi build. Aplikacija radi jer još uvijek ima svoju lokalnu inačicu .dll file-a. Build je primjetio da mu nedostaje originalni .dll file ali je shvatio da je napravio već jednu kopiju u mapi debug i referencira se na tu kopiju.
#pitanje 6
Build je izvršen bez grešaka, NodaTime je ponvno nazad u packages mapi.