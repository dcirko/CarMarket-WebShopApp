# CarMarket

CarMarket is a web application for browsing and buying cars. Shoppers can filter listings, view vehicle details, and see their purchase history. Administrators can add, edit, and remove listings.

## Stack

The frontend uses Angular 18 and TypeScript. The Node.js API is in [server.js](server.js) and listens on port 3000. It uses MySQL. The repository includes a [database export](carzone%20-%20export%20baze.sql).

## Run locally

1. Install Node.js, npm, and MySQL. Import the database export locally and configure the connection in `server.js` to match your local MySQL setup.
2. Run `npm ci` from the repository root. The server also imports Express and CORS, which are absent from the package manifest. Install them locally with `npm install --no-save express cors`.
3. Run `node server.js` to start the API.
4. Run `npm start` in a second terminal and open http://localhost:4200/.

## Development commands

- `npm run build` builds the frontend under `dist/`.
- `npm test` runs the Angular unit tests through Karma.
- `npx ng generate component component-name` scaffolds a new component.
- End-to-end tests require adding a runner first.

[Angular CLI documentation](https://angular.dev/tools/cli)
