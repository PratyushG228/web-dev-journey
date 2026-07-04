# Tips

## Early Return

Instead of

```js
if (name !== "") {
    // lots of code
}
```

Prefer

```js
if (name === "") return;
```

It reduces nesting and improves readability.

---

## One Function = One Job

Bad

```js
calculateBMI()
```

calculates BMI, updates DOM, validates input...

Good

```js
calculateBMI()

validateInput()

updateResult()
```

Each function has one responsibility.

---

## Think Before Coding

Ask:

- What is my input?
- What is my output?
- What data do I need?
- Can I split this into functions?