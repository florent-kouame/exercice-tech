Ce programme demande un nombre à l’utilisateur dans le terminal, puis l’affiche. Voici le code expliqué morceau par morceau.

# Importer l’outil de lecture
require sert à charger un module. Ici, readline est un outil déjà inclus dans Node.js qui permet de lire ce que l’utilisateur tape au clavier. On le range dans la constante readline.

# Créer l’interface
On crée un objet rl qui gère la conversation avec l’utilisateur :

input: process.stdin : le programme lit depuis le clavier.
output: process.stdout : le programme écrit à l’écran.

# Poser la question
"Entrez un nombre : " est le message affiché.
Le programme attend que l’utilisateur tape sa réponse et appuie sur Entrée.
(answer) => { ... } est une fonction de rappel (callback) : elle ne s’exécute qu’après la réponse. Ce qu’a tapé l’utilisateur est stocké dans answer, sous forme de texte, même si c’est 5.

# Convertir en nombre
Number() transforme le texte en vrai nombre : "42" devient 42. Si l’utilisateur tape abc, le résultat est NaN (Not a Number)

# Afficher le résultat
console.log écrit dans le terminal : le nombre est: 42

# Fermer l’interface
On arrête d’écouter le clavier. Sans cette ligne, le programme resterait bloqué en attente.

Déroulement complet
Entrez un nombre : 42
le nombre est: 42