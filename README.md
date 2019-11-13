# New Macbook Setup
Have you ever wondered to have summary of scripts to setup in your new Macbook for Java/ Javascript Developer point of view.

I've run through these common Installation Scripts everytime, whenever I need to setup a new macbook. Thought these could help any beginners who are using for the first time or who just want to quickly setup their machine.


I love to start with brew.

## Brew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
Just update once, to get later software versions
```
brew update
```

## Git
```
brew install git
```


## Java 8
```
brew tap adoptopenjdk/openjdk
brew cask install adoptopenjdk8
```

```
java -version
```

## Build Tools (Maven & Grade)
```
brew install maven
```

```
mvn -v
```

```
brew install gradle
```

```
gradle -v
```

## Quick Downloads (.dmg)
- Chrome
- IntelliJ
- Docker

## Dockerizing (From Local Machine)
- Create a Bootable Jar
```
git clone https://github.com/whyaneel/book-a-meeting-room.git
cd book-a-meeting-room
```

```
./gradlew clean build
```

- Create a Docker Image (from Dockerfile)
```
docker build --no-cache -t book-a-meeting-room-app .
```

- Run The Application
```
docker run -p 9000:8080 book-a-meeting-room-app
```
This Application Should be Running at http://localhost:9000/



## SHOW Hidden Files
```
defaults write com.apple.finder AppleShowAllFiles YES
```

