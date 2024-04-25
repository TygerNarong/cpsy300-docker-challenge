STEPS:
1.	Create a final assignment folder
2.	Create a challenge 3 folder
3.	Extract D2L challenge folder to challenge 3 folder
4.	Create a .env file containing your configuration variables
5.	Create a docker-compose.yml file
6.	Edit the api docker file to contain the following prompts 
#Copy package.json and package-lock.json 
COPY package*.json ./  
#Copy the rest of the application 
COPY . .
7.	Run the command docker-compose up
8.	To check your work 
When you request URL:
 “http://localhost:8080/api/books” you will get a JSON message with all books.
 “http://localhost:8080/api/books/1” you will get a JSON message with just one book.
