# Voire

Documentation: [https://doc.Voire.dev](https://doc.Voire.dev)

## Screenshot
<p align="center">
  <!-- <img width="900" src="https://cdn.Voire.dev/screenshot.png"> -->
</p>

## Getting started

### Prerequisites

 * Your machine needs to be ready for the latest [Laravel](https://laravel.com/docs/7.x#installation) and [Node.js](https://nodejs.org).


### Installing
#### Manual

```bash
# Clone the project and run composer
composer create-project tuandm/Voire
cd Voire

# Migration and DB seeder (after changing your DB settings in .env)
php artisan migrate --seed

# Install passport
php artisan passport:install

# Install dependency with NPM
npm install

# develop
npm run dev # or npm run watch

# Build on production
npm  run production
```

#### Docker
```sh
docker-compose up -d
```
Run database migration and seed within Docker container
```sh
# Get laravel docker container ID from containers list
docker ps

docker exec -it <container ID> php artisan migrate --seed 
# Where <container ID> is the "laravel" container name, ex: docker_laravel_1
```

`npm` commands are also supported:
```sh
docker exec -it <container ID> npm run watch 
# Where <container ID> is the "laravel" container name, ex: docker_laravel_1
...
```

## Running the tests
* Tests system is under development

## Built with
* [Laravel](https://laravel.com/) - The PHP Framework For Web Artisans
* [VueJS](https://vuejs.org/) - The Progressive JavaScript Framework
* [Element](https://element.eleme.io/) - A  Vue 2.0 based component library for developers, designers and product managers

## Authors

* **Richie Olivier M.N** - *Initial work* - [Ric-olive](https://github.com/Ric-olive).

## Donate
If you find this project useful, you can [buy me a coffee](https://www.buymeacoffee.com/tuandm)
