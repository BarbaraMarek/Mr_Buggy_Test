# Mr_Buggy_Test

**Moje spostrzeżenia jeszcze przed zapoznaniem się ze specyfikacją:**

**I.**          **Użytkownicy:**

 

**A)**   **Super administrator:**

\1.    Za każdym razem trzeba dodawać administratora

\2.    Można dodać drugiego administratora o takiej samej nazwie, ale z innym hasłem niż ten pierwszy 

\3.    Nie można usunąć danych administratora z bazy

\4.    Dodałam 3 super administratorów i za 4 włączeniem programu już poprosiło mnie o autoryzację, a nie o ponowne dodanie super administratora. Ciekawe…

 

**B)**   **Dodanie nowego użytkownika:**

\5.    Można dodać 2 nowych użytkowników o tej samej nazwie, ale innych danych osobowych, np. o innym imieniu

\6.    Nie ma podglądu hasła (nie jest to błąd, ale mógłby być)

\7.    Można dodać 2 i więcej użytkowników o tym samym haśle, ale o innych danych osobowych (PaniA, PaniB, PaniC)

\8.    Można dodać dwóch takich samych użytkowników

\9.    Nie można dodać hasła o mniejszej liczbie znaków niż 8 i o większej liczbie znaków niż 32 – więc jest ok

\10.  Można dodać użytkownika o tych samych danych osobowych, który będzie zarówno zwykłym użytkownikiem jak i administratorem 

\11.  Wszystkie wymagane pola muszą być wypełnione, więc jest ok

\12.  Nie można kopiować tekstu, który znajduje się w polu hasła, więc jest ok

\13.  Nie można dodać nazwiska z małej litery, ale imię już tak…

\14.  Nie można dodać cyfry w imieniu 

\15.  W opisie błędu do imienia nazwano znaki specjalne słowami, natomiast w opisie błędu do nazwiska symbolami. Powinno się to ujednolicić, albo tak, albo tak żeby w dwóch miejscach było tak samo.

\16.  W nazwisku może być duża litera w środku albo na końcu wyrazu. Trochę to nielogiczne… Powinna być dozwolona tylko na początku lub po znaku „-„

\17.  Jeśli w polu hasło wpisze się: „    „ (8 znaków spacji, to wyskakuje błąd, że pole jest wymagane)

 

**C)**   **Sortowanie po kolumnach:**

\18.  Źle się sortuje po Id (1, 10, 11, …, 2, 3) zamiast 1,2,3,4,… 

\19.  Typ posortowałabym inaczej: Super administrator, administrator, zwykły użytkownik, a nie: Administrator i dopiero potem Super administrator

\20.  Pokazywanie się na jednej stronie do 20 użytkowników jest ok, po dodaniu 21 pokazuje się następna strona. Pokazywanie się na jednej stronie do 40 użytkowników jest ok, po dodaniu 41 pokazuje się następna strona. Sprawdzić czy działa dla pozostałych wartości.

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image002.jpg)

 

**D)**   **Edycja danych użytkownika:** 

\21.  Tutaj chyba wszystko jest ok

 

**E)**   **Usuwanie użytkownika**

\22.  Tutaj chyba wszystko jest ok

\23.  Jak zaznaczę z ctrl to usuwa się tylko jeden użytkownik, nie powinno się dać zaznaczyć dwóch naraz 

 

**F)**   **Dodanie projektu do użytkownika**

\24.  Po próbie dodania użytkownika do projektu wyskakuje błąd: „Podany użytkownik nie istnieje” – to w ogóle trzeba przecież podać nazwę projektu, a nie użytkownika chyba. Nie można dodać użytkownika do projektu jeśli żaden projekt jeszcze nie istnieje.

\25.  Po dodaniu projektu do listy projektów można już przypisać danego użytkownika do danego projektu – jest ok

\26.  Do projektu użytkownika można przypisać tylko jeden raz – to jest ok

\27.  Nie można przypisać użytkownikowi dwóch ról w projekcie – sprawdzić ze specyfikacją czy to jest ok 

 

**II.**         **Projekty**

 

**G)**   **Dodanie nowego projektu**

 

\28.  Menadżer projektu – aby dodać menadżera projektu trzeba zacząć wpisywać od nazwiska, aby pojawiła się lista rozwijana. Nie ma żadnej podpowiedzi co należy wpisać i należy się tego domyślać. Tak nie powinno być. Jeśli wpisze się nazwę użytkownika lub imię wyskakuje błąd: „Podany użytkownik nie istnieje”.

\29.  Można dodać dwa projekty o takim samym prefixie i nazwie, ale z innym menadżerem

