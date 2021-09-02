## React & Apollo Pokemon Application

This application (a Pokemon application) was built using create-react-app as a base, and the technologies used were React & Apollo.

<p align="center">
![Preview](pokemon-preview.png?raw=true)
![Preview](pokemon-preview2.png?raw=true)
</p>

## How to use

Simply get Pokémon's information through queries in GraphQL, example:

```graphql
query {
  pokemon(name: "pikachu") {
    id
    name
    attacks {
      special {
        name      
        damage
      }
    }
```

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
