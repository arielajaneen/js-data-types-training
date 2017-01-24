# Training: JavaScript Data Types

*Use the JavaScript console in your browser to solve the challenges. Press `command + option + J` to open the console in Chrome. Feel free to also record your responses in a file, but make sure you test them in the console!*

### Strings

1. Store your first name in a variable.
2. Concatenate your first name with your last name, and store the result in another variable.
3. Use the `String` <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split" target="_blank">`split`</a> method to turn your string variable from challenge #2 into an array.

### Arrays

1. An array called `foods` holds the names of my top 20 favorite foods, starting with the best food. How can you find my fifth favorite food?

  <details>
    <summary>answer</summary>
    ```js
    foods[4]
    ```
  </details>


2. Starting from the existing `friends` variable below, change the element that is currently "Elizabeth" to "Liz".


  ```js
  var friends = [
    "Moe",
    "Jane",
    "Emma",
    "Elizabeth",
    "Abanov",
    "Lycia"
  ];
  ```

  <details>
    <summary>answer</summary>
    ```js
    friends[3] = "Liz";
    ```
  </details>

3. Using array methods, add your name to the end of the `friends` array, and add another name to beginning.


  <details>
    <summary>hint</summary>
    Look up array methods `push` and `unshift`.
  </details>

  <details>
    <summary>answer</summary>
    ```js
    friends.push("Me!");
    friends.unshift("Someone else!");
    ```
  </details>

4. We have two lists of friends below. Use array methods to combine them into one alphabetically-sorted list.

  ```js
  var myFriends = [
    "Rickon",
    "Meera",
    "Hodor",
    "Jojen",
    "Osha",
    "Rickard",
    "Maester"
  ];

  var yourFriends = [
    "Bilbo",
    "Boromir",
    "Elrond",
    "Faramir",
    "Frodo",
    "Gandalf",
    "Legolas",
    "Pippin"
  ];
  ```

  <details>
    <summary>hint</summary>
    Look up array methods `concat` and `sort`.
  </details>

  <details>
    <summary>answer</summary>
    ```js
    var allFriends = myFriends.concat(yourFriends);
    allFriends.sort();
    ```
  </details>

5. This array contains 2 arrays, of different groups of friends. But everyone became friends! Merge these two arrays into a single array using array methods.

```js
var friends = [
  [
    "George",
    "John",
    "Ringo",
    "Paul"
  ], [
    "Brian",
    "Mick",
    "Keith",
    "Ian",
    "Bill",
    "Charlie"
  ]
]
```
  <details>
  <summary>answer</summary>
  ```js
  friends[0].concat(friends[1]);
  ```
  </details>

### Strings & Arrays
1. We have an array of the cardinal directions. In one line, get the first letter of the word "north" from this array.
```js
var directions = [
"north",
"south",
"east",
"west"
];
```
  <details>
  <summary>answer</summary>
  ```js
  directions[0][0];
  ```
  </details>

2. We need to use in-between directions, like "east northeast", when navigating. Build the string "east northeast" using this array.

  <details>
  <summary>answer</summary>
  ```js
  directions[2] + " " + directions[0] + directions[2];
  ```
  </details>

3. We can shorten east northeast into shorthand using just the first letters, ene. Build that string using this array.
  <details>
  <summary>answer</summary>
  ```js
  directions[2][0] + directions[0][0] + directions[2][0];
  ```
  </details>
