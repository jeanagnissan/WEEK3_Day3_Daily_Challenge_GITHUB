
/**
 * Exercice Daily chalenge
 */
console.log("----------------Exercice Daily chalenge------------")

// 1- Créez un texte de type d'entrée qui prend/affiche uniquement des lettres. (c'est-à-dire que les chiffres et les caractères spéciaux ne seront pas acceptés)
// ok

// 2- utilisez l'un des événements suivants pour supprimer tout caractère qui n'est pas une lettre :
/*
keyup un événement
ou keypressévénement
ou keydownévénement
ou inputévénement 
*/
const letterInput = document.getElementById('letterInput');
    letterInput.addEventListener('keydown', (event) => {
        if (event.key < 65 || event.key > 90) {
        event.preventDefault();
    }
});

// 3- Astuce : Découvrez les codes d'accès en Javascript ou en expressions régulières
const letterInput2 = document.getElementById('letterInput');
letterInput2.addEventListener('input', () => {
  letterInput2.value = letterInput2.value.replace(/[^a-zA-Z]/g, '');
  console.log();
});

