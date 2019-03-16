+++
date = "2017-01-22T18:04:24-05:00"
title = "JSON"
toc = true
prev = "/17-working-with-apis/agenda"
next = "/17-working-with-apis/api-overview"
weight = 7

+++

## What is JSON?

- Stands for JavaScript Object Notation

- A way to store information in an organized, easy-to-access manner

- A popular way to send data from on web server (service) to another

- Resembles a normal Javascript Object (it contains properties and values) but **does not** contain methods


```

{
  "id": 1,
  "name": "Scoobie Doo",
  "favoriteFood": "Scoobie Snacks"
}


```

---

## JSON Guidelines

- Property names **must be double-quoted strings**

- Use meaningful property names

- Access properties of a JSON object using dot notation

```

// json object that contains smurfs

var smurfs = {
    "papa" : {
        "name" : "Papa Smurf",
        "gender" : "male"
    },
    "smurfette" : {
        "name" : "Smurfette",
        "gender" : "female"
    }
}

console.log(smurfs.smurfette.name);
console.log(smurfs.smurfette.gender);

```

---

## JSON.stringify()

- Since JSON is used to send data from one service to the next "over the wire" (i.e. via cloud) it is transmitted as a string which makes it lightweight and fast

- `JSON.stringify()` is a method that turns an JSON object into a string

- "Stringify-ing" JSON objects is a common step developers take before sending data to another service


```
  var smurfs = {
      "papa" : {
          "name" : "Papa Smurf",
          "gender" : "male"
      },
      "smurfette" : {
          "name" : "Smurfette",
          "gender" : "female"
      }
  }

  var stringJSON = JSON.stringify(smurfs));


  // result: "{"papa":{"name":"Papa Smurf","gender":"male"},"smurfette":{"name":"Smurfette","gender":"female"}}"

  console.log(typeof stringJSON); // result: string

```

<a class="jsbin-embed" href="https://jsbin.com/sudalo/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.6"></script>

---

## JSON.parse() 

- When JSON is **received** from another service, it is in a string format

- In order to effectively work with JSON data in our code, we need to covert it so an object (or array)

- JSON.parse() is a method that converts an JSON object to an Javascript object or array

<a class="jsbin-embed" href="https://jsbin.com/cibixis/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.6"></script>
