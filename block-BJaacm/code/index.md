```js
let user = {
  name: "Arya",
  sibling: ["Robb", "Ryan", "John"],
};
let allBrothers = ["Robb", "Ryan", "John"];
let brothersCopy = user.sibling;
let usename = user.name;
let newUser = user;
```

1. Memory representation

- Create the memory representation of the above snippet on notebook.
- Take a photo/screenshot and add it to the folder `code`

<!-- To add this image here use ![name](./hello.jpg) -->

./Capture.PNG

2. Answer the following with reason:

- `user == newUser;` // output and reason true - as both will have same address
- `user === newUser;` true - as both will have same address
- `user.name === newUser.name;` true as both have same values at same adress
- `user.name == newUser.name;` true as both have same values at same adress
- `user.sibling == newUser.sibling;` true as both have same values at same adress
- `user.sibling === newUser.sibling;` true as both have same values at same adress
- `user.sibling == allBrothers;` false as both array's at different address
- `user.sibling === allBrothers;` false as both array's at different address
- `brothersCopy === allBrothers;` false as both array's at different address
- `brothersCopy == allBrothers;` false as both array's at different address
- `brothersCopy == user.sibling;` true as both array's same address
- `brothersCopy === user.sibling;` true as both array's same address
- `brothersCopy[0] === user.sibling[0];` true as both array's same value
- `brothersCopy[1] === user.sibling[1];` true as both array's same value
- `user.sibling[1] === newUser.sibling[1];` true as both array's same value
