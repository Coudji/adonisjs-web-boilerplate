Boilerplate for the [Adonisjs framework](https://adonisjs.com/) based on the [web starter kit](https://docs.adonisjs.com/guides/installation#web-starter-kit)

Use Adonisjs v6

:warning: Node.js >= 20.6 required

This boilerplate contain:
* Adonisjs framework's core
* Adonisjs auth package configured to session
* Adonisjs shield package for frontend security
* Adonisjs static package to serve static assets
* Edge template engine for HTML pages composition
* Lucid ORM preconfigured to use PostgreSQL
* VineJS for validation
* Vite for frontend assets compilation
* Added docker-compose file for setup the DB



# Usage

**Clone the repo:** (replace folder-name by what you want)

`git clone https://github.com/Coudji/adonisjs-web-boilerplate folder-name` and remove the .git folder

**Or**

`npx degit https://github.com/Coudji/adonisjs-web-boilerplate folder-name`

**Install the dependencies with pnpm:**

`pnpm i`

**Setup environement variables:**

`cp .env.example .env`

Don't forget to fill the missing parts

```
DB_PASSWORD=YOUR_DB_PASSWORD
DB_DATABASE=YOUR_DB_NAME
```

**Generate a new APP_KEY:**

`node ace generate:key`

**Mounting the Docker container if needed:**

`docker compose up -d`

**Migrate the db:**

`node ace migration:run`

**Start the dev server:**

`pnpm dev`

**To view all aviable commands:**

`node ace`