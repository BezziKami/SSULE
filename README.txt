Opis działania programu SSULE:

	Na początku zanim zacznie się wykonywać główna pętla na górze generujemy pierwsze części ciała węża,
na dole zaś zależnie od wybranej opcji inicjalizujemy działanie pada. Jeśli nie znajdzie żadnego mimo wybrania,
program użyje klawiatury.

	Najpierw sprawdzamy czy wąż zjadł jabłko lub czy nowo zespawnowane jabłko nie znajduje się w wężu, jeśli tak to
program generuje nowe jabłko i dodaje do listy z koordynatami węża kolejny rekord oraz zwiększamy ilość punktów o jeden.
	Następnie sprawdzamy kolizje ze ścianą i ogonem, jeśli ściany są włączone, następuje koniec gry, jeśli nie, wąż przechodzi
na drugą stronę. W przypadku zjedzenia ogona gra zawsze się kończy.
	Generujemy ogon węża w pętli while kolejno z rekordów w tabeli z koordynatami węża. Również rysujemy jabłko i głowe 
oraz tekstury krawędzi mapy. 
	Aby głowa obracała się w momencie zmiany kierunku musimy sprawdzić w którą stronę porusza się wąż, a następnie
obrócić tekstury węża tak, aby pasowały do kierunku poruszania się

	Pominięta obsługa klawiatury wyciąga pierwszy input z listy i nadaje jej konkretny kierunek x i y, następnie dla lepszej
responsywności została wykorzystana prosta kolejka, która przechowuje input gdyby program jeszcze nie zdążył się wykonać, 
na końcu jest jeszcze blokada przed złamaniem karku wężowi, na koniec kierunek zamieniamy na koordynaty, o które przesuniemy głowę węża.
