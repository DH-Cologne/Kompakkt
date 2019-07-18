# Installation

## Debian 10

Install dependencies
```apt install -y nodejs npm docker```

Update submodules
```git submodule update --init --recursive```

# Building

```cd Kompakkt.Viewer && npm install && npm run build```
```cd Kompakkt.Repo && npm install && npm run build```
```cd Kompakkt.Server && npm install && npm run build```

# Running

Boot MongoDB with docker
```docker run --name mongodb -p 27017:27017 mongo:latest```
Alternative: if you want to have the database files available on host system do
```docker run --name mongodb -v /path/on/host:/data/db -p 27017:27017 mongo:latest```