\30.  Można dodać projekt o takim samym prefixie, ale o innej nazwie niż ten już istniejący, ale o takiej samej nazwie niż też już istniejący

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image004.jpg)

 

\31.  Nie ma listy rozwijanej przy wyborze menadżera, trzeba go znać z nazwiska, a przydałaby się moim zdaniem 

\32.  Nie można dodać prefixu o mniejszej liczbie znaków niż 3 i o większej liczbie znaków niż 7 – więc jest ok

\33.  Nieprawidłowe sortowanie po: Id, Prefiksie, nazwie:

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image006.jpg)

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image008.jpg)

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image010.jpg)

 

**H)**   **Edycja projektu – działa**

**I)**    **Usuwanie projektu – działa**

**J)**    **Pozostałe ikonki (zarządzaj: użytkownikami, wersjami, komponentami i środowiskami) są nieaktywne**

 

**III.**        **W zakładce incydenty nic się nie da zrobić** **L** 

 

**W edycji danych administratora nie trzeba podawać aktualnego hasła żeby zmienić hasło. Czy to błąd?** 

**TERAZ ZBADAĆ PROGRAM NA PODSTAWIE WYMAGAŃ !!!**

**
**

 

**Błędy po zapoznaniu się ze specyfikacją** 

**Adnotacje do specyfikacji:** 

**2. Założenia ogólne**

Tworzenie projektów – ok

Dodawanie raportów z incydentów wewnątrz projektów – gdzie to? 

Zarządzanie incydentami – ok

**2.1. Projekty**

Można tworzyć projekty, edytować je i usuwać, ale nie wiem jak nimi zarządzać, bo pola do zarządzania są szare, nieaktywne (Użytkownicy, Wersje, Komponenty, Środowiska)

Po najechaniu myszką na opcje projektu w menu dolnym pojawiają się dodatkowe opisy, np. dodaj nowy projekt. Natomiast po najechaniu myszką na projekt w menu górnym dodatkowy opis pojawia się tylko w przypadku opcji „Użytkownicy”. W pozostałych opcjach nie pojawia się. 

**2.2. Zarządzanie incydentami**

 Wszystkie opcje są nieaktywne. Nie wiem, gdzie jest rozwiązywanie incydentów. Chyba, że to jest status incydentu, to ok. 

Po najechaniu myszką na opcje *Incydentu* w menu dolnym pojawiają się dodatkowe opisy. Natomiast po najechaniu myszką na *Incydent* w menu górnym dodatkowe opisy opcji nie pojawiają się. 

**2.3. Użytkownik**

Po najechaniu myszką na opcje *Użytkownika* w menu dolnym pojawiają się dodatkowe opisy. Natomiast po najechaniu myszką na *Użytkowników* w menu górnym dodatkowe opisy opcji nie pojawiają się. 

W tym komponencie można dodać użytkownika, edytować jego dane lub usunąć użytkownika. Można również wyświetlić do jakiego projektu przypisany jest użytkownik lub dodać użytkownika do projektu, ale projekt ten musi być już utworzony wcześniej w zakładce *Projekty.* Nie wiem, gdzie tu można administrować systemem. 

**3. Konwencje**

**3.1. Załączniki** 

**Sprawdzić ten punkt, bo na razie nic nie da się dodać…**

**3.2. Filtrowanie i sortowanie**

Można sortować, ale sortowanie to jest błędne. Zamiast 1,2,3,…,10,11,12… sortuje się następująco: 1,10,11,12,2,3,4,5,6,7,77,… Nie widzę opcji filtrowania danych…

**3.3.** **Nr obiektu**

**Nie rozumiem tego punktu… Wrócić do niego później**

**3.4. Pole obowiązkowe**

Tu jest ok póki co 

**4. Budowa systemu** 

**4.1. Projekty**

Skoro jest podstawową jednostką w aplikacji to dlaczego jest dopiero drugą zakładką, a nie pierwszą? Nie umiem dodać incydentu, więc ciężko stwierdzić czy wewnątrz projektu znajdują się raporty z incydentów. Na razie się nie znajdują. 

**Można dodać dwa projekty o tej samej nazwie, ale o innym prefiksie – niezgodność ze specyfikacją, która mówi, że każdy projekt ma indywidualną nazwę. Można nawet dodać dwa projekty o tej samej nazwie i tym samym prefiksie!!! Toż to skandal :D** 

„Dla zwykłego użytkownika zakładka Projekty nie będzie widoczna do czasu przypisania tego użytkownika do projektu.” Nie wiem, musiałabym się przelogować na zwykłego użytkownika. Dla mnie na razie jest widoczna, ale jestem Super administratorem :D 

