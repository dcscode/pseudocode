# How to Make Chocolate Milk

## Functionality

**End Goal**: A glass of chocolate milk

## Objects

Milk
    has volume


Glass
    status: clean or unclean


Chocolate Syrup
    has volume


Spoon
    status: clean or unclean

## Functions

User
    wash --> change value in isClean
    stir --> mix syrup and milk

Milk
    gotMilk --> yes or no
    milkLeft --> is milk >= 8 oz
    pourMilk --> add milk to glass


Chocolate Syrup
    gotSyrup --> yes or no
    addSyrup --> add syrup to glass

Glass
    isClean --> yes or no

Spoon
    isClean --> yes or no
    
````
1. User wants chocolate milk.
2. Is there milk?
    - Yes --> is there enought milk?
            - Yes --> proceed
            - No --> cry, drink what's left
    - No --> no chocolate milk, cry
3. Is there chocolate syrup?
    - Yes --> proceed
    - No --> cry and/or just have milk
4. Is there a clean glass?
    - Yes --> proceed
    - No --> wash a glass --> proceed
5. Is there a clean spoon?
    - Yes --> proceed
    - No --> wash a spoon --> proceed
6. Add chocolate syrup to glass.
7. Add milk to glass.
8. Stir.
9. Drink chocolate milk.
````
