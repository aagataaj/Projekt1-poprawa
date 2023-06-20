# Projekt1-poprawa

1. Zastosowanie programu

   Program jest przeznaczony głównie dla geodetów. Zadaniem Kalkuratora jest przeliczanie współrzędnych na różne sposoby.
   
   Program obsługuje elipsoidy: WGS 84 i GRS 80

   Program posiada następujące funkcje:

    hirvonen - Wykonuje transformacje XYZ na BLH.
    geodezyjne2XYZ - Jest odwrotnością Hirvonena.
    neu - Wykonuje transformacje z współrzędnych geodezyjnych do układu topocentrycznego NEU.
    u2000 - Wykonuje transformacje współrzędnych geodezyjnych do współrzędnych płaskich prostokątnych w układzie 2000.
    u1992 - Wykonuje transformacje współrzędnych geodezyjnych do współrzędnych płaskich prostokątnych w układzie 1992.
 
2. Wymagania systemowe i oprogramowania

      Program został napisany do pracy na komputerach lub laptopach posiadających system operacyjny Windows.
      Do uruchomienia programu potrzebne będzie środowisko python w wersji 3.8 lub nowszej.

      Dodatkowo potrzeba będzie posiadać zainstalowane następujące biblioteki: math, numpy, argparse
      
      Instalacja bibliotek na systemie windows wygląda następująco: Otwieramy folder, w którmy znajduje się nasz program. W pasku zawierającym ścieżkę               dostępu wpisujemy cmd i wciskamy enter. W odpalonej konsoli windowsa należy wpisać komendę: python -m pip install [options] zamiast options wpisać             nazwę biblioteki.

3. Instalacja i uruchomienie
   Aby poprawnie uruchomić program należy:
    umieścić pliki main.py i transformacje.py w jednym folderze.
    w pasku zawierającym ścieżkę dostępu wpisujemy cmd i wciskamy enter.
    w konsoli wpisać polecenie main.py
    Następnie należy podać ścieżki do pliku wejściowego i wyjściowego.

4. Opis działania programu
   Program składa się z czterech plików:

    kod-got-inf2.py - plik posiadający klasę i funkcje, które posłużą do robienia transformacji oraz wykonuje wszystkie niezbędne obliczenia
    wsp_inp.txt - jest to plik tekstowy zawierający współrzędne wejściowe w układzie geocentrycznym. Plik powinien składać się z dowolnej ilości wierszy          będących punktami (punkty powinny być ułożone następująco X,Y,Z, separatorem między nimi to ",", a znak oddzielający liczby całkowite od części               dziesiętnych to "."
    wsp_out.txt - jest to plik tekstowy, który już zawiera wyniki po wykonaniu kodu. W przypadku zmiany danych wejściowych plik nadpisze swoją zawartość dla      aktualnych współrzędnych

5. Problemy
   Plik wejściowy musi mieć tą samą nazwę i strukturę, aby mógł zostać użyty.
   Plik wejściowy musi znajdować się w tym samym folderze co głowny kod.
      