„Dodatkowo, jeśli użytkownik jest Superadministratorem lub Administratorem, w tym komponencie
 systemu dostępne są dodatkowe funkcje administracji projektami, np. dodawanie, edycja i usuwanie
 projektów.” Dla Superadministratora jest ok, dla Administratora nie wiem, musiałabym się akoś przelogować. 

**4.2. Incydenty – na razie nic nie umiem zrobić w tej zakładce** 

**4.3. Użytkownicy**

„Komponent dostępny tylko dla osoby z uprawnieniami Superadministratora” - ok „lub Administratora. Dla pozostałych użytkowników zakładka jest niewidoczna.” – nie wiem, muszę się przelogować.

„W tym komponencie istnieje możliwość dodawania, edycji lub usuwania użytkowników.” – ok, takie akcje oraz przypisanie użytkownika do projektu można wykonać dla administratorów i zwykłych użytkowników, natomiast nie można ich wykonać w przypadku Super administratorów (pola te są nieaktywne). 

**5. Pierwsze uruchomienie**

**5.1. Ekran 1 – Definiowanie baz danych**

Jest ok, ale tylko jak się wpisze dane z dokumentu konfiguracyjnego. Czyli root, hasło takie jak podane przy konfiguracji, locallhost, port 3306, mr_buggy (Ja wpisałam mr_buggy1, bo odinstalowałam i zainstalowałam program jeszcze raz oraz utworzyłam nową bazę danych i nazwę mr_buggy1 wpisałam w MySQL Command Line Client). Układ pól zgodny ze specyfikacją.

**5.2. Ekran 2 - Zakładanie konta superadministratora**

Układ pól zgodny ze specyfikacją. 

| ![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image012.jpg) | ![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image014.jpg) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

 

„Problemy z walidacją w aplikacji są wyświetlane jako pokolorowanie nazwy błędnego pola z dodatkową podpowiedzią po najechaniu kursorem.” **- ok** 

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image015.png)

***Nazwa użytkownika:\***

Max 50 znaków - ok
 Min 3 znaki - ok

Pole wymagane - ok
 Dopuszczalne są litery oraz znaki „._-” - Nie można wpisać polskich znaków. Komunikat: „Niepoprawna nazwa użytkownika. Dozwolone znaki to małe i duże litery, cyfry oraz znaki: ._- ‘’. 

Reszta ok, długość zgodna ze specyfikacją, pole musi być wymagane, duże i małe litery oraz znaki: ._- wchodzą. Reszta znaków specjalnych nie wchodzi: !@#$%^&*()_-+={[}]|\:;”’<,>.?/

 

***Hasło\*****:** 

Długość 8-32 znaki – ok

Dozwolone wszystkie znaki – właśnie, że nie, bo spacja nie wchodzi. Same spacje nie wchodzą. Komunikat: „Pole jest wymagane”. Spacja na początku,  w środku i na końcu może być. Reszta znaków działa – duże i małe litery, znaki specjalne, polskie znaki.

***Powtórz hasło:\***

Długość 8-32 znaki – pole może zawierać mniej niż 8 znaków (nie pojawia się komunikat o błędzie), ale logowanie i tak nie przejdzie, bo nie przejdzie hasło. 

Dozwolone wszystkie znaki – właśnie, że nie, bo spacja nie wchodzi. Komunikat: „Pole jest wymagane”. Reszta znaków działa – duże i małe litery, znaki specjalne, polskie znaki.

„Pole „hasło” i „powtórz hasło” muszą być takie same” – ok, działa również dla różnej wielkości liter. Wielkości liter w obu hasłach musi być taka sama. 

 

***Imię\*****:**

 

2-32 znaków - ok
 małe, duże litery - ok
 oraz spacja - ok
 apostrof - ok

Pole wymagane – ok

 

***Nazwisko:\***

 

2-32 znaków – Można wpisać więcej niż 32 znaki (do 64 znaków: taki też jest opis błędu). 
 małe, duże litery - ok
 oraz znaki „-'” - ok
 Pole wymagane – ok

 

**E-mail:**

 

Domyślna walidacja adresów email – ok

 

***Przyciski: OK i Anuluj\*** – ok

 

 



 

Poprawnie wypełniony formularz:

 

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image017.jpg)

 

**6. Logowanie**

 

Po instalacji użytkownik może uruchomić aplikację oraz zalogować się. Pierwszy ekran wyświetlony po uruchomieniu aplikacji to ekran autoryzacji. 

Błąd: Po drugim i każdym kolejnym uruchomieniu aplikacji ponownie pojawia się pole dotyczące zakładania konta Super administratora. Po jakimś czasie już się udało zalogować bez zakładania konta Super administratora. 

