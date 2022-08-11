# Markdown Cheatsheet


## Nagłówki

# H1
## H2
### H3
#### H4
##### H5
###### H6

Alternatywnie, dla H1 i H2 styl podkreślenia:

Alt-H1
======

Alt-H2
------


## Podkreślenie

Wyróżnienie, czyli kursywa, z *gwiazdkami* lub _podkreśleniami_.

Silne podkreślenie, czyli pogrubienie, z **gwiazdkami** lub __podkreśleniami__.

Połączone wyróżnienie z **gwiazdkami i _podkreśleniami_**.

Przekreślenie wykorzystuje dwie tyldy. ~~Podrap to.~~


## Listy

1. Pierwsza zamówiona pozycja na liście
2. Kolejny przedmiot
   * Nieuporządkowana podlista.
1. Rzeczywiste liczby nie mają znaczenia, tylko to, że to liczba
   1. Zamówiona podlista
4. I kolejny przedmiot.
   
    Jakiś tekst, który powinien być dopasowany do powyższego elementu.

* Lista nieuporządkowana może zawierać gwiazdki
- Lub minusy
+ Lub plusy


## Tworzenie połączeń
Istnieją dwa sposoby tworzenia linków.

[Jestem linkiem w stylu inline](https://www.google.com)

[Jestem łączem w stylu referencyjnym][Dowolny tekst referencyjny bez uwzględniania wielkości liter]

[Możesz użyć liczb dla definicji linków w stylu referencyjnym][1]

Lub pozostaw to puste i użyj [samego tekstu linku]

Adresy URL i adresy URL w nawiasach ostrych zostaną automatycznie przekształcone w linki.
http://www.example.com lub <http://www.example.com>, a czasami
example.com (ale nie na przykład na Github).

Trochę tekstu, aby pokazać, że linki referencyjne można później wykorzystać.

[arbitralny tekst referencyjny bez uwzględniania wielkości liter]: https://www.mozilla.org
[1]: http://slashdot.org
[sam tekst linku]: http://www.reddit.com


## Obrazy

Oto nasze logo (najedź, aby zobaczyć tekst tytułu):

Styl wbudowany:
![tekst alternatywny](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Tekst tytułu logo 1")

Styl referencyjny:
![tekst alternatywny][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Tekst tytułu logo 2"


## Podświetlenie kodu i składni
Bloki kodu są częścią specyfikacji Markdown, ale podświetlanie składni już nie. Jednak wiele programów renderujących — takich jak Github i Markdown Here — obsługuje podświetlanie składni. Markdown Here obsługuje podświetlanie dla kilkudziesięciu języków (i nie-tak naprawdę-języków, takich jak diff i nagłówki HTTP); aby zobaczyć pełną listę i jak pisać nazwy języków, zobacz stronę demonstracyjną highlight.js .

Wbudowany „kod” ma „wsteczne kleszcze”.

Bloki kodu są ogrodzone liniami z trzema znakami zaznaczenia ```lub wcięte czterema spacjami. Polecam tylko używanie chronionych bloków kodu - są łatwiejsze i tylko obsługują podświetlanie składni.

```javascript
var s = "Podświetlanie składni JavaScript";
alert(y);
````
 '''
„python”
s = "Podświetlanie składni Pythona"
drukuj
````
 
````
Nie wskazano języka, więc nie ma podświetlania składni.
Ale dorzućmy <b>tag</b>.
````

var s = "Podświetlanie składni JavaScript";
alert(y);

s = "Podświetlanie składni Pythona"
drukuj

Nie wskazano języka, więc nie ma podświetlania składni w Markdown Here (różni się na Github).
Ale dorzućmy <b>tag</b>.

Aby zobaczyć, jakie języki są dostępne do podświetlania i jak wpisywać nazwy tych języków, zobacz stronę demonstracyjną highlight.js .


## Przypisy
Przypisy nie są częścią podstawowej specyfikacji Markdown, ale są obsługiwane przez GFM .

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].  

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]: Every new line should be prefixed with 2 spaces.  
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.  
    This footnote also has been made with a different syntax using 4 spaces for new lines.


## Tabele
Tabele nie są częścią podstawowej specyfikacji Markdown, ale są częścią GFM i Markdown Here je obsługuje. Są łatwym sposobem dodawania tabel do wiadomości e-mail — zadanie, które w innym przypadku wymagałoby kopiowania i wklejania z innej aplikacji.

Dwukropki można wykorzystać do wyrównania kolumn.

| Tabele | Czy | Fajne |
| ------------- |:-------------:| -----:|
| kolumna 3 to | wyrównany do prawej | $1600 |
| kolumna 2 to | wyśrodkowany | 12 zł |
| paski zebry | są schludne | 1 USD |

Zewnętrzne rury (|) są opcjonalne i nie musisz ładnie układać surowej linii Markdown. Możesz także użyć wbudowanego Markdowna.

Przecena | Mniej | Ładny
--- | --- | ---
*Nadal* | „renderuje” | **ładnie**
1 | 2 | 3


## Cytaty blokowe

> Cytaty blokowe są bardzo przydatne w wiadomościach e-mail do emulacji tekstu odpowiedzi.
> Ten wiersz jest częścią tego samego cytatu.

Przerwa na wycenę.

> Jest to bardzo długa linijka, która nadal będzie poprawnie cytowana po zakończeniu. Och chłopcze, piszmy dalej, aby upewnić się, że to wystarczająco długo, aby rzeczywiście zapakować dla wszystkich. Och, możesz *wstawić* **Markdown** do cytatu blokowego. 


## Wbudowany kod HTML
Możesz także użyć surowego HTML w swoim Markdown i będzie on w większości działał całkiem dobrze.

<dl>
   <dt>Lista definicji</dt>
   <dd>Jest czymś, czego ludzie czasami używają.</dd>

   <dt>Markdown w HTML</dt>
   <dd> *Nie* działa **bardzo** dobrze. Użyj <em>znaczników</em> HTML.</dd>
</dl>

## Linia pozioma

Trzy lub więcej...

---

Myślniki

***

Gwiazdki

___

Podkreślenia

## Podziały wierszy
Moim podstawowym zaleceniem, aby nauczyć się, jak działa podział linii, jest eksperymentowanie i odkrywanie -- naciśnij <Enter> raz (tj. wstaw jeden znak nowej linii), a następnie naciśnij go dwa razy (tj. wstaw dwa nowe wiersze), zobacz, co się stanie. Wkrótce nauczysz się dostawać to, czego chcesz. "Przełącznik Markdown" jest twoim przyjacielem.

Oto kilka rzeczy do wypróbowania:

Oto linia, od której możemy zacząć.

Ta linia jest oddzielona od powyższej dwoma znakami nowej linii, więc będzie to *oddzielny akapit*.

Ta linia to także osobny akapit, ale...
Ta linia jest oddzielona tylko pojedynczym znakiem nowej linii, więc jest to osobna linia w *tym samym akapicie*.

(Uwaga techniczna: Markdown Here używa łamania wiersza GFM, więc nie ma potrzeby używania dwuspacji łamania wiersza MD.)


## Filmy na YouTube
Nie można ich dodać bezpośrednio, ale możesz dodać obraz z linkiem do filmu w ten sposób:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE
" target="_blank"><img src="http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

Lub w czystym Markdown, ale tracąc rozmiar obrazu i obramowanie:

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](http://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)

## Wzory matematyczne TeX
Pełny opis symboli matematycznych TeX wykracza poza zakres tej ściągawki. Oto dobre odniesienie i możesz wypróbować różne rzeczy na CodeCogs . Możesz także bawić się formułami na stronie opcji Markdown Here.

Oto kilka przykładów do wypróbowania:

$-b \pm \sqrt{b^2 - 4ac} \over 2a$
$x = a_0 + \frac{1}{a_1 + \frac{1}{a_2 + \frac{1}{a_3 + a_4}}}$
$\forall x \in X, \quad \exists y \leq \epsilon$

Początkowe i końcowe znaki dolara ( $) są ogranicznikami znaczników TeX.

https://www.michalbartyzel.pl/documentation-as-code/