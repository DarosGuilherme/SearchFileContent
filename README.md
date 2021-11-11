The project was developed using Mulesoft Anypoint Plataform. You cannot run the project without the Licensed Runtime from the Mulesoft, or without the Anypoint Studio.
You can download the Anypoint Studio in this website
https://www.mulesoft.com/lp/dl/studio
After the installation of the Anypoint Studio, import the project in your current workspace:
 
After the import, you can run the project locally
 
After that, you can use the Console of the application, or run it in the Postman.

Console: http://localhost:8081/console/#docs/method/#3
Run the Method GET of the api/search url
In the Path, input the path of the folder in your environment: You can use any directory
In the Search, input the words that you want to search inside the files.

Postman:
Run the GET query:
http://localhost:8081/api/search?path=C%3A%5CfolderTexts&search=No+words+found+quantity+online
Where the queryParameter path is the folder in your environment and the queryParameter search is the words that you want to search inside the files.

NOTE:
The word is Case Sensitive. Word/word are different.

Problems that I found but could no resolve in 2-3 hours:
1 – You don’t need to find the exact word in the fileContent, for example, if the file content is “My name is Guilherme”, and you search for Gui, I will find the word and score as 100%
2 – It will not work with \t (enter) in the queryParameter. It split by “ ”
