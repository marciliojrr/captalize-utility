# captalize-utility
Função utilitária para colocar as primeiras letras de um texto em upperCase.

## Código

```js
export const captalize = (text) => {
  if(!text) return undefined;
  var result = '';
  const words = text.split(' ');
  words.map(word => {
    if(word.length == 2) result += `${word} `;
    else result += `${word.charAt(0).toUpperCase() + word.slice(1)} `
  });
  return result.trim();
}
```
