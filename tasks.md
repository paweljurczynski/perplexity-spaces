# Apollo

- Stworzyłem mechanizm do automatycznego dodawania kolejnego języka do stron marketingowych. W tym momencie gdy chcemy dodać nowy język do strony wystarczy uruchomić skrypt który obecne tłumaczenia napisane dla języka angielskiego przetłumaczy na zadany język. Używa do tego modelu Grok i wykorzystuje sztuczną inteligencję do tworzenia odpowiednich tłumaczeń. Dzięki odpowiedniemu “system promptowi” nadaje odpowiedni kontekst zapytania do modelu.
- Zaproponowałem i wdrożyłem rozwiązanie które dla wszystkich dokumentów wyświetlanych w aplikacji używa plików zapisanych w formacie markdown, dzięki czemu mamy ujednolicone przechowywanie wszystkich dokumentów w aplikacji i nie potrzeba dodawać w kodzie customowego rozwiązania do tego samego problemu na wszystkich stronach.
