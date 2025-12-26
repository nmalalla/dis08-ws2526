# Basic Formatting  
grundsätzlich ähnelt Markdown in Grundzügen der Formatierung mit HTML

### Stufe 3 Headings sehen z.B. so aus  
mit der Anzahl der # wird das Heading kleiner. Man darf das Leerzeichen nach # nicht vergessen.

### Paragraphs & line breaks  

durch zwei Leerstellen am Ende einer Zeile wird ein line break gesetzt. man kann aber auch mit dem html-break <br> arbeiten

### Bold, Italic und Strikethrough  
dafür gelten ähnliche Regeln wie bei HTML, 

mit ** oder __ an Anfang und Ende geht bold. * oder _ sind italic, Tilden ~~ machen ein Strikethrough. 

Also **dicker Text**, __schräger Text__, Text ~~mit Strich~~ und für *__ganz eindrucksvollen__* Text kann auch genested werden.  

### Inline code

Inline Code wird mit `backticks´ eingegrenzt. 

### Lists  
Unordered lists: Listen können mit -, * oder + je Item begonnen werden. Einfach an den Zeilenanfang setzen. Wie:  
Prüfungen dieses Semester: 
+ DIS08
+ DIS16
- DIS19
* DIS14
- DIS11
- DIS 13  

##### Ordered lists
Hier einfach mit einer Zahl beginnen. Wie Reihenfolge in der Woche:  
1. DIS11
2. DIS13
3. DIS19
4. DIS 14
es ist schön, dass automatisch die nächste Zahl/Zeichen ergänzt wird!

##### Nested lists  
Wenn man nach jedem Zeichen um mehrere Leerstelle einrückt, erhält man eine nested list. so:  
1. DIS11
   2. DIS13 - 3 Leerzeichen Einrückung
      3. DIS19 - 6 Leerzeichen Einrückung
         4. DIS 14 - 9 Leerzeichen Einrückung

### Links & Images
##### Inline links
in Doppelklammern "[(" kann man URLs einsetzen. So: [Wikipedia zufälliger Artikel](https://en.wikipedia.org/wiki/Special:Random)]

##### Reference-style links
Hier ist ein [Beispiel][1] für einen Referenzlink.  
[1]: https://en.wikipedia.org/wiki/Reference "Referenzen"
##### Images
![Alt-Text](https://en.wikipedia.org/wiki/Reference#/media/File:Ogden_semiotic_triangle.png "Titel")
### Code & Technical Content
##### Inline code
mit backticks den Code einrahmen. single tick = inline
`def test():
    print("Markdowntest")`
##### Fenced code blocks
um in eine eigene zeile zu rücken wie:
```
def test():
    print("Markdowntest")
``` 
ist es wichtig, dass die ticks in eigenen zeilen stehen

##### Syntax highlighting

nach den backticks die sprache nennen

```python
def test():
    print("Markdowntest")
```

### Quotes & Notes
##### Blockquotes
>Blockzitate mit einem größer-als vorher
>nächste Zeile
##### Nested blockquotes
>Blockzitate mit einem größer-als vorher
>>Zitat-im-Zitat
>nächste Zeile
##### Blockquotes with formatting
>Blockzitate mit einem größer-als vorher
>>Zitat-im-Zitat
>>**man kann auch formatieren**
>nächste Zeile
### Tables
werden mit Pipes formatiert und Bindestrichen unter dem Header
##### Basic tables
| Lab | Kalenderwoche |Thema    |
|-|-|-|
|1| 41 | open software and hosting   |
|2| 42 | open data     |
|3| 43 | command line interface|
##### Alignment
mit : kann man die Bündigkeit des Tetxts ändern
| Lab | Kalenderwoche |Thema    |
|:-|:-:|-:|
|1| 41 | open software and hosting   |
|2| 42 | open data     |
|3| 43 | command line interface|
##### Complex tables
man kann natürlich auch innerhalb des tables formatieren 
mit : kann man die Bündigkeit des Tetxts ändern
|_Lab_ | _Kalenderwoche_ |_Thema_|
|:-|:-:|-:|
|1| 41 | open software and hosting   |
|2| 42 | open data     |
|3| 43 | command line interface|
##### Task Lists
formatieren wie:
- [x] Fertig  
- [ ] Offen
##### Checkboxes
kann man natürlich auch in Tabellen integrieren:
|_Lab_ | _Kalenderwoche_ |_Thema_|_erledigt?_
|:-|:-:|-:|:-:|
|1| 41 | open software and hosting   |[x]
|2| 42 | open data     |[x]
|3| 43 | command line interface|[ ]
### Dividers & Layout
##### Horizontal rules
kann man mit drei oder mehr Zeichen hintereinander erzeugen:
---
***
___
sehen aber alle gleich aus
##### Line breaks 
siehe oben, mehr als zwei leerzeichen+Absatz  
hintereinander
### Online and collaborative editors
##### Markdown-based editors
es gibt noch andere editoren wie zB Joplin, Obsidian oder Typora. Diese haben den Vorteil, dass sie in Echtzeit die Ausgabe der .md Datei zeigen
### Platform/Tool Specific: GitHub
##### Task lists
Es ist sehr umgebungsabhängig, ob eine Taskliste interkativ gerendert wird. Spezifisch in GitHub sind diese zum Beispiel interaktiv renderbar in Issues, PRs, Project Boards oder Wikis. Nicht anklickbar sind sie in README.md und anderen .md Dateien im repo.
##### Mentioning users (@username)
man  kann user mit @ und dem usernamen aufrufen, zB @nmalalla
##### Automatic linking of issues/PRs
issues oder PRs werden nummeriert, diese kann man mit #Nummer aufrufen, zB  
siehe Issue #1
##### Emoji shortcodes
Der Code :heart: rendert ein  Herzchen, genauso mit allen anderen emojinamen