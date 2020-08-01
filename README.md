# docker-practice
Experiments with docker and examples of working with it.

# Get started
For working with Docker, you need to install it.
```
brew install docker
brew cask install docker
```

For check docker version enter `--version`.
```
docker --version
```

For run containers need to install virtual machine, 
for example on MacOS X may to install `docker-machine` as brew service.
```
brew cask install docker-machine
```

After you can to display all brew services.
```
brew services list
```

A list of all brew services was displayed.
```
Name              Status  User  Plist
docker-machine    stopped
```

Now, the `docker-machine` service is stopped by default. For running enter following command.
```
brew services start docker-machine
```

After need to create a new virtual machine by the name `default` for docker.
```
docker-machine create --driver virtualbox default
```

Configure enviroments as the `default` virtual machine.
eval "$(docker-machine env default)"

So, then you can work with docker. Congratulations!
