# screen scripts

![Alt text](screen.png?raw=true "screen")

## enable path:
```
source setup-env
```
## Start 4 screens tiled:
```
mscreen
```
## To switch screens:
Ctrl-A tab

## To go back previous screen:

F8


## To Quit without terminating screens:
Ctrl-A \ ==> y

## not tiled (Full) screens:
```
m2screen
```

## in m2screen switch screens:

F5 backward

F6 forward

## Different layouts:
```
m3screen
or
screen4K
```

# Running shell commands in remote shell

With following commands any shell command could run on specified screen.

Using ssh, shell commands also could be run on remote computer:

screen terminals on one computer, screenSend command scripts on anohter.

## Send commands to screens:
```
./topLeft echo "I am top Left Screen"

./topRight echo "I am top Right Screen"

./bottomRight top

./bottomLeft "ps -aux | grep screen"
```

## to stop a running app:
```
./bottomRight ^C
```
## To send same command to all screens run:
```
./broadcast clear
./broadcast echo "test"
```
