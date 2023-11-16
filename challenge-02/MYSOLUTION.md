# My solution

```js
let ac = 0
const OPTIONS = {
  '#': value => value + 1,
  '@': value => value - 1,
  '*': value => value * value
}

// test
const code = '##*&' // output 4
const code2 = '&##&*&@&' //output 0243
const code3 = '&###@&*&###@@##@##&######@@#####@#@#@#@##@@@@@@@@@@@@@@@*&&@@@@@@@@@####@@@@@@@@@#########&#&##@@##@@##@@##@@##@@##@@##@@##@@##@@##@@##@@##@@##@@##@@##@@&'


const input = code3.split('')

const output = input.reduce(
  (previous, current) => {
    if (current === '&')
      return previous.concat('', ac)
    else {
      ac = OPTIONS[`${current}`](ac)
      return previous
    }
  },
  ''
)

console.log('Descodificado', output)
```