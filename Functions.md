# Functions

## Declaration

### Complete:

functionName = <arg1, arg2... argN> <- {

}

### No args:

functionName = <- {

}

### Anonymous:

<arg1, arg2... argN> <- {

}

### One-liner:

functionName = <arg1, arg2... argN> <- #code goes here

### Callback:

functionName = <functionName> <- functionName ->

### Closure:

functionName = <arg1> <- <arg2> <- arg1 + arg2;

OR

makeCounter = <- {
  privateCounter = 0;
  changeBy = <val> <- privateCounter += val;
  {
    increment = <- changeBy(1);
    decrement = <- changeBy(-1);
    value = <- privateCounter;
  };
};



## Call

### Complete:

functionName<args> -> <args>

### Normal:

functionName<args> ->

### No arguments:

functionName ->

### Repetitive Function Calls:

fn1 -> fn2<arg1> -> fn3 -> fn4<arg1+arg2> ->

### Return value as argument for function declaration:

fn2 = < fn1<args> -> > <- #Code goes here

OR:

fn1 ->:<-

### Anonymous calls:

publicvar = 'test'
fn1 = <- {
publicvar;
}
publicvar; #returns 'test'
fn1 ~>; #returns undefined
