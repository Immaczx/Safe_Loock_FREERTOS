# Safe_Loock_FREERTOS

La cerradura electronica permite abrir puertas sin necesidad de usar llaves. en lugar de llaves, puede elegir un pin y este cambiará cada vez que se abra la puerta permitiendo el su uso para varios usuarios a lo largo del tiempo.

La cerradura tiene una contraseña por defecto la cual debe ingresarse por medio el keypad por el usuario, luego al cerrarla debe ingresar una nueva contraseña la cual será guardada hasta que sea abierta nuevamente, si la contraseña ingresada corresponde a la guardada se abrirá la puerta pero si no corresponde la puerta permanecerá cerrada. También está integrada con un display 7 segmentos el cual muestra los dígitos ingresados por el usuario, muestra una letra A cuando   estos dígitos coinciden con la contraseña, una F para cuando los dígitos ingresados son erróneos y la letra E cuando almacena una nueva contraceña.

![Alt text](/Safe_Look_Diagram.png?raw=true "Safe Look Diagram") 

![Alt text](/Debouncing_Keypad.png?raw=true "Debouncing Keypad") 

![Alt text](/Keep_password.png?raw=true "Keep password") 
En la siquiente figura se ve como al precionar un boton del keypad el display 7 segmentos muestra el numero presionado en este caso es en numero 2.
![Alt text](/Prest_keypad.jpeg?raw=true "Prest keypad") 
Al introducir los 4 numeros que coresponden al pin inmediatamente el display mostrara una A y el LED verde de la targeta nucleo se pondra en ON indicando que se abrio la cerradura. 
![Alt text](/Unloock.jpeg?raw=true "Unloock") 
Cuando los 4 numeros ingresados son diferentes al pin el display mostrara una F y la cerradura permanecera cerrada.
![Alt text](/loock.jpeg.png?raw=true "loock")
Si la cerradura esta abierta y se introduce una combinacion de 4 numeros estos pasaran a ser el nuevo pin, el display muestrara una E y el LED pasara a OF indicando que la cerradura de a cerrado.
![Alt text](/Save_new_password.jpeg?raw=true "Save new password") 
