# Les principes FIRST : Répétable (Reproducible)

Le troisième principe **FIRST** est celui de la _reproductibilité_ des tests. Cela signifie que les tests doivent être répétables et produire des résultats déterministes. En d'autres termes, un test donné doit donner les mêmes résultats chaque fois qu'il est exécuté avec les mêmes données d'entrée. Un test non répétable peut entraîner un comportement instable, où le résultat fluctue entre le succès et l'échec. 🔄

Lorsqu'un test est non répétable, il peut afficher un comportement de "_flickering_", c'est-à-dire qu'il passe du statut réussi au statut échoué, puis à nouveau au statut réussi. Parfois, il peut être réussi neuf fois sur dix, puis échouer une fois. Lorsque vous rencontrez de tels cas, il est important de reconnaître qu'il s'agit de tests non déterministes et de faire des efforts pour éliminer ce comportement instable. ❌

Le non-déterminisme peut être causé par divers facteurs. Par exemple, il peut être lié au temps, à l'utilisation de données aléatoires ou à des dépendances externes qui ne sont pas disponibles ou qui ont des résultats inattendus. Pour rendre les tests répétables, il est recommandé de mettre en place des conditions reproductibles en établissant chaque test avec ses propres données et en organisant son environnement. 📈

Il est possible d'utiliser des données aléatoires dans les tests, mais elles ne doivent pas influencer le résultat du test. Par exemple, si un champ de nom n'est pas utilisé dans le scénario de test, il peut être alimenté avec des données aléatoires, car cela n'aura pas d'impact sur le résultat du test. L'utilisation de données aléatoires peut même aider à découvrir des problèmes potentiels. Cependant, il est crucial de s'assurer que le résultat du test ne dépend pas de ces données aléatoires. 🎲

Lorsqu'un test échoue, il est essentiel de prendre cela au sérieux et de ne pas simplement le réexécuter et le voir passer au vert sans aucun changement. La fiabilité des tests repose sur leur capacité à être répétables, ce qui signifie que nous devons pouvoir leur faire confiance. 🛠️

Le principe de reproductibilité est lié au principe d'isolation et d'indépendance, car en rendant les tests isolés et indépendants, on favorise également leur reproductibilité. Cependant, il existe un compromis entre la reproductibilité et la vitesse des tests. Les tests d'intégration de base de données ou les tests de bout en bout peuvent être sujets à des problèmes de scintillement en raison de la synchronisation ou des modifications de données dans la base de données. Dans ces cas, il est possible de mettre en place des stratégies, comme l'utilisation de transactions ou la création et la suppression de bases de données pour chaque test, afin de rendre les tests plus reproductibles, même si cela peut ralentir leur exécution. ⏱️

En conclusion, la reproductibilité des tests est essentielle pour pouvoir leur faire confiance et obtenir des retours d'information fiables. Il est important de mettre en place des conditions reproductibles, d'éliminer les comportements non déterministes et d'optimiser la vitesse des tests tout en maintenant leur reproductibilité. 🔄

Restez à l'écoute pour le prochain principe **FIRST** : **Self validating (auto-validation)**. 👂
