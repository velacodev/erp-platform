HolaMundo — Validador de contraseña con WinForms
Vista del LogIn

<img width="426" height="625" alt="image" src="https://github.com/user-attachments/assets/05a73213-f6ef-4f6e-92d0-30e8344fe66c" />

Aplicación de escritorio desarrollada en C# con Windows Forms que valida la estructura de una contraseña mediante una expresión regular (Regex) y comprueba que coincida con su confirmación.

Warm up: Crear un formulario simple con WinForms 
Profesora: Ma. Inés Calderón Zetter 
Alumno: Fernando Vela Covarrubias

Descripción

El formulario contiene dos campos de texto (contraseña y confirmación) y un botón. Al hacer clic en el botón se ejecutan dos validaciones en orden:

Estructura de la contraseña (Regex). Debe contener al menos:
Una letra mayúscula
Una letra minúscula
Un número
Un símbolo

Si ambas validaciones se cumplen, aparece un MessageBox con el mensaje "La contraseña ha sido validada". Si alguna falla, se muestra un mensaje indicando el motivo.


Requisitos
Windows 10 u 11
Visual Studio Community edition con la carga de trabajo Desarrollo de escritorio con .NET
.NET 18.10.3


Cómo ejecutarlo


Clona el repositorio:
bash
   git clone https://github.com/velacodev/HolaMundo.git
Abre el archivo HolaMundo.sln (o HolaMundo.csproj) con Visual Studio.
Presiona F5 o el botón Iniciar para compilar y ejecutar.




Escenario 1: la contraseña no cumple la regla
Entrada: contraseña “hola123” en ambos campos. Resultado esperado: MessageBox indicando que falta mayúscula y símbolo.

<img width="618" height="617" alt="image" src="https://github.com/user-attachments/assets/0f0a8b9d-0333-480a-b5fe-dad10df9859b" />










Escenario 2 El campo de información para el usuario esta vacío
Entrada: “        ” en el primer campo y “Hola#124” en el segundo. Resultado esperado: MessageBox con “Por favor ingrese un nombre de usuario y una contraseña.”



<img width="423" height="622" alt="image" src="https://github.com/user-attachments/assets/968ac839-a5f3-4def-9502-f1bf5a22c2a4" />









Escenario 3: validación exitosa
Entrada: “Contraseña777@” en ambos campos. Resultado esperado: MessageBox con “La contraseña ha sido validada”.



<img width="426" height="625" alt="image" src="https://github.com/user-attachments/assets/5b78236a-204e-4fc1-b574-775ef670a1f8" />







Autor
Ing Q. Fernando Vela Covarrubias — Maestría en Cómputo Aplicado, Universidad de Guadalajara





