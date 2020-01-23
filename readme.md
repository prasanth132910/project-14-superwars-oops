# ProGrad

## LAB | ProGrad Superwars

Dustin and Lucus are best friends, they spend their weekends watching superhero series and playing superhero games. One Friday in school Mr.Hooper who is their computer science faculty member taught them HTML, CSS, and JavaScript. So what's next? It's Weekend! Lucus and Dustin will be on their laptops. Are they watching series or playing games? Lucus says, No we are building a new game.

Lucus always loves protagonists like most of us. But Dustin is quite crazy he likes antagonists. So now they are collecting a bunch of their favorite Super Heroes and Super-Villains names along with images. Did they tell you about the game that they are building? Uh no. Okay, lemme explain. They are going to facilitate the ultimate war between Super Heroes and Super-Villains. As they are new to these technologies, they need **YOU** to help them build this game. Go to the `src/app.js` file and complete all the unfinished code to propel both of these young champ's dreams.

## What should you do?

- Fork this repo
- Clone this repo
- Practice JavaScript Oops -  _classes, objects, member variables, member functions_

## How do you submit?

- Upon completion, run the following commands:

  ```
  git add .
  git commit -m "prograd ID"
  git push origin master
  ```

- Create a pull request so your teaching mentors can check your work.

## Starter code

The `src/app.js` contains an array of 20 Super Heroes and Super-Villains. We are talking about the array of 20 _strings_ containing each Super Heroes and Super-Villains names. Here is one example of how the data is displayed:

```javascript
[
    "Spiderman"
]
```

### Tests

Ohh yes! We have our beloved tests, and you already know how this works. Open the `SpecRunner.html` file on your browser and start coding to pass the test. Remember to focus on one test at a time and read carefully the instructions to understand what you have to do.

## Trial 1: RETHINK ! REUSE !

Kudos so far so good ! Add `member variables` like id, name, strength, image and type to `class` `Player` then assign them appropriate values such that it _return a valid player object_.
*  `strength` can be generated from `getRandomStrength()` `member function`, which _return a random strength_ from 1 to 100 .
* `image` can be sequential i.e. "images/super-"+(i+1)+".png"  
* `type` of player can alternating between hero and villain or your own logic
    ```javascript
    [
        {
            id:1,
            name:"Super Man",
            strength:100,
            img:"images/hero-1.png",
            type:"hero|villain"
        }
    ]
    ```

## Trial 2: MAKE IT SUBTLE !

Dustin and Lucus wants to create players for displaying so help them by creating a method `view()`, to accumulate HTML template as below and _return an HTML element_.
```JS
<div class="player" data-id="${players[i].id}">
    <img src="${players[i].image}">
    <div class="name">${players[i].name}</div>
    <div class="strength">${players[i].strength}</div>
</div>
```

## Trial 3: THE SUPER WAR !

To begin the war there should be players, we can generate players by creating object for class `Superwars`, which should use `map` array method to loop through passed constant and _return `Player` Objects_. 