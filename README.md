# How this repo was built

1. `npx create-nx-workspace --preset=angular` to build repo for angular app with nx with options: 
    - Workspace name (e.g., org name) angularBasicWebsite
    - Application name frontend
    - Default stylesheet format SASS(.scss) [ http://sass-lang.com ]
    - Default linter ESLint [ Modern linting tool ]
    - Use Nx Cloud? (It's free and doesn't require registration.) No

2. `npm install --save-dev @nrwl/nest` to add NestJS support

3. `npx nx g @nrwl/nest:app backend --frontendProject=frontend` to generate the back end app

More in depth instructions about what was done can be found through the Nx tutorials: https://nx.dev/latest/angular/tutorial/01-create-application

# Run the apps
 - Start both with `npm run start`
 - Navigate to the main folder and type command `npm run start:frontend` to start the front end. Navigate to http://localhost:4200/
 - Navigate to the main folder and type command `npm run start:backend` to start the back end. Navigate to http://localhost:3333/songs for the base path

## Code scaffolding

Run `ng g component my-component --project=my-app` to generate a new component.

## Build

Run `ng build my-app` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test my-app` to execute the unit tests via [Jest](https://jestjs.io).

Run `nx affected:test` to execute the unit tests affected by a change.

## Running end-to-end tests

Run `ng e2e my-app` to execute the end-to-end tests via [Cypress](https://www.cypress.io).

Run `nx affected:e2e` to execute the end-to-end tests affected by a change.
