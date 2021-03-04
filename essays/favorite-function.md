# funções favoritas



member -> simples, 2 linhas, declarativa, recursiva, funcional

bônus: statically typed, mas polimórfica parametricamente AND com  type inferecence

```c#
fun member(xs, s) = 
	not(null xs) andalso (hd xs=s orelse member(tl xs,s)
```



Finite State Machine with 2 states

Dizer se a lista faz alternado [1,2,1,2] e se termina em 2. Devolve true or false



**Com açucar**

```c#
fun fsm(xs) = 
    let 
        fun state_1(xs) = 
            case xs of
                [] =>true
            | 1::xs' => state_2(xs')
            |  _ => false
        and state_2(xs) = 
            case xs of
                [] => false
            | 2::xs' => state_1(xs')
            | _ => false
        
    in
        state_1(xs)
    end
```





**Sem açucar**



```c#
fun fsm1(xs, f) = 

    case xs of

       [] => true

    | 1::xs' => f (xs')
    |   _    => false

    

fun fsm2(xs) = 

    case xs of

       [] => false

    | 2::xs' => fsm1 (xs', fsm2)

    |   _    => false
```

