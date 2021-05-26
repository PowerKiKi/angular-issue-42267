# Angular issue #42267

See https://github.com/angular/angular/issues/42267

This app was generated with:

```
ng new  --strict --no-routing --style=css app
```

Running `yarn start` should compile without error, but it incorrectly fails with:

```
yarn run v1.22.5
$ ng serve
✔ Browser application bundle generation complete.

Initial Chunk Files | Names         |    Size
main.js             | main          | 0 bytes
polyfills.js        | polyfills     | 0 bytes
runtime.js          | runtime       | 0 bytes
styles.css          | styles        | 0 bytes
vendor.js           | vendor        | 0 bytes

                    | Initial Total | 0 bytes

Build at: 2021-05-26T07:41:00.355Z - Hash: e7cdce6c6be13af310f7 - Time: 6342ms

Error: src/app/app.component.html:5:23 - error TS2322: Type 'null' is not assignable to type 'string | number'.

5 <input type="number" [min]="null" [formControl]="control">
                        ~~~

  src/app/app.component.ts:6:16
    6   templateUrl: './app.component.html',
                     ~~~~~~~~~~~~~~~~~~~~~~
    Error occurs in the template of component AppComponent.




** Angular Live Development Server is listening on localhost:4200, open your browser on http://localhost:4200/ **

```
