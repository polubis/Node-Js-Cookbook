1. Experience in Node JS 

Describe typical structure in Node JS

. What is dotenv ?

3. what is `uncaughtException` ?

4 what is `unhandledRejection` ?

. Explain what mean blocking or non-blocking behaviour

. Exmaples of async functions in node js

```js
// File 1
var i = 0;

// File 2
console.log(i) -> value
```

```js
a = 1;
var b = 2;
cFunc = function(e) {
  var c = 10;
  var d = 15;
  console.log(c);
  console.log(a); 
  function dFunc() {
    var f = 5;
    console.log(f)
    console.log(c);
    console.log(a); 
  }
  dFunc();
}
cFunc(10);
```

```js
function changeStuff(a, b, c)
{
  a = a * 10;
  b.item = "changed";
  c = {item: "changed"};
}

var num = 10; // 10
var obj1 = {item: "unchanged"}; 
var obj2 = {item: "unchanged"}; 

changeStuff(num, obj1, obj2);

console.log(num); // 10
console.log(obj1.item); // changed
console.log(obj2.item); // unchanged
```

```ts
interface Cloneable<T> {
    clone(): T;
}

interface User {
    name: string;
}

class UserModel implements Cloneable<UserModel> {
    data: User;
}
```

```js
var Frodo = new Hobbit();
Frodo.height = 100;
Frodo.weight = 300;
console.log(Frodo); // Output: ReferenceError: Hobbit is not defined
class Hobbit {
  constructor(height, weight) {
    this.height = height;
    this.weight = weight;
  }
}
```

Masz nastepujaca sytuacje:

```js
class User {
    constructor() {}
}

class AuthService {
    private _status: boolean;
}

```

What are LTS releases of Node.js?

LTS stands Long Term Support version of Node.js that receives all the critical bug fixes along with security updates and performance improvements. These versions are supported for at least 18 months and mainly focus on stability and security

V8 engine what is responsible in Node JS

Error first pattern in Node JS

```js
const fs = require('fs');
const folderPath = '/home/jim/Desktop/';

fs.readdir(folderPath, (err, files) => {
  files.forEach(file => {
    console.log(file);
  });
});
```

Implementujesz komunikacje w czasie rzeczywistym pomiedzy uzytkownikami. Jakiej technologi bys uzyl ? Jakich wzorcow projektowych ?

- uzytkownicy moga pisac do siebie,
- wiadomosci sa trzymane w bazie,
- system pilnuje kolejnosci,
- system wykonuje walidacje - tylko konkretni uzytkownicy moga pisac do siebie,
- skalowalnosc

Masz fragment legacy kodu w aplikacji - jest on uzywany w wielu plikach. Jednak chcialbys przepisac krok po kroku ten modul poniewaz jest on zle napisany. Jak bys do tego podszedl ?

Explain reactor pattern in Node JS

W jak sposob znalezc wycieki pamieci w Node

Did you head about Lock on Write behaviour in MongoDb

Which type of communications can you use to create real time behaviour in Node Js app

What is redis ?

Is MongoDb single threaded

Is MySql single threaded

Explain module.exports

What is commonJS modules

Drawback of true private

How to avoid callback hell

what reflect-metadata is

How to implement async task cancel feature in Node JS

Can you use RxJS in Node JS ?

Difference between relatives and non relatives dbs

Drawback of use ORMS

What is Dto's

2. How do you know the types of host objects ?

3. What is libuv ?

4. What is Event Loop and how it works in Node ?

5. Is Node Js single threaded ?

6. What cluster is and how they works ?

7. What is middleware (tell some examples) ?

8. Node Js architecture patterns (MVC, ONION) ?

9. How debug memory leak in Node JS ?

10. How to create new Node Js process ?

11. How to configure Node JS + Typescript

12. How to overwrite / change a weak type definition in Node Js ?

13. Authorization via JWT token ?

14. Authorization via session cookie ?

15. What http only cookies does

16. Functional programming vs object orientes in Node js ?

17. What is thread pool ?

18. Which design patterns would you use to create a chat ?

19. n+1 problem - explain in GraphQl or MongoDb / MySql

20. Which type of orms you used in Node

21. When use webpack in Node JS

22. How you implement features like online game via Node Js - chess

