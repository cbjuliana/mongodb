# Mongodb

#### Exercício 1

Insira os seguintes registros no MongoDB e em seguida responda as questões abaixo: 

```
use petshop 
db.pets.insert({name: "Mike", species: "Hamster"}) 
db.pets.insert({name: "Dolly", species: "Peixe"}) 
db.pets.insert({name: "Kilha", species: "Gato"}) 
db.pets.insert({name: "Mike", species: "Cachorro"})
db.pets.insert({name: "Sally", species: "Cachorro"}) 
db.pets.insert({name: "Chuck", species: "Gato"})
```

1 - Adicione outro Peixe e um Hamster com nome Frodo 
#### Resposta

```
> db.pets.insert({name: "Frodo", species: "Peixe"})
WriteResult({ "nInserted" : 1 })
> db.pets.insert({name: "Frodo", species: "Hamster"})
WriteResult({ "nInserted" : 1 })
```

2 - Faça uma contagem dos pets na coleção 
#### Resposta

```
> db.pets.count()
8
```
