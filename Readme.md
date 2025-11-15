Ce projet a pour objectif d’étudier l’impact des biais dans un workflow classique d’intelligence artificielle, ainsi que d’évaluer différentes méthodes de fine-tuning appliquées à un modèle LLM. L’idée centrale est de montrer comment un jeu de données peut influencer les décisions d’un modèle, comment ces biais peuvent être introduits puis analysés, et comment expliquer les prédictions à l’aide d’outils d’Explainable AI.

Le projet commence par la sélection d’un dataset réel. Une première analyse exploratoire est menée pour observer la répartition des variables et vérifier l’absence de biais majeurs initiaux. Ensuite, un biais artificiel est volontairement ajouté sur certaines variables sensibles (comme le sexe, l’âge, le BMI ou d’autres attributs) pour étudier son influence sur le modèle.

Deux versions du dataset sont utilisées : une version originale et une version modifiée contenant les biais. Un même modèle LLM est ensuite adapté à l’aide de trois techniques de fine-tuning : le full fine-tuning, LoRA et la distillation. Ces trois méthodes sont comparées afin d’évaluer leurs performances, leurs coûts et leur sensibilité aux biais présents dans les données.

Les modèles fine-tunés sont testés sur plusieurs exemples afin d’observer les différences de comportement entre modèle non biaisé et modèle biaisé. La méthode de fine-tuning la plus performante est retenue pour la suite.

Enfin, les décisions du modèle choisi sont expliquées à l’aide des outils XAI LIME et SHAP. Ces méthodes permettent de visualiser l’importance des variables dans les prédictions du modèle, de comprendre l’impact des biais introduits et de rendre les décisions plus transparentes.
Ce projet illustre donc l’ensemble du cycle : création de biais, entraînement de modèles, comparaison des approches de fine-tuning et explication des décisions grâce à des outils d’IA explicable.

