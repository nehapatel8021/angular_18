# angular_18
Install Node js and npm 
->Then install Angular using the command: npm install -g @angular/cli
->check whether it is intalled or not using: ng v
->Then create the project using: ng new angular_tutorial
-> to run the project: npm start OR ng serve, it will shows us the URL and click on it and it will open up the application in web browser
-> to stop your application from running, in your terminal press "Ctrl + C" and it will stop your application from running in the browser.

Explaination of package.json file:
->dependencies: contain all the packages which are the part of your build process
->devdependencies: contain all the packages which are only available locally for the use, these packages are not the part of your build process. 

=>Whenever the Angular application starts main.ts file is executed first.
=>When we load the application why AppComponent is getting load first? : Answer: Because we have defined it in our "main.ts" file, when we are boostraping the application. We can check the main.ts file where you can find that bootstrapApplication() fucntion, first argument is AppComponent.

Components:

=> How many files are required in Component?: Answer: If we have only .ts file then also its fine, but .ts file is necessary for components.
->Create Component using Angular CLI: ng g c component_name   OR ng generate component component_name . This command will automatically generate all the necessarry files required for it, html file,css file, ts file
->@Component decorator we have selector property: we can say it as a Unique Id for particular component. we can use that selector property value as a class to call that component. Example: we have selector: app-add-employee . Then if you want this AddEmployee Component in other components then in that other components's .ts file add <app-add-employee></app-add-employee>.
