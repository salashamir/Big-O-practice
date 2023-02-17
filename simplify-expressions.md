# STEP ONE.

### 1.

O(n)

### 2.

O(n)

### 3.

O(1)

### 4.

O(n^3)

### 5.

O(n)

### 6.

O(n)

### 7.

O(nlog(n))

### 8.

O(2^n)

### 9.

O(1)

### 10.

O(n^2)

# STEP TWO.

```javascript
function logUpTo(n) {
  for (let i = 1; i <= n; i++) {
    console.log(i);
  }
}
```

Time complexity: O(n)

```javascript
function logAtLeast10(n) {
  for (let i = 1; i <= Math.max(n, 10); i++) {
    console.log(i);
  }
}
```

Time complexity: O(n)

```javascript
function logAtMost10(n) {
  for (let i = 1; i <= Math.min(n, 10); i++) {
    console.log(i);
  }
}
```

Time complexity: O(1)

```javascript
function onlyElementsAtEvenIndex(array) {
  let newArray = [];
  for (let i = 0; i < array.length; i++) {
    if (i % 2 === 0) {
      newArray.push(array[i]);
    }
  }
  return newArray;
}
```

Time complexity: O(n)

```javascript
function subtotals(array) {
  let subtotalArray = [];
  for (let i = 0; i < array.length; i++) {
    let subtotal = 0;
    for (let j = 0; j <= i; j++) {
      subtotal += array[j];
    }
    subtotalArray.push(subtotal);
  }
  return subtotalArray;
}
```

Time complexity: O(n^2)

```javascript
function vowelCount(str) {
  let vowelCount = {};
  const vowels = "aeiouAEIOU";

  for (let char of str) {
    if (vowels.includes(char)) {
      if (char in vowelCount) {
        vowelCount[char] += 1;
      } else {
        vowelCount[char] = 1;
      }
    }
  }

  return vowelCount;
}
```

Time complexity: O(n)

# STEP THREE.

True or false: n^2 + n is O(n^2). 1. True

True or false: n^2 \* n is O(n^3). 2. True

True or false: n^2 + n is O(n). 3. False

What’s the time complexity of the .indexOf array method? 4. O(n)

What’s the time complexity of the .includes array method? 5. O(n)

What’s the time complexity of the .forEach array method? 6. O(n)

What’s the time complexity of the .sort array method? 7. O(nlog(n))

What’s the time complexity of the .unshift array method? 8. O(n)

What’s the time complexity of the .push array method? 9. 0(1)

What’s the time complexity of the .splice array method? 10. O(n)

What’s the time complexity of the .pop array method? 11. O(1)

What’s the time complexity of the Object.keys() function? 12. O(n)
