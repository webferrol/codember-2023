```js
const validate = payload => {
const [id, name, email, age, location] = payload
  if (!/^[a-zA-ZÀ-ÿ0-9]+$/.test(id)) return false
  if (!/^[a-zA-ZÀ-ÿ0-9]+$/.test(name)) return false
  if(!/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email)) return false
  if(age!=='' && isNaN(age)) return false
  if(location!=='' && !/^[a-zA-ZÀ-ÿ ]+$/.test(location)) return false
  return true
}


validate('O8TsZ7,jauTbB,bb@gmail.com,45,New York'.split(','))
```