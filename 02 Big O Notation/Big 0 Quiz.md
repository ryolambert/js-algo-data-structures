# Big 0 Quiz

### 1. Determine the time/space complexity of the following function:
---

``` javascript
function logUpTo(n) {
  for (let i = 1; i <= n; i++) {
    console.log(i);
  }
}
```
***Time ⏰***
  - [x] `O(n)`
  - [ ] `O(n^2)`
  - [ ] `O(n*log(n))`

***Space 🌌***
  - [x] `O(1)`
  - [ ] `O(n)`
  - [ ] `O(n^2)`

### 2. Determine the time/space complexity of the following function:
---

``` javascript
function logAtMost10(n) {
  for(let i = 1; i <= Math.min(n, 10); i++) {
    console.log(i);
  }
}
```
***Time ⏰***
  - [x] `O(1)`
  - [ ] `O(n)`
  - [ ] `O(n^2)`

***Space 🌌***
  - [x] `O(1)`
  - [ ] `O(n)`
  - [ ] `O(n^2)`

### 3. Determine the time/space complexity of the following function:
---

``` javascript
function logAtLeast10(n) {
  for(let i = 1; i <= Math.max(n, 10); i++) {
    console.log(i);
  }
}
```
***Time ⏰***
  - [x] `O(n)`
  - [ ] `O(1)`
  - [ ] `O(n*log(n))`

***Space 🌌***
  - [x] `O(1)`
  - [ ] `O(n)`
  - [ ] `O(n^2)`

### 4. Determine the time/space complexity of the following function:
---

``` javascript
function onlyElementsAtEvenIndex(array) {
  let newArray = Array(Math.ceil(array.length / 2));
  for (let i = 0; i < array.length; i++) {
    if (i % 2 === 0) {
      newArray[i / 2] = array[i];
    }
  }
  return newArray
}
```
***Time ⏰***
  - [x] `O(n)`
  - [ ] `O(1)`
  - [ ] `O(n^2)`

***Space 🌌***
  - [ ] `O(1)`
  - [x] `O(n)`
  - [ ] `O(n^2)`

### 5. Determine the time/space complexity of the following function:
---

``` javascript
function subTotals(array) {
  let subTotalArray = Array(array.length);
  for (let i = 0; i < array.length; i++) {
    let subTotal = 0;
    for (car j = 0; j <= i; j++) {
      subTotal += array[j];
    }
    subTotalArray[i] = subTotal;
  }
  return subTotalArray;
}
```
***Time ⏰***
  - [ ] `O(n)`
  - [ ] `O(1)`
  - [x] `O(n^2)`

***Space 🌌***
  - [ ] `O(1)`
  - [x] `O(n)`
  - [ ] `O(n^2)`