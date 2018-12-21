# Todoapp-Heroku
My Todo App Project on Angular With Firebase as Backend Deploy on Heroku Cloud......    

Deploying into Heroku wrote by sumit patil full stack developer:
======================

1. Goto heroku.com and create an account (Email & Password)

2. sudo snap install heroku --classic (Installing heroku CLI) inside the project

3. heroku --version (Check if the tool is installed properly)

4. heroku login (Provide your login credentials)

5. heroku create (It will automatically a project name). Check the URL. 

6. In the package.json make the following changes:

    a. Move @angular/compiler-cli and @angular/cli and typscript into Dependencies (From DevDependencies)
    b. Under the scripts section add "postinstall": "ng build --prod" && 
    "start" section with "node server.js"

7. In the server.js make "dist" as "dist/[project name]" (I M repo provide server.js express file in todoapp project)

8. Install Express (npm install express --save)

9. git add . 

10. git commit -m "Some comment"

11. git remote 

12. git push heroku master


Deploying into Github pages (Some issues are there):
=====================================================

git remote add origin https://github.com/WebstackAcademy/angular-deploy.git

Provide GIT username & password 

sudo npm i -g angular-cli-ghpages 

Provide sudo username & password 

ng build --prod --base-href="https://webstackacademy.github.io/angular-deploy/"
