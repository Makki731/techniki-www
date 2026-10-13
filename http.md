CW.1

1. calc -> pozwala wykonywać obliczenia z podstawowymi funkcjami (abs, log, exp) 

2. ipaddr -> wyświetla adres IP oraz lokalizację

3 qr <text> -> generuje kod QR dla dowolnego tekstu

Wszystkie te funkcje mamy dziś w przeglądarce albo w aplikacjach: kalkulator jest w telefonie, adres IP sprawdzają różne strony, a kody QR generują strony i aplikacje.


CW.2

| żądanie | metoda | ścieżka | kod | 3 nagłówki + co znaczą |

 info.cern.ch | GET | / | 200 OK | `Content-Type: text/html` – serwer mówi, że wysyła stronę HTML; `Content-Length` – ile bajtów ma treść odpowiedzi; `Server: Apache` – jakim programem jest serwer |

| github.com | HEAD | / | 301 Moved Permanently | `Location: https://github.com/` – adres, pod który przeglądarka ma przejść; `Content-Length: 0` – odpowiedź nie ma treści, jest tylko przekierowanie; `Date` – kiedy serwer wysłał odpowiedź |

| nie-ma-takiej | HEAD | /nie-ma-takiej | 404 Not Found | `Content-Type: text/html` – zamiast strony dostajemy stronę z błędem; `Server: Apache` – ten sam serwer co wcześniej, tylko nie znalazł pliku; `Date` – czas odpowiedzi |


CW.3

| pomiar                | info.cern.ch      |    spacejam.com/1996      | onet.pl |
| liczba żądań          | 1                 | 17                        | 320 |
| przesłane dane (kB)   | 1                 | 81                        | 5669 |
| czas ładowania        | 0,5 s             | 1,7                       | 3,4 |
| elementy DOM          | 31                | 127                       | 3201               |

