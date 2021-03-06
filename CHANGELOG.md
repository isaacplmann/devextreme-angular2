# 16.1.7-alpha (2016-09-19)
###Angular 2.0.0 version.

We have supported [NgModules](https://angular.io/docs/ts/latest/api/core/index/NgModule-interface.html) in the context of updating to Angular 2.0.
You can read more about NgModules [here](https://angular.io/docs/ts/latest/guide/ngmodule.html).

We defined `NgModule` for each of our components: `DxButtonModule`, `DxCheckBoxModule`, `DxTextBoxModule`, etc.

To make the process of migration easier, you can check our [updated README](https://github.com/DevExpress/devextreme-angular2#adding-devexteme-widgets-to-an-angular-2-application) and take a look at [this commit](https://github.com/DevExpress/devextreme-angular2/commit/50b6d6).

Also we defined a `DevExtremeModule`, which exports all our components:

```TypeScript
import { DevExtremeModule } from 'devextreme-angular2';
```

###Breaking changes

- Added 'Directive' suffix has been added to the `DxTemplate` directive's class name. Use `DxTemplateDirective` instead of `DxTemplate`.
- Added 'Component' suffix has been added to all our components' class names. Example: Use `DxButtonComponent` instead of `DxButton`.

We made these changes according to the [Angular 2 style guide](https://angular.io/docs/ts/latest/guide/style-guide.html#!#02-03).