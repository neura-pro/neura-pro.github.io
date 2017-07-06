W jednym zdaniu: Tezos to platforma smart-kontraktowa z formalnie weryfikowalnym językiem programowania i ze zintegrowanym systemem samorządności.

Najlepiej zacząć od krótkiej prezentacji promocyjnej Tezosa:
https://www.youtube.com/watch?v=7m7EU4JWI88

A teraz po kolei najważniejsze kwestie tam poruszone.

> Tezos is an all new smart contract platform built from scratch.

Czyli mamy kolejną, niezależną od innych blockchainów, platformę do procesowania smart-kontraktów. Pozostałe to: [Ethereum](https://www.ethereum.org/), [EOS](https://eos.io/), [Lisk](https://lisk.io/), [TauChain/Agoras](http://www.idni.org/), [Stratis](http://stratisplatform.com/), [Rootstock](http://www.rsk.co/) i [Emercoin](https://emercoin.com/).

Czym się Tezos chce wyróżnić? Są trzy główne sprawy:
- Formal governance mechanism
- Modular design
- Formal verification of smart-contracts

#### Formal governance mechanism

> Unlike other smart contract platforms, Tezos has a formal governance mechanism on the blockchain itself.

Rzeczywiście, sprawa sprawności podejmowania decyzji (tzw. governance issue) jest mocno zaniedbana w świecie blockchainowym, choć jest ona krytycznie ważna. Chodzi tu o dwa zakresy: 
- decyzje strategiczne (np. istotna zmian protokołu, np. słynna kwestia wielkości bloku w BTC, albo zapowiadane przejście z POW do POS w przypadku ETH)
- obsługa nietypowych sytaucji (np. słynne fiasko *The DAO* na ETH).


Moja subikektywna opinia:  w tej chwili jedynie blockchainy oparte na DPOS [Delegated Proof of Stake] (czyli BitShares, Steem, EOS, PeerPlays) mają tę kwestię w pewnym stopniu rozwiązaną. Można też przyjąć, że blockchainy, w których jest jakaś hierarchia ważności node'ów, (tj. mają warstwę tzw. *master nodes*, np. Dash), również w jakimś stopniu są w stanie skutecznie podejmować decyzje.

Natomiast wszystkie pozostałe blockchainy są niebezpiecznie bezbronne w zakresie *governance issue* i zapewne prędzej czy później poniosą negatywne konsekwencje tego faktu.

Wracając do Tezosa - to zatem duży atut, że troska o *governance issue* leży u samych podstaw tej technologii.

> We enable token holders to make decisions about how the protocol should evolve. All decisions are made transparently on the blockchain. (...) It can even change the rules for decision-making.

Czyli nawet będą reguły pozwalające zmienić reguły tworzenia reguł. To jest analogiczne do artykułu w konstytucji o trybie, w jakim mogą być dokonane zmiany w konstytucji.

#### Modular design

> Because Tezos starts with a unique modular design, with cleanly separated layers, upgrading the protocol is as simple as changing out one layer for another.

Bez zaglądania do kodu źródłowego trudno zweryfikować na ile jest to prawdziwe. Niemniej wiadomo, że architektura modułowa jest czymś pożądanym, bo umożliwia liczne modyfikacje działania systemu (czyli mamy wysoką elastyczność) i otwiera go na dalszy rozwój.

> There is no need need for hard forks.

To jest ciekawa rzecz. Na razie nie mam pojęcia, jakim cudem będą w stanie uniknąć hard forków. Być może chodzi o to, że hard forki będą tyle, że nigdy nie będzie niebezpieczeństwa że nastąpi split (jak np. miało to miejsce w przypadku ETH i ETC).

#### Formal verification of smart-contracts

> Formal verification can ensure the security of the platform by proving the correctness of its code.

To jest mega ważna sprawa. Bo to pozwala w dużym stopniu mieć pewność, że smart-kontrakt nie zachowa się wbrew intencjom jego twórców. Czyli *The DAO* prawdopodobnie nie przeszłoby takiej weryfikacji i nie zostałoby wpuszczone na Tezosa.

> Tezos is written in OCaml, a statically-typed functional programming language.

No i tu mamy cenę za tę podwyższoną odporność na błędy. Języki programowania typu OCaml, są bardzo skomplikowane, więc są trudne w użyciu i nie tak powszechne jak inne (np. Java czy C++).

I druga istotna sprawa: nie mamy tu 100% gwarancji wykrycia błędu w kodzie, jedynie zestaw narzędzi, które czynią to mało prawdopodobnym. Projektem, który ma ambicję osiągnąć 100% takiej gwarancji, jest   [TauChain/Agoras](http://www.idni.org/), ale póki co nie wiadomo czy to się uda.

#### Podsumowując
Tezos idzie w stronę obsługi smart-kontraktów, które wymagają największego stopnia bezpieczeństwa. Nie idzie więc w masowość i efektywność procesowania, w zamian stawia na jakość. Czyli taka najwyższa półka wśród platform smart-kontraktowych. Na drugim biegunie jest Lisk - ten używa masowo znanego java-scriptu.

Tezos ma jeden duży minus: tworzenie nietrywialnych smart-kontraktów jest samo w sobie piekielnie trudne, a Tezos dodatkowo istotnie zwiększa tę trudność. No ale z drugiej strony można spekulować, że ludzie, którzy są w stanie tworzyć smart-kontrakty, prawdopodobnie są też w stanie posługiwać się trudniejszymi językami programowania.
