## Building a Full Stack Polls app similar to twitter polls with Spring Boot, Spring Security, JWT, React and Ant Design

![App Screenshot](screenshot.png)

### Tutorials

I've written a complete tutorial series for this application on The CalliCoder Blog -

+ [Part 1: Bootstrapping the Project and creating the basic domain models and repositories](https://www.callicoder.com/spring-boot-spring-security-jwt-mysql-react-app-part-1/)

+ [Part 2: Configuring Spring Security along with JWT authentication and Building Rest APIs for Login and SignUp](https://www.callicoder.com/spring-boot-spring-security-jwt-mysql-react-app-part-2/)

+ [Part 3: Building Rest APIs for creating Polls, voting for a choice in a Poll, retrieving user profile etc](https://www.callicoder.com/spring-boot-spring-security-jwt-mysql-react-app-part-3/)

+ [Part 4: Building the front-end using React and Ant Design](https://www.callicoder.com/spring-boot-spring-security-jwt-mysql-react-app-part-4/)

## Steps to Setup the Spring Boot Server

1. **Clone the application**

	```bash
	git clone https://github.com/kyliel/microservice-polls
	cd microservice-polls
	```


3. **Set MySQL hostname and password as per your MySQL installation**

	+ set `MYSQL_HOST` and `MYSQL_PASSWORD` environment variables as per your mysql installation(the username is `root`), see see `poll-app-web/src/main/resources/application.yaml` file for details.
	

4. **Run the app**

	You can run the spring boot app by typing the following command -

	```bash
	mvn install
    cd poll-app-web
	mvn spring-boot:run
	```

	The server will start on port 5000. The spring boot app includes the front end build also, so you'll be able to access the complete application on `http://localhost:5000`.

	You can also package the application in the form of a `jar` file and then run it like so -

	```bash
	mvn package
	java -jar poll-app-web/target/poll-app-web-0.1.0.jar
	```
