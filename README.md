## React & Apollo Pokemon Application

This application (a Pokemon application) was built using create-react-app as a base, and the technologies used were React & Apollo.

## Preview
![Preview](pokemon-preview.png?raw=true)

## Preview 2 
![Preview](pokemon-preview2.png?raw=true)

## How to use

Simply get Pokémon's information through queries in GraphQL, example:

```graphql
query {
  pokemon(name: "Pikachu") {
    id
    image
    name
    attacks {
      special {
        name        
        damage
      }
    }   
  }
}
```
Try this query [here](https://graphql-pokemon2.vercel.app/?query=query%20%7B%0A%20%20pokemon(name%3A%20%22Pikachu%22)%20%7B%0A%20%20%20%20id%0A%20%20%20%20image%0A%20%20%20%20name%0A%20%20%20%20attacks%20%7B%0A%20%20%20%20%20%20special%20%7B%0A%20%20%20%20%20%20%20%20name%20%20%20%20%20%20%20%20%0A%20%20%20%20%20%20%20%20damage%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%0A%20%20%7D%0A%7D%0A%0A%0A)!

### Production

```sh
yarn
yarn run build-app
yarn start
```

### Development

```sh
yarn
yarn run watch # Using nodemon for auto-reloading


## Related Projects

* [Pokemon Gopher](https://github.com/racerxdl/pokemon-gopher) - Fetch information about pokémons with GraphQL and GO 🙂
