# Zdobywanie podstawowych informacji o systemie decyzyjnym

1. Tworzymy **publiczne** repozytorium w platformie [GitHub](https://github.com/)
   - Repository name: `uwm-ssi`,
   - Description: `Numer indeksu: {numer_indeksu}`,
   - Zaznaczamy `Initialize this repository with a README`,
   - Add .gitignore: `Python`.
   - Add a license: `MIT`.
2. Klonujemy repozytorium do następującej lokacji:
   - `D:/SSI/{numer_indeksu}/`
   - W tym folderze będą przechowywane wszystkie zadania studenta.
3. Wybieramy jeden z systemów decyzyjnych dostępnych w katalogu `data` tego ćwiczenia.
   - W pliku `_info-data-discrete.txt` mamy opis poszczególnych systemów w formacie:
      ```
      nazwa_systemu liczba_atrybutów liczba_obiektów
      ```
   - W pliku `{*}-type.txt` mamy informacje o typie atrybutów:
      ```
      n - atrybut numeryczny
      s - atrybut symboliczny
      ```
      Pamiętamy o ograniczeniach dla atrybutów symbolicznych.
4. Tworzymy nowy plik `c01.py` a następnie wczytujemy z pliku wybrany system.
5. Dla wybranego systemu decyzyjnego zdobywamy następujące informacje i wypisujemy:
   - istniejące klasy decyzyjne
   - wielkość klas decyzyjnych (liczba obiektów w klasach),
   - minimalne i maksymalne wartości poszczególnych atrybutów numerycznych
   - dla każdego atrybutu wypisujemy liczbę różnych dostępnych wartości,
   - dla każdego atrybutu wypisujemy listę różnych dostępnych wartości,
   - odchylenie standardowe dla poszczególnych atrybutów numerycznych w całym systemie i klasach decyzyjnych.
6. Po wykonaniu zadania `push` do repozytorium.

##### DODATKOWO

1. Stworzyć klasę `SystemDecyzyjny`, która obsługuje powyższe zadania w formie obiektowej np.
   - Plik systemy przekazywany w konstruktorze,
   - Zadania z podpunktu 5 rozbite na funkcje.
2. Za pomocą wybranej właściwości języka `Python`, wczytać wszystkie pliki i wywołać funkcje z klasy `SystemDecyzyjny`.
3. Zapoznać się z biblioteką [pandas](https://pandas.pydata.org/) i jej możliwościami. Następnie proszę użyć wbudowanych w nią funkcji do uproszczenia zadania.