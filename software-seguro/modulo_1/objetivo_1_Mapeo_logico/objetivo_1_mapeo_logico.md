<img width="1180" height="441" alt="screenshot-2026-10-17_00-14-26" src="https://github.com/user-attachments/assets/269f47f7-112a-4cf9-8cfc-63a519113bfd" />

## Turnero

Analizando la pagina de turnos medicos, el flugo para enviar un dato, especificamente en el login con usuario y contraseña.
El usuario cuando interactua con el frontend y envia los datos, estos inmediatamente se transmiten por el protocolo HTTPs, el cual cifra el contenido
de los mensajes, portegiendo de atacantes que esten escuchando o de un man in the middle. 

Cuando llegan al servidor valida el certificado del protocolo y recupera los datos encriptados para luego corroborar si existe en la DB
Si no existe el servidor emite un codigo 404 indicando que no existe el recurso, deneagando el acceso. Si existe el servidor emite un codigo 200, el cual
indica que se proceso con exito y el servidor le da acceso al usuario. Ademas se ejecutan metodos GET solicitando los turnos del usuario y el html para mostrar 
la nueva pagina. Todos los request y response entre el servidor y el cliente son por medio del protocolo HTTPs.


<img width="920" height="82" alt="imagen" src="https://github.com/user-attachments/assets/0442d848-02fe-4ea8-89ec-629127675fa8" />


