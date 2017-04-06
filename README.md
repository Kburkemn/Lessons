# Lessons
Short examples of learning coding


//Write a loop that gives you the 9's times table,from 9 x 1 = 9 to 9 x 12 = 108.
for (var i = 1; i <= 12; i++) {
    var timesNine = i * 9;
    console.log(timesNine);
}

//use a loop inside a loop to write all the times tables, from 1 to 12
for (var i = 1; i <= 12; i++) {
      for (var j = 1; j <= 12; j++) {
        var times = i * j;
        console.log(times);
    }
}

//Arrays
var favoriteFoods = ['pizza', 'popcorn', 'ice cream'];
console.log('My favorite food is ' + favoriteFoods[1]);
//output = My favorite food is popcorn

//Array plus for loop
var favoriteFoods = ['pizza', 'popcorn', 'ice cream'];

for (var i = 0; i < favoriteFoods.length; i++) {
    console.log('My favorite food is ' + favoriteFoods[i]);
}

//Objects
var favoriteRecipe = {
    recipeTitle: 'Cookies',
    servings: 1,
    ingredients: ['flour', 'sugar', 'eggs'],
    directions: 'mix and bake'
};

console.log(favoriteRecipe.servings);

//create a loop to list all ingredients from an object property
for (var i = 0; i < favoriteRecipe.ingredients.length; i++) {
    console.log(favoriteRecipe.ingredients[i]);
}

//object method
var favoriteRecipe = {
    recipeTitle: 'Cookies',
    servings: 1,
    ingredients: ['flour', 'sugar', 'eggs'],
    directions: 'mix and bake',
    letsCook: function() {
        console.log('I\'m hungry! Let\'s cook ' + favoriteRecipe.recipeTitle);
    }
};

favoriteRecipe.letsCook();
