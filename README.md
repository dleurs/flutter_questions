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
     
6.Difference between Array and List ?
|                                              | LinkedList                                                                                         | List / Array                                                                                                                                    | Map                                                                                                |
|----------------------------------------------|----------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| Taille fixe                                  | Non                                                                                                | Oui                                                                                                                                             | Non                                                                                                |
| Comment stocké  en mémoire vive ?            | fragmenté                                                                                          | uni                                                                                                                                             | fragmenté                                                                                          |
| Rapidité en lecture  ex : list[23]           | o(n)                                                                                               | o(1) instantanné                                                                                                                                | o(log(n)) => Arbre rouge et noir                                                                   |
| Complexité mémoire  pour ajouter un éléments | On n'a besoin  uniquement de réserver l'espace mémoire d'un élément et de jouer avec les pointeurs | On a besoin de créer une nouvelle  liste, et donc de réserver (liste taille + 1) * taille élément  et de copier manuellement  tous les éléments | On n'a besoin  uniquement de réserver l'espace mémoire d'un élément et de jouer avec les pointeurs |
| Autorise les duplicats                       | Oui (sinon Set)                                                                                    | Oui                                                                                                                                             | clé différentes                                                                                    |

7. Difference between Map and Array in terms of searching an element ?
   - o(log(n)) and o(n)
   - Et set ?
   -   Pas de doublon dans set


8. Difference between var and dynamic
9. debounce ?
    - https://bloc-event-transformers.web.app/bloc_event_transformers/debounce.html
    - https://stackoverflow.com/questions/67826924/what-is-debouncetime-buffer-throttle-methods-in-bloc
   
![dynamic_var](https://github.com/dleurs/flutter_questions/assets/58068925/00cdc679-ea48-43d2-bcd2-7c584d4b86c6)

   
7. What are Mixin ?

## Archi / packages questions

1. How to handle state management ?
2. What package for navigation ?
3. How to test ?
4. How to store offline ? SQL or noSQL ?
5. What is clean archi ?
6. What is dependency injection and how is it good for repository ?




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




