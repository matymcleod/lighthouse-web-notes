### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  const lessThan20 = 'Quickly pick up some food and head back to the lab or kitchen where you can get to know your classmates better.';
  const between20To30 = 'You deserve a break, maybe try something new in the area';
  const moreThan30 = 'You can take your time because you are ahead if schedule but not too long as there is more work that you can do to stay ahead.';
  const notHungry = 'You have some time but not hungry, take a quick stretch break and get back to it until you get hungry';

  if (hungry) {
    if (availableTime < 20) {
      console.log(lessThan20);
    } else if ((availableTime >= 20) && (availableTime <= 30)) {
      console.log(between20To30);
    } else {
      console.log(moreThan30);
    }
  } else {
    console.log(notHungry);
  }
};
```