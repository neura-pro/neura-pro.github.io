### Tezos to platforma smart-kontraktowa z formalnie weryfikowalnym językiem programowania i ze zintegrowanym systemem samorządności. 

Najlepiej zacząć od [krótkiej prezentacji promocyjnej Tezosa](https://www.youtube.com/watch?v=7m7EU4JWI88).

Tezos jest niezależny od innych blockchainów, a jego kod źródłowy zbudowany jest od zera. Do tworzenia kontraktów wymagane jest użycie specjalnego języka skryptowego (odpowiednik języka *Solidity* na ETH).

Czym się Tezos chce wyróżnić? Mamy trzy główne aspekty:
- Sformalizowany system samorządności
- Sformalizowany system weryfikacji smart-kontraktów
- Modułowa architektura

### Sformalizowany system samorządności

> Unlike other smart contract platforms, Tezos has a formal governance mechanism on the blockchain itself.

Rzeczywiście, sprawa sprawności podejmowania decyzji (tzw. *governance issue*) jest mocno zaniedbana w świecie blockchainowym, choć jest ona krytycznie ważna. Chodzi tu o dwojakiego typu sytuacje:
- decyzje strategiczne (np. istotna zmian protokołu, np. słynna kwestia wielkości bloku w BTC, albo zapowiadane przejście z POW do POS w przypadku ETH)
- obsługa nietypowych wydarzeń (np. słynne fiasko *The DAO* na ETH).

Moja subiektywna opinia:  w tej chwili jedynie blockchainy oparte na DPOS (Delegated Proof of Stake, czyli BitShares, Steem, EOS, PeerPlays) mają powyższą kwestię rozwiązaną - na pewno nie idealnie, ale przynajmnej instnieją stosowne mechanizmy na poziomie blockchaina. Można też przyjąć, że blockchainy, w których jest jakaś hierarchia ważności *node*'ów, (tj. mają warstwę tzw. *master nodes*, np. Dash), również w jakimś stopniu są w stanie w miarę skutecznie działać w zakresie podejmowania decyzji.

Natomiast wszystkie pozostałe blockchainy są niebezpiecznie bezbronne w aspekcie *governance issue* i zapewne prędzej czy później poniosą negatywne konsekwencje tego faktu. Albo będą tkwiły w decyzyjnej stagnacji.

Wracając do Tezosa - to zatem duży atut, że troska o *governance issue* leży u samych podstaw tej technologii.

> We enable token holders to make decisions about how the protocol should evolve. All decisions are made transparently on the blockchain. (...) It can even change the rules for decision-making.

Czyli nawet będą reguły pozwalające zmienić reguły tworzenia reguł. To jest analogiczne do artykułu w konstytucji o trybie, w jakim mogą być dokonane zmiany w konstytucji. Duży plus.

### Sformalizowany system weryfikacji smart-kontraktów

> Formal verification has been used in the aerospace industry, in medical devices, and other instances where the stakes are too high to fail. It can ensure the security of the platform by proving the correctness of its code.

To jest mega ważna sprawa. Bo to pozwala w dużym stopniu mieć pewność, że smart-kontrakt nie zachowa się wbrew intencjom jego twórców. Czyli np. *The DAO* prawdopodobnie nie przeszłoby takiej weryfikacji, więc nie doszłoby do katastrofy, jaka miała miejsce na ETH.

> To mitigate that risk, the development team designed our smart contract language with correctness and formal verification in mind.

No i tu mamy cenę za tę podwyższoną odporność na błędy - Tezos wprowadza swój własny język skryptowy (o nazwie *Michelson*), co powoduje że pojawia się dodatkowa bariera dla developerów. 

> Tezos is written in OCaml, a statically-typed functional programming language.

Ważne rozróżnienie: platforma Tezos jest napisana w języku [OCaml](https://en.wikipedia.org/wiki/OCaml), który jest bardzo solidny, ale trudny w użyciu i mało znany. Nie należy mylić tego z językiem skryptowym *Michelson*, który ma służyć do pisania smart-kontraktów na Tezosie.

Istotna sprawa: Tezos nie daje 100% gwarancji wykrycia błędu w kodzie smart-kontraktu, daje jedynie zestaw narzędzi, które w sposób istotny zmniejszają możliwość powstania takiego błędu. Projektem, który ma ambicję osiągnąć 100% takiej gwarancji, jest [TauChain/Agoras](http://www.idni.org/), ale póki co nie wiadomo czy to się uda.

### Modułowa architektura

> Because Tezos starts with a unique modular design, with cleanly separated layers, upgrading the protocol is as simple as changing out one layer for another.

Bez zaglądania do kodu źródłowego trudno zweryfikować, na ile jest to prawdziwe stwierdzenie. Niemniej wiadomo, że architektura modułowa jest czymś pożądanym, bo umożliwia liczne modyfikacje działania systemu (czyli mamy wysoką elastyczność) i otwiera go na dalszy rozwój.

> There is no need need for hard forks.

To jest ciekawa rzecz. Na razie nie mam pojęcia, jakim cudem Tezos będzie w stanie unikąć hard forków. Być może chodzi o to, że hard forki będą, tyle że nigdy nie będzie niebezpieczeństwa splitu (jak np. miało to miejsce w przypadku ETH i ETC).

### Podsumowując
Tezos idzie w stronę obsługi smart-kontraktów, które wymagają największego stopnia bezpieczeństwa. Nie idzie więc w masowość i efektywność procesowania, w zamian stawia na jakość. Czyli pozycjonuje się jako najwyższa półka wśród platform smart-kontraktowych. Na drugim biegunie jest Lisk - ten nie przejmuje się zbytnio bezpieczeństwem i stawia na masowo znany z zastosowań webowych java-script.

Tezos ma jeden duży minus: tworzenie nietrywialnych smart-kontraktów jest samo w sobie piekielnie trudne, a Tezos dodatkowo istotnie zwiększa tę trudność. No ale z drugiej strony można spekulować, że ludzie, którzy są w stanie tworzyć smart-kontrakty, prawdopodobnie są też w stanie posługiwać się trudniejszymi językami programowania.

### Kim są ludzie którzy za tym stoją?

Zlokalizowani we Francji, co jest dość nietypowe. Na pierwszy rzut oka [zespól nie wygląda imponująco](https://www.tezos.com/team). Moim zdaniem wyraźnie brakuje tu dużego kalibru developera, a CEO Arthur Breitman jest dość niedoświadczony w zakresie technologii blockchainowych:

> Arthur Breitman had worked at the high frequency trading desk at Goldman Sachs and was an options market maker at Morgan Stanley, while Kathleen Breitman is a former management associate at Bridgewater Associates, the world's largest hedge fund.

Obszerny wywiad Breitmana dla [Epicenter Bitcoin](https://www.youtube.com/watch?v=3mgaDpuMSc0) też nie zrobił na mnie wrażenia. Breitman mówi słuszne rzeczy, ale brakuje w tym większego insight'u.

[Whitepaper]([https://www.tezos.com/static/papers/white_paper.pdf) jest raczej pobieżny, ledwo 17 stron. W porównaniu z whitepaperem Ethereum lub EOSa wygląda dość niepoważnie.

### Parametry blockchaina

Mechanizm konsensusu to DPOS (Delegated Proof of Stake), czyli będzie to wzorowane na koncepcji twórcy EOS'a Dana Larimera.

Nie znalazłem informacji o docelowej inflacji ani informacji w zakresie opłat transakcyjnych (w tym opłat za procesowanie smart-kontraktów) - całkiem dziwne, bo to są dość istotne sprawy.

### Dodatkowe informacje

[Tezos - oficjalna strona webowa](https://www.tezos.com/)

[Tezos Roadmap](https://www.tezos.com/static/papers/Tezos_Overview.pdf)

[Billionaire investor Draper to participate in blockchain token sale for first time](http://www.reuters.com/article/us-tezos-blockchain-draper-idUSKBN181250)
