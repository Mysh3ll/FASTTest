# Les principes FIRST : Indépendants/Isolés (Independent/Isolated)

Le deuxième principe **FIRST** est celui de _l'indépendance_ ou de _l'isolement des tests_. L'objectif est de s'assurer que les tests ne sont pas
affectés par des facteurs externes. Autrement dit, un test ne doit pas dépendre d'un élément externe qui doit être configuré de manière spécifique pour que le test fonctionne. Certains exemples courants d'éléments externes incluent les données d'une base de données ou l'exécution à une heure précise. L'idée est de pouvoir exécuter les tests à tout moment et n'importe où. 🌍

Les tests doivent être indépendants et isolés les uns des autres. Ils ne doivent pas s'influencer mutuellement, de sorte que le résultat d'un test ne doit pas affecter l'exécution d'un autre test. Cela signifie qu'il ne doit pas y avoir d'état partagé entre les tests. De plus, les tests doivent être isolés ou indépendants de l'environnement externe, comme mentionné précédemment, par exemple les bases de données, le temps ou les variables d'environnement. 💪

Pour atteindre cet objectif, il est recommandé d'utiliser le modèle **A**rrange-**A**ct-**A**ssert. Dans ce modèle, la partie _"Arrange"_ configure l'environnement pour le test, la partie _"Act"_ invoque la méthode ou la fonction testée, et la partie _"Assert"_ vérifie une condition logique. Une fois l'instruction _"Assert"_ terminée, il ne devrait plus y avoir d'actions affectant l'environnement, ce qui contribue à maintenir le test autonome. 🧪

Il est important de ne pas utiliser d'état partagé entre les tests. Utilisez plutôt des fixtures transitoires, qui sont des données et des objets nécessaires pour exécuter un test. Les fixtures transitoires doivent être jetées une fois le test terminé. Cela garantit que les tests ne dépendent pas les uns des autres. Si une fixture est partagée entre les tests et qu'un test la modifie, un autre test ne sera pas isolé de celui-ci. La dépendance entre les tests crée un couplage temporel, ce qui peut être difficile à gérer, notamment lorsque les tests sont exécutés dans différents ordres. 🔒

Il peut être tentant de placer des états partagés dans les blocs de description (_describe_) pour s'assurer que les tests sont rapides. Cependant, cela peut entraîner une confusion, car l'état partagé peut s'éloigner du code qui l'utilise lorsque de nouveaux tests sont ajoutés. Pour éviter cela, il est recommandé de contenir chaque test dans une seule méthode, en utilisant des méthodes d'aide ou des méthodes/fonctions de construction si nécessaire. 🚧

Assurez-vous également qu'il n'y a pas de dépendances de séquence entre les tests. L'ordre dans lequel les tests sont exécutés ne devrait pas avoir d'importance. Lorsque vous écrivez un test, supposez que ce test est la seule chose qui s'exécute dans tout le programme. Chaque test est son propre programme, commençant et se terminant comme s'il était exécuté depuis la ligne de commande. 🔄

Il est vrai que cela peut rendre les tests un peu plus lents, mais le principe d'indépendance l'emporte généralement sur celui de la vitesse, à moins que des problèmes de performance sérieux n'empêchent l'exécution des tests. Si l'indépendance n'est pas correctement optimisée, la suite de tests devient difficile à utiliser. 🐢

Dans la prochaine partie, nous aborderons le troisième principe **FIRST** : **Reproducible (Reproductible)**. 🔄

Je vous donne rendez-vous dans la prochaine partie, à tout de suite. 👋
