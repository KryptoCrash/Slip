# Bin

## A bin is an object of more than 4096 properties.

## Declaration

Complete:

```
newBin = *{key1: prop1, key2: prop2... keyN: propN}
```

## Properties

### Length:

```
newBin.length
```

## Methods:

## Load

```
*newBin<> #*newBin< 0, newBin.length, 1, -> >
```

OR

```
*newBin<startIndex, endIndex, stepCount, callBack>
```

##Get (Must be loaded)

```
newBin.getByKey<key>
```

OR 

```
newBin.getByProp<prop>
```

OR

```
*newBin[index]
```
