# firebase-hosting-404-error-solution

### General Info
***
The most common error while hosting on Firebase was "Page not found." This is the ultimate solution to these problems.

### Screenshot
![Screenshot](https://i.ibb.co/cNyw8k7/161684728-892531181535923-1886768611045037189-n.jpg)

## Installation
***
You only need to remove all the codes from the firebase.json file before pasting it.
```
 {
"hosting": {
"public": "build",
"ignore": [
"firebase.json",
"**/.*",
"**/node_modules/**"
],
"rewrites": [
{
"source": "**",
"destination": "/index.html"
}
]
}
}
```