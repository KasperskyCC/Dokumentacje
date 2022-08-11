#Prezentacja

## Stosowanie
Stosowanie
Funkcje marp zostaną włączone, gdy "marp: true" zostanie napisane na początku dokumentu Markdown.

'''
---
marp: true
---

# Your slide deck

Start writing!
'''

## [Jak pisać slajdy?](https://marpit.marp.app/markdown?id=how-to-write-slides)
Marpit dzieli strony zjeżdżalni za pomocą poziomej linijki (np "---". ). To jest bardzo proste.

'''
# Slide 1

foo

---

# Slide 2

bar
'''


## [Na liście punktowanej](https://marpit.marp.app/fragmented-list?id=for-bullet-list)
CommonMark dopuszcza "-", "+", i "*"jako znak [znacznika listy](https://spec.commonmark.org/0.29/#bullet-list-marker) punktowanej . Marpit przeanalizowałby jako pofragmentowaną listę, jeśli używasz "*"jako znacznika.

'''
# Bullet list

- One
- Two
- Three

---

# Fragmented list

* One
* Two
* Three
'''


## [Dla uporządkowanej listy](https://marpit.marp.app/fragmented-list?id=for-ordered-list)
[Znacznik uporządkowanej listy](https://spec.commonmark.org/0.29/#ordered-list-marker) CommonMark musi zawierać cyfry "."lub po nich. ")"Marpit przeanalizowałby jako pofragmentowaną listę, jeśli używasz )jako następującego znaku.

'''
# Ordered list

1. One
2. Two
3. Three

---

# Fragmented list

1) One
2) Two
3) Three
'''


## [Dyrektywy](https://marpit.marp.app/directives)
Marpit Markdown rozszerzył składnię o nazwie **„Dyrektywy”** , aby wspierać pisanie niesamowitych slajdów. Może kontrolować motyw slajdów, numer strony, nagłówek, stopkę, styl i tak dalej.


## [Składnia obrazu](https://marpit.marp.app/image-syntax)
Marpit rozszerzył składnię obrazu Markdown "![](image.jpg)", aby była pomocna w tworzeniu pięknych slajdów.