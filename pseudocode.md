# How to Make Chocolate Milk

## Functionality

**End Goal**: A glass of chocolate milk

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

## Objects

User 
    performs actions

Milk
    has volume

Glass
    can hold chocolate syrup and milk
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

## Pseudocode

```
IF user wants chocolate milk RUN makeChocolateMilk.

Program: Chocolate Milk

START 

    IF milk != 0
        IF milk >= 8 oz
            IF chocolate syrup true
                IF glass.isClean === true
                    IF spoon.isClean === true
                        user.addChocolateSyrup
                        user.addMilk
                        user.stir
                        user.drink
                        break
                    ELSE user.wash(spoon)
                ELSE user.wash(glass)
            ELSE user.drink
        ELSE break
    ELSE break

END


// wash function, takes object as argument
IF object.isClean != true
    return object.isClean === true

//add chocolate syrup function
IF glass.chocolateSyrup != true
    add chocolateSyrup property to glass

//add milk function
IF glass.milk != true
    add milk property to glass

//stir function
IF glass.milk && glass.chocolateSyrup === true
    add isChocolateMilk property to glass

//drink function
IF glass.isChocolateMilk === true
    reset glass object
```