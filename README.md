# WordDictionary
Dictionary of your own words
########## PROJECT INFO #####################################################
* The Working Repository for the Project is called "WordDictionary".
* Server side scripting is done in Java using Spring Boot Framework.
* Client Side scripting(User Interface) is done using JSX using React Js.
* Database used is MYSql db.
#############################################################################

########## How to Run #######################################################
1. Import the project WordDictionary in your IDE.
2. Make changes as per your choice of database in application.properties.
3. Build the maven project and run it using .jar file from target folder or if you are using Eclipse you can Run WordDictionary.class as Java application. Default port is 9393
4. The UserInterface is in folder "app-ui".
5. You need NodeJs inorder to run UI. Please install NodeJs.
6. 'node-modules' folder is not there as the size of the project becomes more than 25MB. Please install all the dependencies in package.json.
6. Go inside folder app-ui. Open command Prompt and run "npm start".
7. The Application will start at http://localhost:3000/home.

Note: If you change the server.port = newPort in application.properties then please make the appropriate changes inside "./app-ui/package.json" -> 'proxy': "http://localhost:newPort"

########## API INFO ######################################################################
The application has 3 API points:
* /api/upload(method=POST) : It uses a file as Request Parameter to read the file and then to                              store unique words in database.
* /api/dictionary(method=GET): It is used to get all the words in the database
* /api/search/word(method=GET): Uses Path varialble to search the word in the database.

Note: Swagger2 has been implemented in the Spring Boot project if you want to try out api functionality without using the UI
###########################################################################################

########## UI INFO ########################################################################
* The UI has 2 routing pages for the 2 components
1. Home(ShabKosh) : You can upload your text file using the Upload feature. This page also 		    displays all the words in the dictionary.
2. ShabdKhoj: This page can be used to search a word in the dictionary.
########################################################################################### 
