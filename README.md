# docker-sbt

Docker image to use sbt, the Scala Build Tool, without need to install it.

# Usage

Run the following command to create an alias that allow you to use this Docker image in the same way than if the tool would be installed as usual.

```sh
alias sbt='docker run --rm -it -v $(pwd):/app -v /var/run/docker.sock:/var/run/docker.sock boxyware/sbt'
```

After that, just go to the *Scala* project folder and run the alias command:

```sh
sbt
```

>This image has set the working directory at ```/app```.