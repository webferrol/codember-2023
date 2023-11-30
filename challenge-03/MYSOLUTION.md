## sudo nljzuyfzb Para entrar en privado

# My solution

```js
function isValidCode (code = '1-6 h: hhhhhh') {
  const fields = code.split(' ')

  const [min, max] = fields[0].split('-').map(number => +number) /*split --> '1-6'*/

  const iterations = fields[2].split('').reduce((ac, current) => 
    current === fields[1][0] ? ac + 1 : ac  /*fields[1} --> 'hhhhhh' */
  ,0)

  return iterations >= min && iterations <= max 
}
```

## Example

```js
const keys = [ '1-7 p: ppppppp', '8-10 r: ozrcdfnug', '9-10 q: hvsazxrigf', '10-10 g: gifzgmpab', '7-8 w: lfpveulq', '8-10 f: xlcgglmllky', '7-9 w: siridrjzxqpngwr', '2-3 n: fkrmnniuxeboq', '8-10 g: zlbevnqppg', '1-6 a: yqvwieerrklo', '1-9 d: vxannmz', '8-10 u: hhjyvkckfxo', '7-10 i: nljzuyfzb', '9-10 c: imgjjpzdbmrw',]

let ac = 0
let index = 0;
for (let item of keys) {
  console.log(isValidCode(item)) // <- true, false, false
  if (!isValidCode(item)){
    ac++
  }
  if (ac === 2)
    break;
  index++
}
console.log(index, keys[index]) // <- 2 '9-10 q: hvsazxrigf'
```