Konto to można założyć na inne dane Super administratora niż za pierwszym razem:

 

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image018.png)

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image019.png)

 

Można założyć je również na takie same dane Super administratora jak za pierwszym razem:

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image020.png)

 

Po paru uruchomieniach aplikacji mam 8 Super administratorów, których nie mogę usunąć… Nie mogę przejść do logowania bez założenia konta dla nowego Super administratora.

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image022.jpg)

 

 

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image024.jpg)

**Pole tekstowe - OK**

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image026.jpg)

**Hasło - OK**

 

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image028.jpg)

**Przycisk „OK”** **– Błąd: Można podać błędne hasło więcej niż 3 razy i nic się nie dzieje. Konto nie jest blokowane. Pojawia się tylko komunikat o błędnym haśle.** 

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image030.jpg)

**Przycisk „Anuluj” – OK**

**Widok okna głównego zgodny ze specyfikacją:** 

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image032.jpg)

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image034.jpg)

 

**7. Użytkownicy**

 

**7.1. Superadministrator** **- Sprawdzone**

Pierwsze konto - konto superadministratora - jest konfigurowane na etapie instalacji produktu. Nazwa użytkownika oraz hasło są ustalane na etapie instalacji. Podczas tworzenia tego konta na ekranie konfiguracyjnym należy podać adres email. Błąd: Nie trzeba podawać adresu email. Konta superadministratora nie da się usunąć. W odróżnieniu od uprawnień zwykłego administratora, nie można odebrać uprawnień superadministratorowi. **- ok**

**7.2. Administrator** **– Sprawdzić** 

Uprawnienia administratora może nadać lub odebrać tylko inny administrator lub superadministrator. Administrator otrzymuje globalne prawa w ramach całej aplikacji. Ponadto, w ramach konkretnych projektów może mieć również uprawnienia Menedżera projektu, Testera lub Naprawiacza. – Sprawdzić to będąc zalogowanym jako administrator i zwykły użytkownik. Sprawdzić uprawnienia w ramach konkretnych projektów. 

**7.3. Zwykły użytkownik - Sprawdzone**

Użytkownik, który nie ma prawa modyfikowania innych kont. - OK, może on dodawać tylko nowe incydenty. Wszystkie pola związane z użytkownikami są nieaktywne. 

**7.4. Menedżer projektu**

Menedżer projektu to osoba zarządzająca pojedynczym projektem w aplikacji Mr Buggy. Jest to osoba pośrednicząca między testerami a naprawiaczami, która określa, jakie incydenty zostaną naprawione jako błędy, a które nie. Aplikacja Mr Buggy ustala Menedżera projektu jako osobę pośrednią, która określa, czy incydenty zgłoszone przez osoby weryfikujące powinny trafić do osób rozwiązujących. – Sprawdzić 

**7.5. Tester/Naprawiacz**

Tester to osoba uczestnicząca w jednym lub wielu projektach. Jego zadaniem jest dodawanie incydentów oraz weryfikacja tego, czy incydenty zostały prawidłowo rozwiązane. Naprawiacz z kolei podobnie jak tester może uczestniczyć w dowolnej ilości projektów. Jego zadaniem jest rozwiązywanie incydentów dodanych do bazy przez testerów oraz przesyłanie ich do weryfikacji. – Sprawdzić 

**7.6. Matryca uprawnień – Sprawdzić czy matryca pokrywa się z tym co napisano powyżej**

Uprawnienia z grupy (1) oraz (2) można łączyć, tj. osoba można na raz być administratorem całej aplikacji Mr Buggy oraz Menadżer Projektu w projekcie X, jak i Testerem w projekcie Y.

\- Literówka powinno być Menadżerem 

**7.7. Lista użytkowników - Sprawdzone**

Administrator ma również dostęp do listy wszystkich użytkowników systemu. Lista prezentuje wszystkie konta zarejestrowane w systemie. Pierwsza kolumna wskazuje numer użytkownika w bazie danych, druga wskazuje nazwę użytkownika, kolejne imię, nazwisko, adres e-mail, typ konta oraz status konta. **- OK**

**7.8. Tworzenie nowego użytkownika - Sprawdzone**

Po zalogowaniu do aplikacji, Administrator ma dostęp do ekranu Użytkownik. Po wybraniu z menu
 Użytkownik opcji Dodaj Nowego Użytkownika, Administrator dostaje się do ekranu, na którym ma
 możliwość stworzyć nowe konto użytkownika. Na danym ekranie dostępne będą takie same pola jak opisane w tabeli Ekran 2 „Zakładanie konta superadministratora” z uzupełnieniem o typ określający czy jest to zwykły użytkownik czy też administrator. **– OK**

