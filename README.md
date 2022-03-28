# PVA2 - Programování a vývoj aplikací
## Cvičení 13: OOP část 2

### 1
Uvažuj, že navrhuješ software pro zásilkovou společnost.

Vytvoř třídu Balik, která bude mít tři atributy - adresa, hmotnost a stav doručení. První dva atributy nastav pomocí parametrů funkce `__init__`. Parametr doruceno nastav na začátku jako False.
Připoj ke třídě funkci deliver, která změní hodnotu parametru doruceno na True.
Přidej metodu `__str__`, která vypíše adresu, hmotnost a informaci o tom, zda byl balík již doručen.
Zkus si vytvořit nějaké objekty ze třídy Balik a ověř, že vše funguje.

### 2
Nově bubdeme doručovat i cenné balíky, které mají zadanou určitou hodnotu.

Vytvoř třídu CennyBalik, která dědí od třídy Balik. CennyBalik má navíc atribut hodnota, ostatní atributy dědí od třídy Balik.
Atribut hodnota nastav pomocí funkce `__init__`. Ostatní parametry předej funkci `__init__` třídy Balik.
Vytvoř si alespoň jeden objekt a zkus volání jeho funkcí.

### 3
Společnost nyní eviduje jednotlivé řidiče a eviduje balíky, které má každý řidič doručit.

* Vytvoř třídu Ridic, která má dva atributy: jmeno (jméno řidiče) a seznam_baliku (seznam balíků k doručení, na začátku je prázdný).
* Přidej třídě metodu prirad_balik, která bude mít jeden parametr - balik (balík k doručení, může se jednat i o cenný balík). Funkce nejprve zkontroluje, zda balík již nebyl doručen. Pokud ano, vypíše funkce text: "Nelze přiřadit, balík již byl doručen." Pokud balík ještě nebyl doručen, je přidán do seznamu balíků seznam_baliku (použij funkci append).
* U řidiče chceme sledovat, kolik by měl ještě doručit balíků. Napiš funkci zbyva_baliku, která vrátí počet balíků, které má řidič přiřazené a ještě je nedoručil.
