# mysqlworkbench
MySQL workbench in a docker image

## Usage

```
docker run -d \
     --net host \
     -v /tmp/.X11-unix:/tmp/.X11-unix \
     -v $HOME/.Xauthority:/root/.Xauthority \
     -e DISPLAY=$DISPLAY \ 
     yogeek/mysqlworkbench \
     mysql-workbench
```

## Troubleshooting

If the GUI does not show up, try to execute the following command before launching the docker container :
```
xhost +
```

