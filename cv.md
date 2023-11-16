# Yana Boychenko

## Contact

- Discord: .miyanka
- GitHub: [miyanka](https://github.com/miyanka)
- Telegram: @miyanka

## Profile

I have hands-on experience in working with relational databases and implementing database-driven applications. Nevertheless, web development has always been part of my professional interests. Therefore, I'm developing my skills in this area. My goal is to provide better interactivity and user experience.

## Skills

- HTML
- CSS (SCSS)
- JS
- Git
- Figma
- SQL

## Code example

As an example, I provide the solution for this [Codewars task](https://www.codewars.com/kata/526a569ca578d7e6e300034e)

```
const fromDecimal = (input, target) => {
  const base = target.length;
  let result = '';

  while (input) {
    result = target[input % base] + result;
    input = Math.floor(input / base);
  }

  return result;
};

const toDecimal = (input, source) => {
  const base = source.length;
  let result = 0;

  for (let i = 0; i < input.length; i++) {
    result += source.indexOf(input[input.length - 1 - i]) * Math.pow(base, i);
  }

  return result.toString();
};

const convert = (input, source, target) => {
  if (source === Alphabet.DECIMAL) {
    return fromDecimal(input, target);
  }

  if (target === Alphabet.DECIMAL) {
    return toDecimal(input, source);
  }

  const decimalValue = toDecimal(input, source);
  const targetValue = fromDecimal(decimalValue, target);
  return targetValue;
};
```
