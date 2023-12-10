# final-assignment
# prosit 1
Le projet consiste à développer un logiciel de gestion de zoo en Java. L'ingénieur, récemment recruté chez ESPRIT TECH, doit créer une classe principale appelée "ZooManagement". Initialement, le programme affiche le nombre de cages (20) et le nom du zoo ("my zoo"). Par la suite, des modifications sont apportées pour permettre à l'utilisateur d'entrer ces données via le clavier à l'aide de la classe Scanner. Finalement, le programme affiche les informations mises à jour du zoo, prenant en compte les données saisies par l'utilisateur. L'objectif est de créer une application interactive de gestion de zoo en Java.
# prosit 2
Instruction 5:
Le chef de projet demande la création de deux classes, "Animal" et "Zoo", avec des attributs spécifiés. Deux objets, un animal (lion) et un zoo (myZoo), doivent être créés, et leurs attributs doivent être affectés.

Instruction 6:
Ajout de constructeurs paramétrés dans les classes "Animal" et "Zoo" pour simplifier l'initialisation des objets.

Instruction 7:
Création d'animaux en utilisant les nouveaux constructeurs paramétrés.

Instruction 8:
Création de la méthode "displayZoo()" dans la classe "Zoo" pour afficher les informations du zoo, et invocation de cette méthode dans la méthode "main". Problème d'affichage avec "System.out.println(myZoo)" et "System.out.println(myZoo.toString())".

Instruction 9:
Correction de l'affichage en surchargeant la méthode toString() dans les classes "Zoo" et "Animal".

Instruction 10:
Création de la méthode "addAnimal(Animal animal)" dans la classe "Zoo" pour ajouter un animal au tableau "animals". Test de la méthode en ajoutant plusieurs animaux et observation d'un problème lié à la surcapacité du zoo.

Instruction 11:
Ajout de méthodes pour afficher les animaux d'un zoo et rechercher un animal par son nom. Test de la méthode de recherche dans la classe principale.

Instruction 12:
Résolution d'un problème dans la recherche d'animaux identiques dans le zoo.

Instruction 13:
Création de la méthode "removeAnimal(Animal animal)" dans la classe "Zoo" pour supprimer un animal du zoo et renvoyer le succès de la suppression.
# prosit 3
Instruction 14:
La classe Zoo doit subir des modifications pour rendre l'attribut nbrCages constant et fixé à 25. Ces changements nécessitent des ajustements dans le constructeur.

Instruction 15:
Création de la méthode boolean isZooFull() dans la classe Zoo pour vérifier si le zoo est plein en fonction du nombre d'animaux et du nombre de cages.

Instruction 16:
Création de la méthode Zoo comparerZoo(Zoo z1, Zoo z2) dans la classe Zoo, qui prend deux objets de type Zoo comme paramètres et renvoie le Zoo avec le plus d'animaux.
# prosit 4
Instruction 17:
Le chef de projet propose de modifier la méthode addAnimal pour inclure la vérification de la capacité maximale du zoo en utilisant la méthode isZooFull() créée précédemment.

Instruction 18:
Pour protéger les caractéristiques des objets, des restrictions d'accès aux attributs de la classe Animal et Zoo sont nécessaires. Un animal ne peut pas avoir un âge négatif, et le nom d'un zoo ne doit pas être vide. Des modifications doivent être apportées pour corriger ces erreurs.

Instruction 19:
Pour organiser le code de manière plus structurée, le chef de projet recommande l'utilisation des packages "tn.esprit.gestionzoo.main" et "tn.esprit.gestionzoo.entities" pour les classes.
# prosit 5
Instruction 20:
Introduction de deux familles d'animaux pour simplifier la gestion des zoos : Aquatiques et Terrestres. Les animaux aquatiques ont un attribut "habitat", tandis que les animaux terrestres ont "nbrLegs". Deux sous-classes, Dolphin et Penguin, avec des attributs spécifiques ("swimmingSpeed" et "swimmingDepth") sont également introduites.

Instruction 21:
Création d'instances des classes créées précédemment en utilisant les constructeurs par défaut dans la méthode main.

Instruction 22:
Ajout de constructeurs paramétrés dans les sous-classes tout en protégeant les attributs précédemment déclarés.

Instruction 23:
Redéfinition de la méthode toString() dans les trois sous-classes pour inclure les attributs communs et spécifiques. Affichage des objets créés dans la méthode main.

Instruction 24:
Création de la méthode public void swim() dans les classes Aquatic, Dolphin et Penguin. Appel de cette méthode pour trois objets de types Aquatic, Dolphin et Penguin. Observation des résultats.

