# Les principes FIRST : Rapides (Fast)

Le premier principe **FIRST** est la rapidité des tests. ⚡️ Il est essentiel que les tests soient aussi rapides que possible. En effet, plus les tests
sont rapides, mieux c'est. Des tests rapides sont exécutés plus fréquemment, ce qui nous permet d'obtenir des retours plus fréquents sur notre travail. Lorsque nous mesurons la vitesse ou la durée d'un test, nous incluons à la fois la configuration initiale (_setup_) et le nettoyage (_teardown_), c'est-à-dire l'ensemble du cycle du test.

Cela signifie que les tests qui dépendent d'éléments externes tels que des bases de données ont souvent du mal à respecter ce principe et devraient être réduits au minimum pour cette raison. Mais pourquoi est-il important d'avoir plus de retours et en quoi cela nous aide-t-il ? Pour illustrer cela, prenons l'exemple d'un disjoncteur électrique dans un circuit électrique domestique. Imaginons que ce disjoncteur ne vérifie la surcharge que toutes les heures. ⚡️

Pendant 59 minutes, le circuit pourrait être surchargé sans que nous en soyons conscients, ce qui pourrait potentiellement causer des dommages plus importants. La rapidité de détection et de réaction du disjoncteur, qui se déclenche presque immédiatement en cas de surcharge, contribue grandement à la sécurité du système. Il en va de même pour les retours rapides que nous obtenons grâce aux tests. 💡

Plus les tests sont rapides, plus ils sont exécutés fréquemment, et plus nous recevons rapidement des informations sur notre code. Cela réduit les risques d'erreurs passant inaperçues et causant ainsi de plus gros problèmes. Il existe plusieurs mesures que vous pouvez prendre pour respecter ce principe ou l'appliquer. 🏃‍♀️

* Tout d'abord, la plupart de vos tests devraient être de petite taille et s'exécuter rapidement. Lorsque vous dépassez le stade des tests unitaires et que vous effectuez des tests plus larges, cela peut devenir plus difficile à réaliser. Cependant, nous vous recommandons d'écrire des tests de petite taille qui se concentrent sur des parties spécifiques du système. Plus les tests sont petits, plus ils sont rapides.

* Ensuite, surveillez la vitesse de vos tests et cherchez toujours des moyens de les améliorer. Vous pouvez prendre des mesures pour accélérer leur exécution, mais veillez à ce qu'ils restent toujours rapides. Il serait contre-productif que les développeurs ne les exécutent pas simplement parce qu'ils prennent trop de temps. Assurez-vous que vos tests s'exécutent rapidement et efficacement.

* Enfin, vous pouvez séparer les tests plus lents des tests plus rapides en les regroupant dans des suites de tests distinctes et en les exécutant à des moments différents. Vous pouvez exécuter les tests rapides pendant que vous développez, à intervalles réguliers, tandis que les tests plus lents ne sont exécutés qu'avant une validation ou lors de constructions nocturnes, par exemple. Ajustez la fréquence d'exécution des différents tests selon vos besoins.

Rappelez-vous également que ce principe est un guide plutôt qu'une règle stricte. Si vous tirez plus d'avantages d'un test plus lent que vous ne le feriez en le rendant plus rapide, par exemple pour éliminer des dépendances externes, vous pouvez continuer à le faire. Cependant, veillez à limiter le nombre de ces tests plus lents, car la rapidité reste un objectif important. 🚀

Dans la prochaine partie, nous aborderons le deuxième principe **FIRST** : **Isolated/Independent (isolés/indépendants)**.

Je vous donne rendez-vous dans la prochaine partie, à tout de suite. 📚
