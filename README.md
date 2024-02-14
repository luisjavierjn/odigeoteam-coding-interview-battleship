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