Ces instructions visent à introduire une hiérarchie d'héritage entre les classes d'animaux, démontrant ainsi la polymorphie et l'utilisation des méthodes redéfinies dans les sous-classes.
# prosit 6
Instruction 25:
Dans la classe Zoo, création d'un tableau aquaticAnimals capable de contenir jusqu'à 10 animaux aquatiques.

Instruction 26:
Création de la méthode public void addAquaticAnimal(Aquatic aquatic) dans la classe Zoo, permettant l'ajout d'animaux aquatiques au tableau aquaticAnimals. Ajout d'animaux aquatiques dans un zoo depuis la méthode main.

Instruction 27:
Affichage de la méthode swim() pour tous les animaux aquatiques dans le zoo. Observation des résultats.

Instruction 28:
Modification de la méthode swim() dans la classe Aquatic pour qu'elle soit obligatoirement redéfinie dans toutes les classes filles.

Instruction 29:
Création de la méthode public float maxPenguinSwimmingDepth() dans la classe Zoo, renvoyant la profondeur maximale de nage des pingouins dans le zoo.

Instruction 30:
Création de la méthode public void displayNumberOfAquaticsByType() dans la classe Zoo, affichant le nombre de dauphins et de pingouins dans le zoo.

Instruction 31:
Redéfinition de la méthode equals() dans la classe Aquatic, spécifiant que deux animaux aquatiques sont identiques s'ils ont le même nom, le même âge, et vivent dans le même habitat.
# prosit 7
Notre application rencontre certaines circonstances exceptionnelles qui peuvent
compromettre la poursuite normale de son exécution par exemple des données
incorrectes. Pour cela on devra utiliser un mécanisme pour assurer la bonne
exécution et omettre certaines situations.
Instruction 32 :
Modifiez le type de retour de la méthode ’’addAnimal(Animal animal)’’ de
boolean à void et enlevez les tests qui vérifient que le zoo est pas plein.
Instruction 33 :
Créez votre propre classe d’exception ZooFullException.
En effet, la méthode addAnimal devra utiliser cette nouvelle exception.
Corrigez les erreurs dans la méthode main sachant que votre programme doit
toujours afficher le nombre d’animaux après chaque ajout.
Réduisez le nombre de cages à 3 et testez votre code.
Instruction 34 :
On voulait interdire, l’ajout d’un animal ayant un âge négatif, en effet, nous devons
renvoyer l’exception levée à une classe InvalidAgeException qui va la gérer.
Corrigez les erreurs dans la méthode main.
# prosit 8
Instruction 35:
Création des interfaces suivantes :

Carnivore<T> qui définit la méthode void eatMeat(T meat)
Herbivore<T> qui définit la méthode void eatPlant(T plant)
Omnivore<T> qui hérite des deux interfaces précédentes et définit la méthode void eatPlantAndMeat(T food)
Instruction 36:
Création de l'enum Food définissant trois valeurs (MEAT, PLANT, BOTH).

Instruction 37:
Implémentation de l'interface Carnivore pour la classe Aquatic en passant l'énumération Food en paramètre. Implémentation de l'interface Omnivore pour la classe Terrestrial en passant également l'énumération Food en paramètre. Redéfinition des méthodes nécessaires.

Instruction 38:
Dans la méthode main, création d'objets de type Aquatic (Penguin) et Terrestrial, puis test des méthodes implémentées. Cela permet de vérifier le bon fonctionnement des interfaces et des énumérations dans les différentes classes.
# prosit 9
L'objectif est de développer une application de gestion des employés pour une société tunisienne, caractérisée par certaines propriétés d'un employé telles que l'identifiant, le nom, le prénom, le nom du département, et le grade. La classe d'employé comprend deux constructeurs, des méthodes Getter & Setter, la redéfinition des méthodes equals et toString.

Pour une meilleure gestion des entités, une interface IGestion est créée avec des méthodes spécifiques :

