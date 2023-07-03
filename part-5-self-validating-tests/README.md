# Les principes FIRST : Auto-Validation (Self-Validating)

Le quatrième principe **FIRST** est celui de _l'auto-validation_ des tests. Il s'agit d'un concept simple : les tests doivent pouvoir se valider automatiquement. Un test doit soit réussir, soit échouer clairement. Il ne devrait pas renvoyer un résultat ambigu tel que 20, car cela ne permet pas de déterminer si le test a réussi ou échoué. L'objectif est que le test puisse s'évaluer lui-même et rapporter explicitement s'il a produit le résultat attendu ou non. ✅❌

La notion d'auto-validation est extrêmement simple. Lorsqu'un test est exécuté, il doit retourner un résultat qui indique clairement s'il s'agit d'un succès ou d'un échec. Il n'y a pas de place pour l'ambiguïté. L'exécuteur du test doit être en mesure de rapporter le résultat de manière fiable et il devrait toujours être en mesure de le faire. Il n'y a pas de tension avec d'autres principes ici, c'est une règle fondamentale qui doit toujours être respectée. 💡

En fait, il n'est pas nécessaire de considérer cela comme un principe, mais plutôt comme une **règle de base** qui s'applique à tous les types de tests. Les tests unitaires, les tests d'intégration, les tests de bout en bout, tous doivent pouvoir s'auto-valider. Ils doivent être capables de revenir avec un résultat clair indiquant si tout s'est déroulé correctement ou s'il y a eu un échec. ✔️❌

En conclusion, l'auto-validation des tests est essentielle pour garantir la fiabilité des résultats. Les tests doivent pouvoir se valider automatiquement et fournir des réponses claires sur leur réussite ou leur échec. Cela permet d'obtenir un retour d'information immédiat et précis sur l'état du système testé. 🔄

Dans le prochain chapitre, nous aborderons les principes **FIRST** : **Thorough (exhaustifs)**. Ce sera le dernier de la série des principes **FIRST**. 🔚
