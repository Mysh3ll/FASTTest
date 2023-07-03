# Les principes FIRST : Résumé

Résumons les **cinq** principes **FIRST** et rappelons-les : les tests doivent être **rapides**, **isolés**, **indépendants**, **reproductibles** et **exhaustifs**. 💡

En suivant ces principes, nous constatons que nos tests sont de meilleure qualité et gagnent en fiabilité. Lorsque nous avons confiance en nos tests, nous pouvons les utiliser davantage. Nous les exécutons plus fréquemment et accordons plus d'importance à leurs résultats, car nous avons confiance en eux. Si un test signale un dysfonctionnement, nous le croyons. 🚀

Nous verrons également comment le Test-Driven Development (**TDD**) contribue à instaurer cette confiance dans nos tests. Il est important de noter que les principes **FIRST** doivent être appliqués avec une priorité plus élevée que les autres principes, tels que DRY (_Don't Repeat Yourself_) ou les principes _SOLID_. Le code de test comporte souvent des répétitions, mais en raison de l'importance de l'isolation et de l'indépendance, nous évitons généralement de les réduire. Nous éliminons les répétitions dans le code de création, mais la ligne de code qui crée notre contexte sera présente dans chaque test. Cela peut sembler une répétition, mais c'est une application des principes **FIRST** qui prend le pas sur le principe DRY. 🔁

Rappelez-vous également que les principes **FIRST** s'appliquent à tous les types de tests automatisés, mais leur pondération peut varier en fonction des tests unitaires, des tests d'intégration et des tests d'acceptation ou des tests de bout en bout. Vous aurez peut-être des milliers de tests unitaires et moins de tests d'acceptation, qui n'ont pas besoin d'être aussi rapides et peuvent être exécutés moins fréquemment. Les tests d'intégration qui impliquent des connexions à des API ou à des serveurs web peuvent nécessiter l'exécution du serveur web lui-même en tant que partie du test, ce qui peut être plus lent mais garantit l'isolation et la reproductibilité. ⚙️

Ainsi, les **cinq** principes **FIRST** ont été résumés, et bien qu'ils restent valables pour l'ensemble du cours, nous n'y consacrerons pas davantage de temps. ⏱️

Nous allons maintenant nous concentrer sur le **TDD** et voir comment il peut nous aider à appliquer les principes **FIRST**. 🧪
