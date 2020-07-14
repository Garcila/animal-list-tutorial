# tutorial

# Random selection from a list
In this tutorial we'll explore how to create a list of animals, and then select one animal from the list to be displayed on the Microbit.

## Step 1

Add an action to start the code by pressing Button A

```blocks
input.onButtonPressed(Button.A, function() {
})
```
Place the ``||input:onButtonPressed||`` block in work Area

## Step 2

Create a list of 3 animals by using the ``||array||`` group of blocks, and add it to the ``||input:button a||``

    
```blocks
   input.onButtonPressed(Button.A, function () {
      text_list = ['cat', 'bat','rat']
   })
```

## Step 3

Create two variables, chosenAnimal and randomNumber

```blocks
  chosenAnimal = ''
  randomNumber = 0;
  ```

## Step 4

Set our randomNumber variable to a random number from 0 to 2

```blocks
chosenAnimal = ''
randomNumber = 0;
randomNumber = randint(0,2)
```

## Step 5

Set 'chosenAnimal' to be the animal at the selected randomNumber position in the list

 ```blocks
  input.onButtonPressed(Button.A, function () {
      text_list = ['cat', 'bat','rat']
      chosenAnimal = text_list[randomNumber]
   })
 ```


## Step 6

Now display the name of the chosen animal using the ``||basic:show number||``

```blocks
    input.onButtonPressed(Button.A, function () {
        text_list = ['cat', 'bat','rat']
        chosenAnimal = text_list[randomNumber]
        basic.showString(chosenAnimal)
    })
```

## This is the last step @tutorialCompleted

Congratulations you completed the tutorial!

## This is a bonus activity that comes after the last step

Try adding a click on button B to show the same animal you just selected with button A