ajouterEmploye(T t): Ajout d'un employé.
rechercherEmploye(String nom): Recherche d'un employé par nom.
rechercherEmploye(T t): Recherche d'un employé.
supprimerEmploye(T t): Suppression d'un employé.
displayEmploye(): Affichage des employés.
trierEmployeParId(): Tri des employés par identifiant (utilisation de l'interface Comparable).
trierEmployeParNomDépartementEtGrade(): Tri des employés par nom, département et grade (utilisation de l'interface Comparator).
Il est ensuite demandé de créer une classe SocieteArrayList qui implémente l'interface IGestion en utilisant une structure de données ArrayList pour la gestion de la liste des employés.
# prosit 10
L'objectif est de créer une classe Departement pour la gestion des départements d'une entreprise. Chaque département est caractérisé par un identifiant, un nom de département, et un nombre d'employés. La classe Departement possède deux constructeurs, dont un sans paramètre, et redéfinit les méthodes equals et toString.

Pour une meilleure gestion des entités, une interface IDepartement est créée avec les méthodes suivantes :

ajouterDepartement(T t): Ajout d'un département.
rechercherDepartement(String nom): Recherche d'un département par nom.
rechercherDepartement(T t): Recherche d'un département.
supprimerDepartement(T t): Suppression d'un département.
displayDepartement(): Affichage des départements.
trierDepartementById(): Tri des départements par identifiant (utilisation de TreeSet).
L'utilisation de l'interface IDepartement vise à standardiser les opérations de gestion des départements, offrant une structure cohérente pour l'ajout, la recherche, la suppression, l'affichage et le tri des départements.
# prosit 11
L'objectif est de développer des méthodes pour gérer l'affectation des employés aux différents départements dans une application de gestion d'entreprise.

Instruction 1:
Création de la classe AffectationHashMap contenant une collection dynamique de paires clé-valeur, où chaque employé est affecté à un seul département.

Instruction 2:
Création de la méthode ajouterEmployeDepartement(Employe e, Departement d) dans la classe AffectationHashMap pour assurer l'affectation d'un employé à un département.

Instruction 3:
Développement de la méthode afficherEmployesEtDepartements pour afficher tous les employés et les départements auxquels ils sont affectés.

Instruction 4:
Développement de la méthode supprimerEmploye(Employe e) pour supprimer un employé de la collection.

Instruction 5:
Développement de la méthode supprimerEmployeEtDepartement(Employe e, Departement d) pour supprimer un employé travaillant dans un département spécifique.

Instruction 6:
Création de la méthode afficherEmployes() pour afficher la liste des employés.

Instruction 7:
Création de la méthode afficherDepartements() pour afficher la liste des départements.

Instruction 8:
Création de la méthode boolean rechercherEmploye(Employe e) pour tester l'existence d'un employé dans la collection.

Instruction 9:
Création de la méthode boolean rechercherDepartement(Departement d) pour tester l'existence d'un département dans la collection.

Instruction 10:
Développement de la méthode TreeMap<Employe, Departement> trierMap() qui retourne une collection de type TreeMap pour trier les employés selon leur identifiant.

# prosit 12
L'objectif est de créer une classe Etudiant représentant un étudiant caractérisé par un identifiant, un nom, et un âge. Cette classe comprend deux constructeurs, dont un sans paramètre, les méthodes getters & setters, ainsi que la redéfinition de la méthode toString.

Pour une meilleure gestion des entités, une interface Management est créée avec les méthodes suivantes :

void displayStudents(List<Student> students, Consumer<Student> con): Affiche les étudiants en utilisant un consommateur.
void displayStudentsByFilter(List<Student> students, Predicate<Student> pre, Consumer<Student> con): Affiche les étudiants filtrés selon un prédicat.
String returnStudentsNames(List<Student> students, Function<Student, String> fun): Renvoie les noms des étudiants en utilisant une fonction.
Student createStudent(Supplier<Student> sup): Crée un étudiant en utilisant un fournisseur.
List<Student> sortStudentsById(List<Student> students, Comparator<Student> com): Trie les étudiants par identifiant en utilisant un comparateur.
Stream<Student> convertToStream(List<Student> students): Convertit la liste des étudiants en un flux.
Cette interface vise à fournir des méthodes génériques pour la gestion d'étudiants, couvrant des opérations telles que l'affichage, le filtrage, la transformation, la création, le tri, et la conversion en flux.
# prosit 13
Le Prosit 13 se concentre sur l'utilisation des Stream API, une fonctionnalité importante de Java permettant le traitement de données de manière fonctionnelle et déclarative.

Les principales actions du Prosit 13 incluent :

Création de Streams : Utilisation de méthodes comme stream() et parallelStream() pour créer des flux à partir de collections ou d'autres sources de données.

Opérations intermédiaires : Application de transformations et de filtres aux flux, telles que map(), filter(), distinct(), limit(), et sorted().

Opérations terminales : Utilisation de méthodes terminales telles que forEach(), collect(), toArray(), reduce(), et count() pour effectuer des actions finales sur les éléments du flux.

Utilisation de Parallel Streams : Introduction de streams parallèles pour permettre un traitement concurrentiel des données.

Opérations avancées : Exploration des opérations avancées comme flatMap(), peek(), et la création de streams infinis.

Grouping and Partitioning : Utilisation de groupingBy() et partitioningBy() pour regrouper les éléments du flux.

Utilisation de l'API Optional : Introduction de Optional pour traiter les résultats potentiellement nuls des opérations de stream.

Comparaison avec les versions impératives : Comparaison de la syntaxe et de la performance des opérations de stream avec les approches impératives traditionnelles.

L'objectif global du Prosit 13 est de permettre aux développeurs de maîtriser l'utilisation efficace de la Stream API dans le traitement des collections de données en 
