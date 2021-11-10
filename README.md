# EscraMain

## tomcat starten 

````
## service file is at
/lib/systemd/system/tomcat9.service

## start tomcat with 
service tomcat9 start

##check status
service tomcat9 status
`````

## tomcat signin

http://localhost:8080/escra
user:
escra
pw:
escraadmin

## start project

go to client project and change environment
go to server project and change ngrok tunnel for connections

````
// This file can be replaced during build by using the `fileReplacements` array.
// `ng build --prod` replaces `environment.ts` with `environment.prod.ts`.
// The list of file replacements can be found in `angular.json`.
import {Environment} from './ienvironment';
// const ip = '192.168.2.129'
const ip = 'localhost'
const url ='http://' + ip;

export const env: Environment = {
`````

start server
```
node app.js
```

start client project
````
ng serve
````

## escra client sign in

http://localhost:4200/

user:  
escra   
pw:   
escraadmin 

same pw as guacamole server (tomcat)

++ authtoken

## Troubleshooting

error: Spalte »ip« von Relation »guacamole_history_user« existiert nicht

> create ip column in table guacamole_history_user


## Guacamole db 

### db user access
localhost
5432
escra_db
guacamole_user
guacamole_user

### db admin access
localhost
5432
escra_db
postgres
postgres





# TODO next


This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.1.5.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