Moja uwaga: konto nowego użytkownika może utworzyć administrator, ale może go też utworzyć superadministrator. 

Układ pól zgodny ze specyfikacją. 

| ![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image036.jpg) | ![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image037.png) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

**Nazwa użytkownika musi być unikalna.** **– Błąd:**

**Można założyć dwa takie same konta użytkowników (wszystkie pola takie same). Można założyć dwa konta o tej samej nazwie użytkownika, ale z innym hasłem. Można założyć dwa konta o tej samej nazwie, ale innych pozostałych danych osobowych. Można utworzyć dwa konta o tej samej nazwie i pozostałych polach, ale innym typie użytkownika. Czyli taki sam użytkownik może być jednocześnie zwykłym użytkownikiem i administratorem. Może mieć różne imiona, nazwiska i hasła oraz maile.** 

**W tym oknie są dokładnie takie same błędy jak w oknie „Ekran 2”:**

***Nazwa użytkownika:\***

Max 50 znaków - ok
 Min 3 znaki - ok

Pole wymagane - ok
 Dopuszczalne są litery oraz znaki „._-” - Nie można wpisać polskich znaków. Komunikat: „Niepoprawna nazwa użytkownika. Dozwolone znaki to małe i duże litery, cyfry oraz znaki: ._- ‘’. 

Reszta ok, długość zgodna ze specyfikacją, pole musi być wymagane, duże i małe litery oraz znaki: ._- wchodzą. Reszta znaków specjalnych nie wchodzi: !@#$%^&*()_-+={[}]|\:;”’<,>.?/

***Hasło\*****:** 

Długość 8-32 znaki - ok

Dozwolone wszystkie znaki – właśnie, że nie, bo spacja nie wchodzi. Same spacje nie wchodzą. Komunikat: „Pole jest wymagane”. Spacja na początku,  w środku i na końcu może być. Reszta znaków działa – duże i małe litery, znaki specjalne, polskie znaki.

***Powtórz hasło:\***

Długość 8-32 znaki – pole może zawierać mniej niż 8 znaków (nie pojawia się komunikat o błędzie), ale logowanie i tak nie przejdzie, bo nie przejdzie hasło. 

Dozwolone wszystkie znaki – właśnie, że nie, bo spacja nie wchodzi. Komunikat: „Pole jest wymagane”. Reszta znaków działa – duże i małe litery, znaki specjalne, polskie znaki.

„Pole „hasło” i „powtórz hasło” muszą być takie same” – ok, działa również dla różnej wielkości liter. Wielkości liter w obu hasłach musi być taka sama. 

 

***Imię\*****:**

 

2-32 znaków - ok
 małe, duże litery - ok
 oraz spacja - ok
 apostrof - ok

Pole wymagane – ok

 

 

 

 

***Nazwisko:\***

 

2-32 znaków – Można wpisać więcej niż 32 znaki (do 64 znaków: taki też jest opis błędu). 
 małe, duże litery - ok
 oraz znaki „-'” - ok
 Pole wymagane – ok

 

**E-mail:**

 

Domyślna walidacja adresów email – ok

 

**Typ:**

 

Administrator - ok

Zwykły użytkownik - ok

 

***Przyciski: OK i Anuluj\*** – ok

 

Przykładowy poprawnie wypełniony formularz:

![img](file:///C:\Users\basia\AppData\Local\Temp\msohtmlclip1\01\clip_image038.png)

 

**7.9. Edycja danych użytkownika - Sprawdzone**

Administrator systemu ma dostęp do ekranu edycji danych użytkownika. Ekran ten umożliwia zmianę
 wszystkich danych użytkownika. **- OK działa, wszystkie pola można zmienić**

Moja uwaga: konto użytkownika może edytować administrator, ale może go też edytować superadministrator.

Moja uwaga: Żeby zmienić hasło nie trzeba znać starego hasła. Czy tak powinno być? 

 

**7.10. Usuwanie użytkownika - Sprawdzone**

Usunięcie użytkownika z aplikacji jest możliwe (za wyjątkiem konta superadministratora). – OK, Administrator oraz Superadministrator mogą usunąć konto zwykłego użytkownika oraz innego administratora. Nie można natomiast usunąć konta Superadministratora. 

Moja uwaga: nie można usunąć kota administratora, którym się jest aktualnie zalogowanym. Nie ma tego w specyfikacji, ale to chyba dobrze, że nie można usunąć w danej chwili takiego konta.

 

**8. Edycja ról użytkowników w projektach**

 