# screen scripts

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

```
./topLeft echo "I am top Left Screen"

./topRight echo "I am top Left Screen"

./bottomRight top
```

## to stop runnung app:
```

./bottomRight ^C

./bottomLeft "ps -aux | grep screen"
```

## To send same command to all screens run:
```

./broadcast echo "test"
```

## To Quit without terminating screens:
Ctrl-A \ ==> y

## not tiled screens:
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



