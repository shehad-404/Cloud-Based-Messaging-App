# Messenger

A one-to-one realtime chat app. 

# System Architecture
<img width="1348" height="898" alt="image" src="https://github.com/user-attachments/assets/a329c4b8-6f21-418e-863c-2b9b4a7d3e89" />



# Technologies
- React
- MaterialUI
- SocketIO
- Redux
- NodeJS
- Postgres
- Docker 
  
# Functionalities
- Authentification with CSRF protection and Session Cookie
- Real time chat with SocketIO
- Nice UI with MaterialUI
- Containerized application with docker
- Login/Registration system
- Notification system
- Search user


# Screenshots

### Login page
![](/screenshot/login-page.png)
### Account Creation page
![](/screenshot/logout-page.png)
### Chat page
![](/screenshot/message.png)
## Running Application Locally

### Requirement:
- [Docker](https://docs.docker.com/get-docker/)

At the root of the folder, run the following command:
```
docker-compose up -d
```

Create a .env file in the root folder and add your session secret, sql credentials and url as follow:

```
# SERVER VARIABLES
DATABASE_URL= postgres://user:pass@postgres:5432/messenger
NODE_ENV= development
SESSION_SECRET= "your session secret"

# Allow hot reloading in container
CHOKIDAR_USEPOLLING= "true"

#POSTGRES Variables
POSTGRES_USER= user
POSTGRES_PASSWORD= pass
POSTGRES_DB= messenger

```


You access the react app at: `http://localhost:3000`
And the server at: `http://localhost:3001`
