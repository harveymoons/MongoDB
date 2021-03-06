# MongoDB
- [Install](#install)
- [Command](#command)
- [Feature](#feature)
- [Constructor](#constructor)

- [Mongoose](#mongoose)
  
---

## Install
###### MacOS
```sh
brew update
brew tap mongodb/brew
brew install mongodb-community[@version]
brew services start mongodb-community[@version]
brew services stop mongodb-community[@version]
# if there is some error message
# type homebrew command 
brew doctor
```
  
###### Window/Linux
https://www.mongodb.com/download-center/community  
  
---
  
## Command
###### run database
```sh
mongod
# on installed directory (default)
mongo 
```
  
###### add system variable (on Window)  
```sh
# if you want to use this shell command wherever freely
# you must set-up environment variable path (on Window)
# [myPC] => mouse right click 
# [advanced system setup] click 
# [system variable(N)] click
# [system variable(S)] click
# (in list) select named 'Path'
# below [Edit(I)] click
# [New(N)] click
# "add" mongodb installed path
# ex) C:\Program Files\MongoDB\Server\4.2\bin
```
  
###### check version
```
mongo --version
```
  
---
  
## Feature 
###### copy
###### sharding
###### ObjectId
---
  
## Constructor
### DataBase > Collection > Document  
---  
  
## Mongoose
- mongoose is ODM(Object Data Modelling) Library based MongoDB  
  
###### install `mongoose` & `dotenv`
```sh
yarn add mongoose
yarn add dotenv # support to use .env file (set config variable)

# check installed libraries
yarn list [--depth=number]
```
  
###### create `.env` file on project root path & type info
```
PORT=4000
MONGO_URI=mongodb://localhost/test
```
###### not working for permission denied / refused
[Ref.] https://stackoverflow.com/questions/58034955/read-only-file-system-when-attempting-mkdir-data-db-on-mac
