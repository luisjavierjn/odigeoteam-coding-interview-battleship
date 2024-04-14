# Battleship

## Build

```
mvn clean package
```

## Docker network creation

```
docker network create battleship_net
```

## Run

```
docker-compose up --build
```

## Postman
[Postman project](docs/postman)


## Questions
https://docs.google.com/document/d/1OrLbOfF9ChirErVKXggWPrMjJG39I_e26lCmfT6r6gM/edit#heading=h.3b8675kpdnfp

## Notes

luisj@LBE-LNX-00383:~/odigeoteam-coding-interview-battleship/battleship-api$ mvn clean package install:install-file -Dfile=target/battleship-api-1.0.0-SNAPSHOT.jar -DgroupId=com.odigeo.interview.coding -DartifactId=battleship-api -Dversion=1.0.0-SNAPSHOT -Dpackaging=jar  

luisj@LBE-LNX-00383:~/odigeoteam-coding-interview-battleship$ mvn clean package  

---

luisj@LBE-LNX-00383:~/odigeoteam-coding-interview-battleship$ docker rm $(docker ps -a -q)  

luisj@LBE-LNX-00383:~/odigeoteam-coding-interview-battleship$ docker rmi odigeoteam-coding-interview-battleship-battleship_service:latest  

luisj@LBE-LNX-00383:~/odigeoteam-coding-interview-battleship$ docker rmi odigeoteam-coding-interview-battleship-battleship_computer_service:latest  

---

docker-compose up -d  

docker-compose logs -f  

docker-compose stop  

---

During this interview we will ask you to perform some coding activities in Java. So please for the day of the interview we will kindly ask you to have the following installed.  

- JDK min 8
- Maven 3.6.x (see https://maven.apache.org/download.cgi )
- Docker (optional) - https://www.docker.com/products/docker-desktop (you should be able to execute “docker run hello-world”)  

You can download from the following link the maven project and the problem description that we will use during a part of tomorrow's interview, in order to assess your coding skills.  

Feel free to take a look at it, and ensure that you can import it in your favorite IDE, compile it and run it.  

---

Dear Luis,  

the exercise is already coded, you can download the zip file I shared with you, which contains the project that should build and run without any modifications. We don't expect you to do any coding prior to the interview.  
It is however advantageous if you can spend some time to understand the problem description and discover the codebase we provided. Before the interview, we only expect that you import it in an IDE, are able to build it and are able to run unit tests on your computer, so we don't lose time to this activity during the interview.  