# Getting Started with CSS Art!

# Cloning this GiHub Repo
You will need to clone this repo in order to have the base code required for the lesson.
```
git clone repo 
```
which will install Angular globally on your computer. To then check that it installed correctly, run
```
ng v
```

# Creating a New Project
We are now ready to create your local project! This can be done using this command:
```
ng new projectName --routing --style=scss
```
and will initialize a new project with routing (don't worry about this yet!) and the stylesheet will be SASS instead of CSS. SASS is basically css with a bunch of added utility on top of it. It doesn't need to be used, but is recommended.

Now you can check out your new website! Navigate to the file which you just created and run
```
ng serve -o
``` 
which will automatically open a new tab when the code is compiled and running of your new website!

Now we can install some Angular libraries which expand on the core functionality of Angular even more. Angular's animation library comes with some really cool animations that we will use as an example but will not be gone over in this lesson very much. To install this library, run this command:
```
npm install --save @angular/animations
```
Then, once installed successfully, it must be manually included in the /src/app/app.module.ts and imported by adding this line of code to the other imports at the top of the file:
```javascript
import { BrowserAnimationsModule } from '@angular/platform-browser/animations';
```
Then, in addition to this, inside the @NgModule section the name of the module, BrowserAnimationsModule, must also be added in the Imports section. This is a little confusing but order doesn't matter here and it can be imported in whatever order.

The app.component.html may now be edited to display whatever we want! Next, we will be utilizing routing to display another component's html on the site.

# Creating and Understanding Components
Components are one of Angular's key features that makes it effiecient and dynamic for easy workflow. A component, very simply, is a building block which an Angular website is built on, which as it grows turns into a web of components where for the most part, each component is a seperate element of a webpage. A page may contain many components, but ultimately a component should accomplish one goal - maybe to show a map on a site, display an about page, or a contact us form.
To create a component, run the following code:
```
ng generate component home
```
where home will be the component! Try creating another for an "about" page!

Now, we can show how that component works to better understand what these are and how they are used. Delete everything besides the router-outlet tags in the app.component.html file and add the new tag:
```html
<app-home></app-home>
```
This will directly link to the new home component that was just created and we can now see that the website will display the html inside the home.component.html inside the home file. You can run the server now (again using ```ng serve -o```) and see that the new site only displays "home works!" as its displaying the code from the home component! Cool!

# Let's Code!
Here I will be demonstrating how to put it all together with some cool techniques to show off some tools included with Angular!
Clone this repo to your local machine and follow along!

Be sure that after you clone the repo locally, you run
```
npm install
```
to install the needed packages for the provided project. Do not worry about any errors or issues, it should be ok!

To view the complete repository with the rest of the code, click [here](https://github.com/alexpritt/angularLessonComplete)!
\
