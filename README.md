Potoki

2.
Koraystając z polecenia "cat" utwórz plik "tekst3.txt", który będzie składał się z zawartości
pliku "tekst1.txt", ciągu znaków podanego ze standardowego wejścia (klawiatury) i pliku
"tekst2.txt".

'''c 
touch tekst1.txt
touch tekst2.txt

cat tekst1.txt tekst2.txt > tekst3.txt'''

7.
Za pomocą filtru "tr" wykonaj modyfikację pliku "plik.txt", polegającą na umieszczeniu
każdego słowa w osobnej linii.

touch plik.txt
tr -cs [a-zA-Z0-9] [\n*] > plik.txt

9.
Napisać polecenie zliczające sumę znaków z pierwszych trzech linii pliku "/etc/passwd"

kina@Kina-Linux:~/etc$ cat passwd | head -n 3 | wc -c


4.
Wyświetl linie o numerach 3, 4 i 5 z pliku "/etc/passwd"

cat passwd | head -n 5 | tail -n 3

5.
Wyświetl linie o numerach 7, 6 i 5 od końca pliku "/etc/passwd".

kina@Kina-Linux:~/etc$ cat passwd | tail -n 7 | head -n 3

6.
Wyświetl zawartość pliku "/etc/passwd" w jednej linii.
kina@Kina-Linux:~/etc$ cat passwd | tr -d "\n"


