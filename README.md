
# CountJs⏫

Uma função para conseguir pegar as infos como se fosse de um console.count()

## Uso/Exemplos
Primeiro você adiciona está função 
```javascript
var count = (function() {
  var counter = {};
  return function(v) {
    return (counter[v] = (counter[v] || 0) + 1);
  }
}());
```
E logo após quando estiver utilizando um map por exemplo
```javascript
objCachorros.then(resolve => {
    resolve.map(function (obj) {
      if(obj.raca == "SRD")
      srd = count(obj.raca)
    })})
```
Pronto agora você sabe o numero de cachorros SRD no seu obj 🐶
