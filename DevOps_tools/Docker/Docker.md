# Docker

### What is Docker ?
- Docker is a very popular and powerful open source containeraization platform that is used for building, deploying and running applicaion/software from the user.

### How to build docker image

- Steps for building docker image

1) docker image

2) docker init 
   - This will create 4 files 
   A) .dockerignore
      - Reduces image size → unnecessary files (like .git or  node_modules) won’t bloat your image.

      - Improves build speed → fewer files = faster docker build.

      - Security → avoids accidentally copying sensitive files (like .env or credentials) into the image.

      - Cleaner layers → prevents clutter inside /usr/share/nginx/html or /app (depending on your base image).

      ##### Example for HTML/CSS/JavaScript project
    ` 
        # Ignore Git repo
        .git
        .gitignore

        # Ignore Docker config files
        Dockerfile
        .dockerignore

        # Ignore OS files
        .DS_Store
        Thumbs.db

        # Ignore docs
        README.md
        LICENSE

        # Ignore IDE/editor settings
        .vscode
        .idea
        *.swp
    `
    ##### Example for Node/React project
    `
        # Git
        .git
        .gitignore

        # Node modules (we’ll install fresh inside the container)
        node_modules

        # Logs
        npm-debug.log
        yarn-error.log

        # OS/Editor
        .DS_Store
        Thumbs.db
        .vscode
        .idea

        # Docker
        Dockerfile
        .dockerignore
    `

   B) compose.yaml
   `
    version: "3.8"

    services:
    web:
        build: .
        container_name: my-todo-app
        ports:
        - "8080:80"
        restart: unless-stopped
   `

    version: "3.8" → Compose file format version.
    services → web → defines your app (you could add more later).
    build: . → builds image from the Dockerfile in the current directory.
    container_name → gives your container a fixed name.
    ports → maps localhost:8080 → container port 80 (nginx default).
    restart: unless-stopped → auto-restarts unless you manually stop it.

    ` docker compose up -d `

   C) Dockerfile

` # 1) Use nginx base image 
    FROM nginx:alpine
    # 2) Set working directory (nginx serves from here)
    WORKDIR /usr/share/nginx/html
    # 3) Remove default nginx index page
    RUN rm -rf ./*
    # 4) Copy your HTML, CSS, JS files into the image
    COPY . .
    # 5) Expose port 80 (nginx default)
    EXPOSE 80
    # 6) Start nginx (default CMD from base image already runs it) `

    Build & Run (without Compose)
    # Build image
    docker build -t my-todo-app .

    # Run container
    docker run -d -p 8080:80 --name todo my-todo-app

   D) README.Docker.md

3) Build the image
   ` docker build -t my-todo-app:latest . `

4) Run the container
   ` docker run -d --name my-todo-app -p 8080:80 my-todo-app:latest `

5) Open your app
   ` http://localhost:8080 `

6) Update flow (When you change files)

    docker rm -f my-todo-app
    docker build -t my-todo-app:latest .
    docker run -d --name my-todo-app -p 8080:80 my-todo-app:latest
   

   