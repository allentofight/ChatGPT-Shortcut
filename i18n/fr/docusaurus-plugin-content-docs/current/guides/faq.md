# Questions fréquentes

## Pourquoi les mots suggérés sont-ils en anglais ?

AiShort a été créé pour faciliter l'utilisation de ChatGPT par les personnes dont l'anglais n'est pas la langue maternelle. Cependant, tous les mots suggérés sont en anglais. Cela s'explique par le fait que ChatGPT a une meilleure compréhension de l'anglais par rapport aux autres langues. Même MOSS, le premier modèle de langage chinois de dialogue à grande échelle, reconnaît que ses réponses en anglais sont supérieures à celles en chinois. Il est donc recommandé d'utiliser les mots suggérés en anglais. (MOSS n'est plus disponible)

Bien que l'utilisation de mots suggérés dans d'autres langues puisse donner des résultats satisfaisants, les résultats peuvent varier considérablement lorsque vous saisissez à nouveau les mêmes prompts dans une autre langue. Étant donné que la compréhension de ChatGPT des prompts dans d'autres langues varie à chaque fois, il est conseillé d'utiliser des prompts en anglais pour les tâches axées sur la productivité afin d'obtenir le résultat souhaité. De plus, les réponses générées par des prompts en anglais sont susceptibles d'être en anglais. Vous pouvez spécifier la langue de réponse comme le chinois en ajoutant "répondre en chinois" à la fin du prompt. Si votre langue maternelle est différente, veuillez remplacer "chinois" par votre propre langue maternelle.

## Dois-je saisir le prompt à chaque fois ?

Dans l'API, vous pouvez définir le prompt comme un "prompt système", ce qui vous dispense de saisir le prompt à chaque fois. ChatGPT suivra les instructions basées sur le prompt système.

Dans la version Web de ChatGPT, si vous n'avez pas changé le prompt principal, vous pouvez simplement mettre le contenu de la réponse ultérieure entre guillemets, ce qui élimine la nécessité de saisir le prompt à chaque fois. Lorsque la réponse générée ne correspond pas aux exigences du prompt, cela signifie que ChatGPT a oublié le prompt, et dans de tels cas, vous devez ressaisir le prompt pour le recentrer. De plus, chaque lien de conversation est unique, et vous pouvez enregistrer les conversations fréquemment utilisées en tant que favoris pour une utilisation ultérieure.

## Délai de recherche de la méthode d'entrée

La fonction de recherche est basée sur la vitrine de Docusaurus et présente un problème de perte de focus de la méthode d'entrée côté PC. Après avoir signalé le problème à Docusaurus, ils ont mentionné qu'ils essaieraient de le résoudre, mais jusqu'à présent, le problème reste non résolu, avec le commentaire suivant : "FWIW, vous ne devriez pas utiliser le chinois de toute façon, car la vitrine n'est pas localisée." Par conséquent, j'ai catégorisé le composant de recherche en deux types : mobile et PC. La logique de recherche pour mobile reste inchangée, tandis que pour la navigation PC avec une largeur d'écran supérieure à 768px, j'ai introduit la fonction "debounce" pour résoudre le problème de la méthode d'entrée. Cependant, cela entraîne deux problèmes côté PC : la saisie en langue étrangère doit être terminée dans les 800 millisecondes, et le rafraîchissement de la recherche sur PC passe d'une réponse instantanée à un délai de 800 millisecondes. Si vous avez une meilleure solution, veuillez fournir des commentaires.

## Diffusion d'informations erronées

Bien que ChatGPT soit très puissant, il n'est pas infaillible. Parfois, il peut générer des informations erronées. Par exemple, lorsque j'ai dû saisir des centaines de données dans AiShort, j'ai demandé à ChatGPT de convertir les données dans un format spécifié. Cependant, lors du processus de conversion, j'ai remarqué que ChatGPT avait écrit certaines informations de manière incorrecte. Par exemple, un libellé dans le texte était "critique de film", mais ChatGPT l'a changé en "critique de cinéma". Bien que cela n'ait peut-être aucune incidence sur le texte lui-même, cela provoquerait une erreur lors de son utilisation dans le code. Par conséquent, lors de l'utilisation de ChatGPT, il est essentiel de vérifier sa sortie.

## Les mots suggérés ne fonctionnent pas bien

Tous les mots suggérés sont sourcés sur Internet et sont régulièrement mis à jour. Bien que j'aie testé chaque mot suggéré, les performances réelles peuvent varier en fonction des exigences spécifiques. Si vous découvrez des erreurs, avez des idées créatives ou possédez de bons mots suggérés, n'hésitez pas à fournir des commentaires et à contribuer sur la [page GitHub](https://github.com/allentofight/ChatGPT-Shortcut/discussions/11).

Si vous résumez ou condensez des informations, vous pouvez utiliser GPT pour affiner davantage les réponses originales, ce qui améliore la précision des réponses. De plus, les mots suggérés servent non seulement à des fins de productivité, mais ils aident également à élargir votre réflexion, à stimuler la créativité, à envisager des problèmes sous différents angles et à résoudre des problèmes qui sont facilement négligés lors du processus de réflexion.
