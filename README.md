```javascript

let count = 0;

function cc(card) {
  // Only change code below this line
  switch (card) {
    case 2:
    case 3:
    case 4:
    case 5:
    case 6:
      count++;
      break;
    case 10:
    case 'J':
    case 'Q':
    case 'K':
    case 'A':
      count--;
      break;
  }

  let holdbet = 'Hold';

  if (count > 0) {
    holdbet = 'Bet';
  }

  return count + " " + holdbet;
  // Only change code above this line
  
}


cc(2); cc(2); cc(7); cc('K'); cc('A');
console.log(cc(4));

```

# Takeaway

The ```javascript cc(2); cc(2); cc(7); cc('K'); cc('A');"``` at the bottom is referring to the cards that have been seen so far.

In this example, 2++(Now it's 1), 2++(2), 7++(3), K--(Now it goes down 2), A--(1)

The final result is a value of 1 which is greater than 0, so it would be recommended to bet as the chances of winning the hand would be higher.

[FreeCodeCamp](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/counting-cards)