# Belatrix Connect Web Application

Install NodeJS, Bower, GulpJS

then install

npm install -g bower-installer

execute

- From the terminal in the same directory as your bower.json file, enter:

bower-installer

finally use:

gulp server

## Using docker (WIP)

Build the image
```docker build -t webimageallstarts:0.01 .```

Run the container
```docker run -d --name=weballstars -v `$pwd`:/home/app -p 3000:3000 webimageallstarts:0.01```

Install npm packages and bower dependencies
```docker exec -ti weballstars /bin/bash
```npm install && bower install --config.interactive=false --allow-root
