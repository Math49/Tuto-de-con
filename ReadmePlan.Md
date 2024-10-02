# Quel plan type pour un Readme ?

1. [Pourquoi suivre un modèle Readme ?](#pourquoi-suivre-un-modèle-readme-)
2. [Quel modèle ?](#quel-modèle-)
    1. [Le contenu](#le-contenu)
    2. [Les bonnes pratiques d'écriture](#les-bonnes-pratiques-décriture)

## Pourquoi suivre un modèle Readme ?

Un **README** (ou LISEZMOI) est un fichier texte (`.md`, `.txt`, `.docx`...) qui permet de détailler le contexte ou de préciser des informations nécessaires. Il est recommandé d'utiliser le format markdown, parce que celui-ci permet de convertir le contenu en HTML à l'aide de son balisage simple.


Le **formattage du fichier** est important pour sa lisibilité. Les balises titres (`#`, `##`...) indiquent la hiérarchie dans le fichier et peuvent aussi agir en tant que balises afin de mettre en place un sommaire sans difficulté, ainsi facilitant la navigation de l'utilisateur.

## Quel modèle ?

### Le contenu

Il est fortement recommandé de démarrer le **README** avec une balise titre de premier niveau *(avec la balise #)* contenant le nom du projet. Le nom du projet doit être clair et concis. À la suite de celui-ci, il est judicieux de rédiger un court paragraphe explicatif de ce projet.

Dans le cadre où la documentation contient plusieurs niveaux de titres, qu'elle est structurée, il est conseillé de mettre en place un sommaire. Depuis markdown, il est possible de cibler les balises titres directement depuis le sommaire afin de faciliter la navigation de l'utilisateur.

Le contenu à suivre dans le **README** dépend du projet. En général, il y a quelques conventions concernant ce que devrait contenir ce fichier.

__Un fichier README devrait contenir :__
- Une description générale du système ou du projet
- Le statut du projet *(dans le cadre où celui-ci est en phase de développement)*
- Les prérequis pour installer le projet
- Un guide pour accompagner l'utilisateur dans son installation
- Une liste des technologies utilisées et potentiellement des liens qui permettent de s'informer sur ces technologies mentionnées
- Les problèmes (bugs) repérés et ceux corrigés
- Une FAQ avec toutes les questions précédemment posées
- Les informations de licence et copyright

### Les bonnes pratiques d'écriture

À l'aide du formattage de markdown, il est possible de bien organiser le fichier. Lorsque l'on fait référence à une citation, on peut l'indiquer avec la balise `>`. Les balises de code devrait être indiquées entre `\`\`\`\`\`\``