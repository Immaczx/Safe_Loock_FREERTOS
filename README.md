# Safe_Loock_FREERTOS

La cerradura electronica permite abrir puertas sin necesidad de usar llaves. en lugar de llaves, puede elegir un pin y este cambiará cada vez que se abra la puerta permitiendo el su uso para varios usuarios a lo largo del tiempo.

La cerradura tiene una contraseña por defecto la cual debe ingresarse por medio el keypad por el usuario, luego al cerrarla debe ingresar una nueva contraseña la cual será guardada hasta que sea abierta nuevamente, si la contraseña ingresada corresponde a la guardada se abrirá la puerta pero si no corresponde la puerta permanecerá cerrada. También está integrada con un display 7 segmentos el cual muestra los dígitos ingresados por el usuario,  cuando estos dígitos coinciden con la contraseña muestra una letra A, o una F cuando los dígitos ingresados son erróneos y la letra E cuando almacena una nueva contraseña.

![Alt text](/Safe_Look_Diagram.png?raw=true "Safe Look Diagram") 

  "Figura 1. Diagrama de flujo de codigo general"

![Alt text](/Debouncing_Keypad.png?raw=true "Debouncing Keypad") 

  "Figura 2. Diagrama de flujo maquina de estados Debouncing Keypad"

![Alt text](/Keep_password.png?raw=true "Keep password") 

  "Figura 3. Diagrama de flujo maquina de estados Keep password"

En la siquiente figura se ve como al precionar un boton del keypad el display 7 segmentos muestra el numero presionado en este caso es en numero 2.


![Alt text](/Prest_keypad.jpeg?raw=true "Prest keypad") 

  "Figura 4. Montaje presioando tecla del keypad"

Al introducir los 4 numeros que coresponden al pin inmediatamente el display mostrara una A y el LED verde de la targeta nucleo se pondra en ON indicando que se abrio la cerradura. 


![Alt text](/Unloock.jpeg?raw=true "Unloock") 

  "Figura 5. Montaje pin correcto(cerradura abierta)"

Cuando los 4 numeros ingresados son diferentes al pin el display mostrara una F y la cerradura permanecera cerrada.


![Alt text](/loock.jpeg?raw=true "loock")

  "Figura 6. Montaje pin incorrecto(cerradura cerrada)"

Si la cerradura esta abierta y se introduce una combinación de 4 dígitos estos pasaran a ser el nuevo pin, el display mostrara una E y el LED pasara a OF indicando que la cerradura se a cerrado.


![Alt text](/Save_new_password.jpeg?raw=true "Save new password") 

  "Figura 7. Montaje guardando nuevo pin"
