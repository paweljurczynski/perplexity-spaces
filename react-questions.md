### Dlaczego warto pisać controlled components zamiast uncontrolled w React?
Controlled components pozwalają na pełną kontrolę nad stanem komponentu, co ułatwia synchronizację danych z widokiem i zarządzanie formularzami. Dzięki temu można łatwo implementować walidację oraz precyzyjnie sterować zachowaniem komponentów. Uncontrolled components są prostsze, ale mniej przewidywalne i trudniejsze do zarządzania w większych aplikacjach.

### W jakich sytuacjach powinno się używać hooka useEffect w React i dlaczego jest on potrzebny?
useEffect służy do obsługi efektów ubocznych w komponentach funkcyjnych, takich jak pobieranie danych z API, subskrypcje czy ręczna manipulacja DOM. Pozwala uruchamiać kod po wyrenderowaniu komponentu i reagować na zmiany wybranych zależności, dzięki czemu logika „po renderze” jest zebrana w jednym, czytelnym miejscu. Dodatkowo umożliwia sprzątanie po efektach (np. odpinanie timerów, event listenerów), co zapobiega wyciekom pamięci i niepożądanemu zachowaniu aplikacji.

### Jak są liczone zależności w tablicy zależności
Zależności w tablicy useEffect są obliczane przez React na podstawie porównania ich referencji z poprzednim renderem. React wykonuje płytkie porównanie (shallow comparison), czyli sprawdza, czy referencje w tablicy zależności się zmieniły, nie porównując głęboko zawartości obiektów. Jeśli którakolwiek z tych wartości się zmieniła, efekt zostanie ponownie uruchomiony; jeśli tablica jest pusta, efekt uruchamia się tylko raz po pierwszym renderze.​
