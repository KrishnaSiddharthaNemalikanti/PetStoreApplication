# PetStoreApplication
## petStoreUI
# Steps to Run the App:

* Open the terminal on the petStoreUI Folder
* Run npm install
* Run npm i webpack-dev-server --save-dev(this will install webpack dev server which has hot reloading)
* Run npm start ,this will open the application in browser.












# DB Structure
* I have used a sql type database and used .sqlite library to create the database.
* my data design consisted of one single tabe with 8 fields,ID contains a unique random value. 
* CREATE TABLE ANIMAL (id char(36) default (lower(hex(randomblob(4))) || '-' || lower(hex(randomblob(2))) || '-4' || substr(lower(hex(randomblob(2))),2) || '-' || substr('89ab',abs(random()) % 4 + 1, 1) || substr(lower(hex(randomblob(2))),2) || '-' || lower(hex(randomblob(6)))), location INT, name varchar(36), animal varchar(36), breed varchar(36), age INT, picture blob, description varchar(256));
