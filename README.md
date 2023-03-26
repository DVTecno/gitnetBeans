# gitnetBeans
## Un salito para todos
Ultima modificacion: 24-04-2023
Operacones logicas con operadores y conectores
EN ESTA UNIDAD ABODAREMOS LAS OPERACIONES LOGICAS DE UNA MANERA DISTINA YA QUE ES MUY IMPORTANTE ENTENDER EXACTAMENTE QUE SON Y COMO PODEMOS APLICARLAS, TRATAREMOS DE DAR EJEMPLOS COTIDIANOS Y TRATAR DE APLICAR UN POCO DE LOGICA PROPOSICIONAL, SOLO LO BASICO PARA ENTEDER LAS CONECTIVAS LOGICAS MAS QUE NADA!

COMENZAREMOS
OPERACIONES LOGICAS
Las operaciones logicas que mas usaremos son 4 y pueden se combiandas

Operador logico IGUAL ( == ): 
    En Java para comparar dos cosas se utiliza un doble igual, vamos con ejemplos comunes:
        rojo == azul , se traduce como ... el color rojo es igual al azul? obviamente es falso y por lo tanto el resulado de la operacion logica es FALSE;
        1 == 1, se tracude como... el numero 1 es igual a 1??? obviamente es verdadero por que esta hablando de 2 cosas que son iguales, y el resultado de la operacion logica es TRUE;
        1 == "1" se traduce como... el numero 1 es igual que el caracter/cadena 1??? hay cierta confusion aqui, por que los 2 representan el 1... pero SON OGUALES??? Si leemos bien el significado es obvio que es falso, el resultado de esta operacion logica es FALSE;    SE PREGUNTARAN POR QUE?  vamos a tratar de resumirlo y de que se entienda de la mejor manera... En programacion tenemos numeros y cadenas de texto como ya sabemos y se distiguen por tipos de variables, (lo que vimos en el notebook anterior), y los numeros se representan como 1,2,3,4,5,6,7,8,9,0 y las cadenas de caracteres va siempre entre comillas dobles, lo cual dice que eso son caracteres y no numeros... 1 <- es un uno numerico  "1"<- es la representacion del numero uno (caracter)... 

Operador logico MENOR QUE ( < ):
    Se utiliza para compara si el de la izquierda es menor que el de la derecha, vamos con ejemplos comunes:
    1 < 15 se traduce como... el numero 1 es menor que el numero 15??? como ya sabemos es obio que es verdadero, y por lo tanto el resultado es esta operacion logica es TRUE;
    14 < 5 se traduce como... el numero 14 es menor que el numero 5??? como ya sabemos es obio que es falso  , y por lo tanto el resultado es esta operacion logica es FALSE;
    "a" < "h" ... interesante te reto a probarlo primero y despues vemos que es lo que sucede, como por ejemplo "z" < "h" y muchas mas comparaciones entre caracteres... pero que sucede??? lo explicaremos al final del NOTEBOOK.

Operador logico MAYOR QUE ( > ):
Se utiliza para compara si el de la izquierda es mayor que el de la derecha, vamos con algunos ejemplos:
    15 > 7, como ya se es de esperar el resultado de esta operacion logica es TRUE;
    15 > 130 , el resultado de la operacion logica es FALSE;
    COMO EN EL CASO ANTERIOR TE TOCA HACER PRUEBAS CON "a" > "b" y muchas mas...

Operador logico DISTINTO ( != ) :
Se utiliza para hacer lo contrario del igual, lo que evalua que si los 2 elementos son distintos, vamos con ejemplos:
    7 != 2 , se lee como si el numero 7 es distinto al numero 2, como ya imaginamos esto es verdadero y por lo tanto el resultado de esta operacion logica es TRUE;
    9 != "9" , se lee como si el numero 9 es distinto al caracter "9", y como ya imaginamos  esto es verdadero, y por lo tanto el resultado de esta operacion logica es TRUE;
    "nombre" != "nombre", se lee como si la palabra nombre es distinta a la palabra nombre, como imaginamos es falso y el resultado de esta operacion es FALSE;

NOTA: los operadores logicos MENOR QUE (<) y MAYOR QUE (>) se pueden combinar con el operador logico IGUAL (==) de la siguente manera, 
<= que significa MENOR O IGUAL QUE
>= que significa MAYOR O IGUAL QUE

estas operaciones logicas las podemos combinar y hacer varias al mismo tiempo... pero eso lo veremos un rato mas ... por ahora comenzaremos con los condicionales.
System.out.println(" Operador Logico IGUAL QUE( == ) ");
System.out.println("\"rojo\" == \"azul\": " + ("rojo" == "azul") );
System.out.println("1 == 1: " + (1 == 1) );
System.out.println("1 == '1' : " + (1 == '1') );

