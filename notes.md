# Analissa learning new things

## Terminal

- Format and display the on-line <span style="color:red">man</span>ual pages
  - man
- <span style="color:red">L</span>i<span style="color:red">s</span>t directory content
  - ls
- Return <span style="color:red">w</span>orking <span style="color:red">d</span>irectory name
  - pwd
- <span style="color:red">C</span>hange <span style="color:red">d</span>irectory. ___Remember___ one dot is current directory, two dots is out of current directory.
  - cd
- Con<span style="color:red">cat</span>enate and print files
  - cat
- Updates the timestamps on existing files and directories as well as to create new empty files.
  - touch
- <span style="color:red">M</span>a<span style="color:red">k</span>e <span style="color:red">dir</span>ectories
  - mkdir
- <span style="color:red">R</span>e<span style="color:red">m</span>ove files and directories. To remove directories use the -rf flag.
  - rm
- <span style="color:red">C</span>o<span style="color:red">p</span>y files. To include all its files and subdirectories, use the -r flag.
  - cp
- <span style="color:red">M</span>o<span color='red' style="color:red">v</span>e files.
  - mv
- <span style="color:red">Clear</span>s your screen if this is possible.
  - clear
- Allows you to run programs as another user, by default the root user. <span style="color:red">S</span>uper <span style="color:red">U</span>ser <span style="color:red">DO</span>.
  - sudo

#### Tips

- Use TAB button to autofill when typing.
- Ctrl + C stops any command that is currently working.
<br/>
----------------
<br/>

## Docker
<br>

### Docker commands
<br>

#### Build an image from a Dockerfile

```bash
docker build
```

#### Run a command in a running container

```bash
docker exec 
```

#### List images

```bash
docker images 
```

#### List containers. Use -a flag to list stopped containers.

```bash
docker ps
```

#### Pull an image or a repository from a registry

```bash
docker pull
```

#### Rename a container

```bash
docker rename
```

#### Restart one or more containers

```bash
docker restart
```

#### Remove one or more containers

```bash
docker rm
```


#### Remove one or more images

```bash
docker rmi
```

#### Run a command in a new container

```bash
docker run
```

#### Start one or more stopped containers

```bash
docker start
```

#### Stop one or more stopped containers

```bash
docker stop
```

-----------
<br>

### Docker pythonlisssa (without Docker compose)
<br>

#### Build an image from a Dockerfile located inside Docker folder, tagged it. Context is here (.) REMEMBER THE DOT

```bash
docker build -f ./Docker/Dockerfile -t pythonlissa .
```

#### Run container with pythonlissa image, attach current directory to /code and start sh

```bash
docker run -it -v ${PWD}:/code pythonlissa sh
```
