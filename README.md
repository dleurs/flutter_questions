# flutter_questions

## Technical / coding flutter questions 

1. Difference Stateless et Statefull
2.  If you want to display two non-fixed lenght scrollable list inside the same page (you scroll the first list then the second), do you use ListView or CustomScrollView / SliverChildBuilderDelegate
   
   a. Is shrinkWrap: true a problem ?
  
  => https://www.youtube.com/watch?v=LUqDNnv_dh0

3. What is the difference between Expanded and Flexible
   
   a. Which one is "wrap content" and "match parent" in terms of width / height

   => ![image](https://github.com/dleurs/flutter_questions/assets/58068925/d220e5d1-7f09-40aa-8349-0d018b5e396b)

5. Difference between final and const
   - run time / compile time
  
5.2 What is factory ?

Factory constructors return am instance of the class, but it doesn't necessarily create a new instance. Factory constructors might return an instance that already exists, or a sub-class.

https://flutterbyexample.com/lesson/factory-methods

https://medium.com/@shemsedinrobsen/understanding-factory-constructors-in-dart-and-flutter-a-comparison-with-static-methods-d03b471a7944

x. Versioning 

X.Y.Z
- x : Major / breaking changes
- y : minor / new features
- z : patches / bug fixing

6. Les différents type de test
   - unit test
   - integration test
   - widget test
   - golden test

  6. Comment résoudre un problème ?
     - docs officiel, google, github (issue, update), chatgpt

   7. Gestion de l'état
     
6.Difference between LinkedList et List not growable ?

|                                                          | LinkedList                                                                                         | List fixed-length                                        | List growable                                             | SortedList fixed-length                                  |
|----------------------------------------------------------|----------------------------------------------------------------------------------------------------|----------------------------------------------------------|-----------------------------------------------------------|----------------------------------------------------------|
| Taille fixe                                              | Non                                                                                                | Oui                                                      | Non                                                       | Oui                                                      |
| Comment stocké  en mémoire vive ?                        | fragmenté                                                                                          | uni                                                      | uni (avec buffer)                                         | uni                                                      |
| Rapidité en lecture via index  ex : list[23]             | o(n)                                                                                               | o(1)                                         | o(1)                                                      | o(1)                                                     |
| Rapidité en lecture contains() ex list.contains("apple") | o(n)                                                                                               | o(n)                                                     | o(n)                                                      | **o(log(n))**                                                |
| Complexité mémoire  pour ajouter un éléments             | On n'a besoin  uniquement de réserver l'espace mémoire d'un élément et de jouer avec les pointeurs | Copier entièrement la liste  dans une nouvelle liste + 1 | On utilise le buffer, si buffer plein alors on copie tout | Copier entièrement la liste  dans une nouvelle liste + 1 |


=> https://www.kodeco.com/books/data-structures-algorithms-in-dart/v1.0/chapters/3-basic-data-structures-in-dart

J'ai avec ma base de donnée SQL, une liste de rendez-vous (id, description), et des actions lié à ces rendez vous (id, idRdv, description). Quel structure de donnée ?

Benefits of Using Map:

1. Constant Time Lookup O(1)
2. Direct access by ID
3. No need to iterate through entire collection
4. Extremely fast retrieval


Unique Key Guarantee

Prevents duplicate IDs
Automatic key uniqueness


Memory Efficiency

Less overhead for large collections
Faster insertion and deletion


Easy Manipulation

Simple to add/remove by ID


When to Use List:

Order matters
Need to maintain insertion order
Frequent iteration required
Need to keep duplicate entries

When to Use Map:

Fast lookups by ID
Unique identifiers
Quick access/modification
Large datasets

Recommendations:

Use Map when primary access is by ID
Use List when order or duplicates matter
Consider converting lists to maps for performance-critical code



7.
- LinkedList Dart : https://api.flutter.dev/flutter/dart-collection/LinkedList-class.html
- List (Fixed or Growable) https://api.flutter.dev/flutter/dart-core/List-class.html
   - final growableList =
    List<int>.generate(3, (int i) => i * i, growable: true); // https://api.flutter.dev/flutter/dart-core/List/List.generate.html

9. Difference between Map and Array in terms of searching an element ?
   - o(log(n)) and o(n)
   - Et set ?
   -   Pas de doublon dans set


10. Difference between var and dynamic
11. debounce ?
    - https://bloc-event-transformers.web.app/bloc_event_transformers/debounce.html
    - https://stackoverflow.com/questions/67826924/what-is-debouncetime-buffer-throttle-methods-in-bloc
   
![dynamic_var](https://github.com/dleurs/flutter_questions/assets/58068925/00cdc679-ea48-43d2-bcd2-7c584d4b86c6)

   
7. What are Mixin ?
8. Sealed class ?
9. Stockage en flutter ?
    - SharedPreferences
    - FlutterSecureStorage
    - SQFlite ou Hive


11. Clean archi
      Presentation / Domain / Data
   - Présentation : cubit / state / pages
   - Domain : entities / abst repo / usecase
   - Data : Model / API / Mapper / Impl Repo

9.1 Différence BlocListener / BlocBuilder ?

## Archi / packages questions

1. How to handle state management ?
2. What package for navigation ?
3. How to test ?
4. How to store offline ? SQL or noSQL ?
5. What is clean archi ?
6. What is dependency injection and how is it good for repository ?


## Other
- English level

## Mobile in general

1. What are the differences between iOS and Android technically
   - Back navigation : Android inbeded inside bottom bar / iOS left to right swipe
   - In the past : notifications rights where available at installation for Android, asked for iOS
   - Different kind of notifications
  

2. What are the differences between iOS and Android in usage
   - Distribution between countries iOS/Android (~50/50 in the USA, 25/75 Europe, 5/95 India)
   - Users are more willing to pay on iOS than Android (for the latter, mostly AD)

3. What is the differences between mobile and web
   - Access to mobile storage, for media (sound, video) or secure storage
   - Gestion des versions, toujours à jour côté web
   - Tax
  
4. Difference in term of navigation between web and mobile ?
   - web : url based
   - mobile : mostly like an automaton

5. Quand est sortie l'iPhone 1 :
   - 2007
  

## Flutter general

1. Pros and cons flutter
   - DevExp
   - No SEO for web




