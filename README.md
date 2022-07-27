# mimi
```shell
deng@fedora ~/Workspace/frontend-admin (master)$ cd ..
deng@fedora ~/Workspace/frontend-admin (master)$ code .
deng@fedora ~/Workspace/frontend-admin (master)$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
deng@fedora ~/Workspace/frontend-admin (master)$ git pull
Already up to date.
deng@fedora ~/Workspace/frontend-admin (master)$ ng update @angular/core@12 @angular/cli@12
The installed local Angular CLI version is older than the latest stable version.
Installing a temporary version to perform the update.
✔ Package successfully installed.
Using package manager: npm
Collecting installed dependencies...
Found 90 dependencies.
Fetching dependency metadata from registry...
                  Package "@ng-bootstrap/ng-bootstrap" has an incompatible peer dependency to "@angular/common" (requires "^10.0.0" (extended), would install "12.2.16").
                  Package "@ng-bootstrap/ng-bootstrap" has an incompatible peer dependency to "@angular/core" (requires "^10.0.0" (extended), would install "12.2.16").
                  Package "@ng-bootstrap/ng-bootstrap" has an incompatible peer dependency to "@angular/forms" (requires "^10.0.0" (extended), would install "12.2.16").
                  Package "@ng-bootstrap/ng-bootstrap" has an incompatible peer dependency to "@angular/localize" (requires "^10.0.0" (extended), would install "12.2.16").
                  Package "@ngrx/router-store" has an incompatible peer dependency to "@angular/router" (requires "^10.0.0" (extended), would install "12.2.16").
✖ Migration failed: Incompatible peer dependencies found.
Peer dependency warnings when installing dependencies means that those dependencies might not work correctly together.
You can use the '--force' option to ignore incompatible peer dependencies and instead address these warnings later.
  See "/tmp/ng-7chVHm/angular-errors.log" for further details.

deng@fedora ~/Workspace/frontend-admin (master)$ ng update @angular/core@12 @angular/cli@12 --force
The installed local Angular CLI version is older than the latest stable version.
Installing a temporary version to perform the update.
✔ Package successfully installed.
Using package manager: npm
Collecting installed dependencies...
Found 90 dependencies.
Fetching dependency metadata from registry...
                  Package "@ng-bootstrap/ng-bootstrap" has an incompatible peer dependency to "@angular/common" (requires "^10.0.0" (extended), would install "12.2.16").
                  Package "@ng-bootstrap/ng-bootstrap" has an incompatible peer dependency to "@angular/core" (requires "^10.0.0" (extended), would install "12.2.16").
                  Package "@ng-bootstrap/ng-bootstrap" has an incompatible peer dependency to "@angular/forms" (requires "^10.0.0" (extended), would install "12.2.16").
                  Package "@ng-bootstrap/ng-bootstrap" has an incompatible peer dependency to "@angular/localize" (requires "^10.0.0" (extended), would install "12.2.16").
                  Package "@ngrx/router-store" has an incompatible peer dependency to "@angular/router" (requires "^10.0.0" (extended), would install "12.2.16").
    Updating package.json with dependency @angular-devkit/build-angular @ "12.2.18" (was "0.1100.7")...
    Updating package.json with dependency @angular/cli @ "12.2.18" (was "11.2.19")...
    Updating package.json with dependency @angular/compiler-cli @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency @angular/language-service @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency karma @ "6.4.0" (was "5.2.3")...
    Updating package.json with dependency typescript @ "4.3.5" (was "4.0.8")...
    Updating package.json with dependency @angular/animations @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency @angular/common @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency @angular/compiler @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency @angular/core @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency @angular/forms @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency @angular/localize @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency @angular/platform-browser @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency @angular/platform-browser-dynamic @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency @angular/platform-server @ "12.2.16" (was "11.2.14")...
    Updating package.json with dependency @angular/router @ "12.2.16" (was "11.2.14")...
UPDATE package.json (3973 bytes)
✔ Packages successfully installed.
** Executing migrations of package '@angular/cli' **

▸ Remove deprecated options from 'angular.json' that are no longer present in v12.
    "build" target in "metronic" project is using a third-party builder.
    You may need to adjust the options to retain the existing behavior.
    For more information, see the breaking changes section within the release notes: https://github.com/angular/angular-cli/releases/tag/v12.0.0
  Migration completed.

▸ Update 'zone.js' to version 0.11.x.
  Read more about this here: https://github.com/angular/angular/blob/master/packages/zone.js/CHANGELOG.md#breaking-changes-since-zonejs-v0111
UPDATE package.json (3973 bytes)
UPDATE src/polyfills.ts (3002 bytes)
UPDATE src/test.ts (633 bytes)
UPDATE src/environments/environment.ts (1537 bytes)
✔ Packages installed successfully.
  Migration completed.

▸ Remove 'emitDecoratorMetadata' TypeScript compiler option.
  Decorator metadata is no longer needed by Angular.
  Read more about this here: https://www.typescriptlang.org/docs/handbook/decorators.html#metadata
    Skipping migration as the workspace uses third-party builders which may require "emitDecoratorMetadata" TypeScript compiler option.
  Migration completed.

▸ Lazy loading syntax migration.
  Update lazy loading string syntax to use dynamic imports.
  Migration completed.

▸ Remove deprecated ViewEngine-based i18n build and extract options.
  Options present in the configuration will be converted to use non-deprecated options.
  Migration completed.

▸ Updates Web Worker consumer usage to use the new syntax supported directly by Webpack 5.
  Migration completed.

▸ Remove invalid 'skipTests' option in '@schematics/angular:module' Angular schematic options.
  Migration completed.

▸ Replace the deprecated '--prod' in package.json scripts.
UPDATE package.json (3993 bytes)
  Migration completed.

An unhandled exception occurred: Cannot find module '@angular-devkit/core'
Require stack:
- /home/deng/Workspace/frontend-admin/node_modules/@angular/core/schematics/utils/project_tsconfig_paths.js
- /home/deng/Workspace/frontend-admin/node_modules/@angular/core/schematics/migrations/missing-injectable/index.js
See "/tmp/ng-Sw9WgT/angular-errors.log" for further details.
deng@fedora ~/Workspace/frontend-admin (master)$ yarn start
yarn run v1.22.17
$ node --max_old_space_size=8192 node_modules/@angular/cli/bin/ng serve
"BuildCustomWebpackBrowserSchema" schema is using the keyword "id" which its support is deprecated. Use "$id" for schema ID.
⠋ Generating browser application bundles (phase: setup)...Compiling @angular/core : es2015 as esm2015
Compiling @angular/cdk/keycodes : es2015 as esm2015
Compiling @angular/animations : es2015 as esm2015
Compiling @angular/common : es2015 as esm2015
Compiling @angular/cdk/observers : es2015 as esm2015
Compiling @angular/animations/browser : es2015 as esm2015
Compiling @angular/cdk/platform : es2015 as esm2015
Compiling @angular/cdk/bidi : es2015 as esm2015
Compiling @angular/platform-browser : es2015 as esm2015
Compiling @angular/forms : es2015 as esm2015
Compiling @angular/cdk/a11y : es2015 as esm2015
Compiling @angular/platform-browser/animations : es2015 as esm2015
Compiling @angular/cdk/collections : es2015 as esm2015
Compiling @angular/cdk/portal : es2015 as esm2015
Compiling @angular/cdk/scrolling : es2015 as esm2015
Compiling @angular/cdk/layout : es2015 as esm2015
Compiling @angular/common/http : es2015 as esm2015
Compiling @angular/material/core : es2015 as esm2015
Compiling @angular/cdk/overlay : es2015 as esm2015
Compiling @ngrx/store : es2015 as esm2015
Compiling @angular/router : es2015 as esm2015
Compiling @angular/material/form-field : es2015 as esm2015
Compiling @angular/material/button : es2015 as esm2015
Compiling @angular/cdk/text-field : es2015 as esm2015
Compiling @angular/material/tooltip : es2015 as esm2015
Compiling @angular/material/select : es2015 as esm2015
Compiling @angular/cdk/accordion : es2015 as esm2015
Compiling ngx-window-token : es2015 as esm2015
Compiling @angular/material/dialog : es2015 as esm2015
Compiling @angular/material/input : es2015 as esm2015
Compiling @angular/material/divider : es2015 as esm2015
Compiling @angular/cdk/stepper : es2015 as esm2015
Compiling @angular/material/icon : es2015 as esm2015
Compiling @angular/cdk/table : es2015 as esm2015
Compiling @angular/material/paginator : es2015 as esm2015
Compiling @angular/material/sort : es2015 as esm2015
Compiling @angular/cdk/tree : es2015 as esm2015
Compiling @angular/platform-browser-dynamic : es2015 as esm2015
Compiling @ngx-translate/core : es2015 as esm2015
Compiling @angular/material/progress-spinner : es2015 as esm2015
Compiling @angular/material/radio : es2015 as esm2015
Compiling ngx-perfect-scrollbar : es2015 as esm2015
Compiling ng-inline-svg : module as esm5
Compiling ngx-permissions : es2015 as esm2015
Compiling @ngrx/effects : es2015 as esm2015
Compiling @ngrx/router-store : es2015 as esm2015
Compiling @ngrx/store-devtools : es2015 as esm2015
Compiling angular-in-memory-web-api : module as esm5
Compiling @angular/material/snack-bar : es2015 as esm2015
Compiling @ngrx/entity : es2015 as esm2015
Compiling ngx-webstorage-service : es2015 as esm2015
Compiling @angular/material/tabs : es2015 as esm2015
Compiling @angular/material/expansion : es2015 as esm2015
Compiling @angular/material/card : es2015 as esm2015
Compiling ngx-clipboard : es2015 as esm2015
Compiling @angular/material/progress-bar : es2015 as esm2015
Compiling @ngx-loading-bar/core : es2015 as esm2015
Compiling ngx-highlightjs : es2015 as esm2015
Compiling @angular/material/slide-toggle : es2015 as esm2015
Compiling @angular/material/datepicker : es2015 as esm2015
Compiling @angular/material/autocomplete : es2015 as esm2015
Compiling @angular/material/bottom-sheet : es2015 as esm2015
Compiling @angular/material/button-toggle : es2015 as esm2015
Compiling @angular/material/chips : es2015 as esm2015
Compiling @angular/material/grid-list : es2015 as esm2015
Compiling @angular/material/list : es2015 as esm2015
Compiling @angular/material/menu : es2015 as esm2015
Compiling @angular/material/sidenav : es2015 as esm2015
Compiling @angular/material/slider : es2015 as esm2015
Compiling @angular/material/stepper : es2015 as esm2015
Compiling @angular/material/table : es2015 as esm2015
Compiling @angular/material/toolbar : es2015 as esm2015
Compiling @angular/material/tree : es2015 as esm2015
Compiling @angular/material/checkbox : es2015 as esm2015
Compiling @angular/material-moment-adapter : es2015 as esm2015
Compiling split-input : es2015 as esm2015
Compiling @ng-bootstrap/ng-bootstrap : es2015 as esm2015
Compiling ngx-markdown-editor : es2015 as esm2015
Compiling ngx-daterangepicker-material : es2015 as esm2015
⠦ Generating browser application bundles (phase: building)...WARNING: Using / for division is deprecated and will be removed in Dart Sass 2.0.0.

Recommendation: math.div(0.5em, $subscript-font-scale)

More info and automated migrator: https://sass-lang.com/d/slash-div

     ╷
6772 │   $subscript-margin-top: 0.5em / $subscript-font-scale;
     │                          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     ╵
    node_modules/@angular/material/_theming.scss 6772:26                    mat-form-field-typography()
    node_modules/@angular/material/_theming.scss 6996:3                     angular-material-typography()
    node_modules/@angular/material/_theming.scss 7024:3                     mat-core()
    src/assets/sass/theme/core/material-angular/_angular-material.scss 9:1  @import
    src/assets/sass/theme/layout/style-angular.scss 22:9                    root stylesheet

DEPRECATION WARNING: Using / for division is deprecated and will be removed in Dart Sass 2.0.0.

Recommendation: math.div(100%, $font-scale)

More info and automated migrator: https://sass-lang.com/d/slash-div

     ╷
6745 │   width: 100% / $font-scale + $mat-form-field-dedupe;
     │          ^^^^^^^^^^^^^^^^^^
     ╵
    node_modules/@angular/material/_theming.scss 6745:10                    -mat-form-field-label-floating()
    node_modules/@angular/material/_theming.scss 6815:7                     mat-form-field-typography()
    node_modules/@angular/material/_theming.scss 6996:3                     angular-material-typography()
    node_modules/@angular/material/_theming.scss 7024:3                     mat-core()
    src/assets/sass/theme/core/material-angular/_angular-material.scss 9:1  @import
    src/assets/sass/theme/layout/style-angular.scss 22:9                    root stylesheet

DEPRECATION WARNING: Using / for division is deprecated and will be removed in Dart Sass 2.0.0.

Recommendation: math.div($wrapper-padding-bottom, $subscript-font-scale)

More info and automated migrator: https://sass-lang.com/d/slash-div

     ╷
6849 │     top: calc(100% - #{$wrapper-padding-bottom / $subscript-font-scale});
     │                        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     ╵
    node_modules/@angular/material/_theming.scss 6849:24                    mat-form-field-typography()
    node_modules/@angular/material/_theming.scss 6996:3                     angular-material-typography()
    node_modules/@angular/material/_theming.scss 7024:3                     mat-core()
    src/assets/sass/theme/core/material-angular/_angular-material.scss 9:1  @import
    src/assets/sass/theme/layout/style-angular.scss 22:9                    root stylesheet

DEPRECATION WARNING: Using / for division is deprecated and will be removed in Dart Sass 2.0.0.

Recommendation: math.div($line-height - 1, 2)

More info and automated migrator: https://sass-lang.com/d/slash-div

     ╷
6305 │   $line-spacing: ($line-height - 1) / 2;
     │                  ^^^^^^^^^^^^^^^^^^^^^^
     ╵
    node_modules/@angular/material/_theming.scss 6305:18                    mat-form-field-legacy-typography()
    node_modules/@angular/material/_theming.scss 6852:3                     mat-form-field-typography()
    node_modules/@angular/material/_theming.scss 6996:3                     angular-material-typography()
    node_modules/@angular/material/_theming.scss 7024:3                     mat-core()
    src/assets/sass/theme/core/material-angular/_angular-material.scss 9:1  @import
    src/assets/sass/theme/layout/style-angular.scss 22:9                    root stylesheet

DEPRECATION WARNING: Using / for division is deprecated and will be removed in Dart Sass 2.0.0.

Recommendation: math.div(0.5em, $subscript-font-scale)

More info and automated migrator: https://sass-lang.com/d/slash-div

     ╷
6316 │   $subscript-margin-top: 0.5em / $subscript-font-scale - ($line-spacing * 2);
     │                          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     ╵
    node_modules/@angular/material/_theming.scss 6316:26                    mat-form-field-legacy-typography()
    node_modules/@angular/material/_theming.scss 6852:3                     mat-form-field-typography()
    node_modules/@angular/material/_theming.scss 6996:3                     angular-material-typography()
    node_modules/@angular/material/_theming.scss 7024:3                     mat-core()
    src/assets/sass/theme/core/material-angular/_angular-material.scss 9:1  @import
    src/assets/sass/theme/layout/style-angular.scss 22:9                    root stylesheet

WARNING: 32 repetitive deprecation warnings omitted.

✔ Browser application bundle generation complete.

Initial Chunk Files | Names         |      Size
main.js             | main          |  20.11 MB
styles.css          | styles        |   1.84 MB
polyfills.js        | polyfills     |   1.76 MB
scripts.js          | scripts       | 298.26 kB
runtime.js          | runtime       |  13.12 kB

                    | Initial Total |  24.02 MB

Lazy Chunk Files    | Names         |      Size
459.js              | -             |  24.12 kB
314.js              | -             |  23.52 kB

Build at: 2022-07-27T06:34:07.677Z - Hash: 5d44ed247c39ea41f9b2 - Time: 75494ms

./node_modules/amazon-cognito-identity-js/es/utils/cryptoSecureRandomInt.js:20:13-30 - Warning: Module not found: Error: Can't resolve 'crypto' in '/home/deng/Workspace/frontend-admin/node_modules/amazon-cognito-identity-js/es/utils'

BREAKING CHANGE: webpack < 5 used to include polyfills for node.js core modules by default.
This is no longer the case. Verify if you need this module and configure a polyfill for it.

If you want to include a polyfill, you need to:
	- add a fallback 'resolve.fallback: { "crypto": require.resolve("crypto-browserify") }'
	- install 'crypto-browserify'
If you don't want to include a polyfill, you can use an empty module like this:
	resolve.fallback: { "crypto": false }

Warning: ./AuthenticationHelper depends on 'crypto-js/sha256'. CommonJS or AMD dependencies can cause optimization bailouts.
For more info see: https://angular.io/guide/build#configuring-commonjs-dependencies

Warning: ./CognitoUser depends on 'crypto-js/enc-base64'. CommonJS or AMD dependencies can cause optimization bailouts.
For more info see: https://angular.io/guide/build#configuring-commonjs-dependencies

Warning: /home/deng/Workspace/frontend-admin/src/app/views/pages/admin/booking-list/booking-list.component.ts depends on 'jsonata/jsonata-es5'. CommonJS or AMD dependencies can cause optimization bailouts.
For more info see: https://angular.io/guide/build#configuring-commonjs-dependencies



** Angular Live Development Server is listening on localhost:4202, open your browser on http://localhost:4202/ **


✔ Compiled successfully.
✔ Browser application bundle generation complete.

7 unchanged chunks

Build at: 2022-07-27T06:34:19.204Z - Hash: 109a416e19304edaf143 - Time: 5159ms

./node_modules/amazon-cognito-identity-js/es/utils/cryptoSecureRandomInt.js:20:13-30 - Warning: Module not found: Error: Can't resolve 'crypto' in '/home/deng/Workspace/frontend-admin/node_modules/amazon-cognito-identity-js/es/utils'

BREAKING CHANGE: webpack < 5 used to include polyfills for node.js core modules by default.
This is no longer the case. Verify if you need this module and configure a polyfill for it.

If you want to include a polyfill, you need to:
	- add a fallback 'resolve.fallback: { "crypto": require.resolve("crypto-browserify") }'
	- install 'crypto-browserify'
If you don't want to include a polyfill, you can use an empty module like this:
	resolve.fallback: { "crypto": false }



✔ Compiled successfully.
```
