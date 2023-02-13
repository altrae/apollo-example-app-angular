# Example App - Angular

## Start the app

Install the dependencies and start the server.

```sh
npm install
npm start
```

The last command should open your browser and navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## abds component usage

Pre requisites:

1. Add `@abds/components` into your `package.json` as a dependency

Using a Stencil built web component collection within an Angular CLI project is a two-step process. We need to:

1. Include the `CUSTOM_ELEMENTS_SCHEMA` in the modules that use the components.
   - In this example it is used here `src/app/app.module.ts`.
2. Call `defineCustomElements()` from `main.ts` (or the project's entry point).
   - In this example it is imported in `src/main.ts` and then invoked later in that file.
   - This function is provided by Stencil's loader and it allows components to be lazy-loaded.

By importing the abds custom components above, Angular will let you use them freely throughout your project. All abds components use the `<abds-` prefix. You can see an instance of the `<abds-button>` being used in `src/app/app.component.html`.

## Additional information

For more information about the abds components that are available and their props see our [ZeroHeight documentation.](https://zeroheight.com/6af807fb0/v/latest/p/56f98e-components/b/173c7d)

For more information about integrating with Angular see [Stencil's documentation here.](https://stenciljs.com/docs/angular)

---

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 15.1.5.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