System.out.println(" Operador Logico MENOR QUE( < ) ");
System.out.println("1 < 15: " + (1 < 15) );
System.out.println("14 < 5: " + (14 < 5) );
System.out.println("'a' < 'h' : " + ('a' < 'h') );

System.out.println(" Operador Logico MAYOR QUE( < ) ");
System.out.println("15 > 7: " + (15 > 7) );
System.out.println("15 >130: " + (15 > 130) );
System.out.println("'a' > 'b' : " + ('a' > 'b') );

System.out.println(" Operador Logico DISTINTO QUE( != ) ");
System.out.println("7 != 2: " + (7 != 2) );
System.out.println("9 != '9': " + (9 != '9') );
System.out.println("\"nombre\" != \"nombre\" : " + ("nombre" != "nombre") );

System.out.println("OPERADORES LOGICOS COMBINADOS (<= Y >=)\n");
 Operador Logico IGUAL QUE( == ) 
"rojo" == "azul": false
1 == 1: true
1 == '1' : false
 Operador Logico MENOR QUE( < ) 
1 < 15: true
14 < 5: false
'a' < 'h' : true
 Operador Logico MAYOR QUE( < ) 
15 > 7: true
15 >130: false
'a' > 'b' : false
 Operador Logico DISTINTO QUE( != ) 
7 != 2: true
9 != '9': true
"nombre" != "nombre" : false
RECUERDAN QUE DIJIMOS QUE IBAMOS A RETOMAR LOS OPERADORES LOGICOS?
Bueno es ahora... aparte de los operadores logicos tenemos Tenemos las CONECTIVAS LOGICAS que son la disyuncion y la conjuncion! Pero que son? como nos podria ayudar? AHORA LO VEREMOS MAS A DETALLE
En el campo de la Logica proposicional tenemos 2 conectivas logicas (AND y OR) lo que hace es unir 2 operaciones logicas y dependiendo de la conectiva devolver un resultado, SE QUE SUENA DIFICIL PERO QUE NO DECAIGA!
POR AHORA VAMOS A DEFINIR LAS CONECTIVAS Y DESPUES EXPLICAMOS CON MAS DETALLE COMO FUNCIONAN!

----------------Conector logico AND ( && ): -----------------------

    En java para representar el AND utilizamos este simbolo & 2 veces... y lo que significa es "y", ESPERA LO UNICO QUE SIGNIFICA ES ESO? Si es todo lo que significa pero es muy poderoso, muchos no saben manejarlo y se tienden a confundirse o perderse... ahora vamos por unos ejemplos:
    supongamos que tenemos una operacion logica como  4 < 3 ... y tengo otra operacion logica como 6 != "6"... y las quiero conectar para que solo SE EJECUTE UNA PARTE DEL CODIGO DONDE LAS 2 CONDICIONES SEAN VERDADERAS, bueno eso se hace con la conectiva logica AND( && ) entonces quedaria 4 < 3 && 6 != "6"... ESPERA, PERO NO ES FALSA LA PRIMERA CONDICION? exacto es FALSA la primera condicion ... vamos por un ejemplo donde las dos sean verdaderas...
    3 < 20 && 20 < 200 tenemos esa operacion logica... no son 2 distintas, es UNA SOLA OPERACION LOGICA ... las conectivas logicas solo operan con valores de verdad a diferencia de los operadores logicos... entonces como funciona?
    TRANQUILO QUE AHI VA!, Como que operan con valores logicos??? exacto solo operan con los 2 valores de verdad que conocemos ... TRUE y FALSE . Veamos entonces, si observamos (3 < 20 && 20 < 200) vamos a comenzar a trabajarlo
    3 < 20          &&          20 < 200
    (verdadero)     &&       (verdadero) = ((verdadero))
    la conectiva logica AND (&&) solo es TRUE cuando las 2 operaciones logicas que conecta son verdaderas. Ahora en caso de que una sea falsa o las 2 sean falsas el valor que retorna la conectiva logica es FALSE;

    Nos quedaria una TABLA DE VERDAD DE LA SIGUIENTE MANERA:
    VERDADERO && VERDADERO = VERDADERO
    FALSO && VERDADERO = FALSO
    VERDADERO && FALSO = FALSO
    FALSO && FALSO = FALSO

    No te quedo claro? tranquilo vamos a tratar de explicarlo con ejemplos reales! utilizados en la logica proposicional

----------------Conector logico OR ( || ): -------------------
