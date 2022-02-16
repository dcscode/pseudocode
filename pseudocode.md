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
    makeChocolateMilk
    wash
    stir

Milk
    gotMilk --> yes or no
    milkLeft --> is milk >= 8 oz
    pourMilk --> add milk to glass


Chocolate Syrup
    gotSyrup --> yes or no
    addSyrup --> add syrup to glass

Glass
    isClean --> yes or no
    wash --> change value in isClean

Spoon
    isClean --> yes or no
    wash --> change value in isClean
    stir --> mix syrup and milk