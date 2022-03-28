# Tipo de datos primitivo 

Al inicaiar la practica no me salia toda la ayuda para el comando asi que hice un "update-help" que tambien creo un error por que se tenian que aztualizar los parametros del idioma lo cual se soluciona introduciendo "Update-Help -Verbose -Force -ErrorAction -SilentlyContinue", aun que despues de introducir lo anterior salga un error los comandos de "get-help" ya funcionan al completo.

Al empezar salia muy poca o ninfuna informacion:
![image](https://user-images.githubusercontent.com/91567318/160452045-89398108-bda8-40c7-b10e-59cb0b7d2cac.png)

El resultado de toda la informacion despues del "Update-Help -Verbose -Force -ErrorAction -SilentlyContinue":
![image](https://user-images.githubusercontent.com/91567318/160465826-b7f88191-172d-49c0-ba71-36c3f51cecc8.png)


## Tarea 1 Use "Get-Help" para obtener más información sobre 5 cmdlets.  Como ejemplo, puede usar "Get-Service" o "Out-GridView".

· Get-Help Get-Help

· Get-Help New-Item 

![image](https://user-images.githubusercontent.com/91567318/160465839-3a172ac4-c53f-4977-855d-c1d21566df85.png)

· Get-Help Get-Alias

· Get-Help Get-AuthenticodeSignature 

· Get-Help Get-ControlPanelItem 

---

## Tarea 2 

Use "Get-Help" con el parámetro "–Example" para los 5 cmdletsmás en la tarea 1. 
 
· Get-Help Get-Help -Examples

· Get-Help New-Item -Examples

· Get-Help Get-Alias -Examples

· Get-Help Get-AuthenticodeSignature -Examples

· Get-Help Get-ControlPanelItem -Examples 

---

## Tarea 3 
Cree un nuevo archivo de texto llamado "TestFile. txt” en C:\ Maximo\PowerShell\Workshop1\%USERNAME%, El cmdlet para crear un archivo y un nuevo directorio comienza con “Nuevo”.

· New-Item -Path C:\ -Name Expo -ItemType Directory

· New-Item -Path C:\Sudoblark -Name PowerShell -ItemType Directory

· New-Item -Path C:\Sudoblark\PowerShell -Name Workshop1 -ItemType Directory

· New-Item -Path C:\Sudoblark\PowerShell\Workshop1 -Name bclark -ItemType Directory

· New-Item -Path C:\Sudoblark\PowerShell\Workshop1\bclark\ -Name Testfile.txt -ItemType File

---

## Tarea 4 
el archivo de texto que creó en la tarea 3 con los tres tipos de datos que hemos cubierto: "Booleano", " String” e “Int” El cmdlet que necesita comienza con “Add”.

· Add-Content -Path C:\Sudoblark\PowerShell\Workshop1\bclark\Testfile.txt -Value True Agregar contenido -Ruta C:\Sudoblark\PowerShell\Workshop1\bclark\Testfile.txt -Valor " Hola" Agregar contenido -Ruta C:\Sudoblark\PowerShell\Workshop1\bclark\Testfile.txt -Valor 42 

---

## Tarea 5 
Leer de el archivo de texto y use "Get-Member" para encontrar el tipo de datos devuelto , El cmdlet que necesita para leer los datos del archivo de texto comienza a "Obtener".

· Get-Content -Path C:\Sudoblark\PowerShell\Workshop1\bclark\Testfile .txt | Get-Member

---

## Task 6 
Sobrescriba todos los datos dentro del archivo de texto que creó en la tarea 3. 
El cmdlet que necesita comienza con "Set".

· Set-Content -Path C:\Sudoblark\PowerShell\Workshop1\bclark\Testfile.txt - Valor "Boooooo"

---

## Tarea 7 
formato a los datos devueltos por un cmdlet en una lista, Deberá canalizar el cmdlet original y luego usar el cmdlet "Format-List".

· Get-Service | Format-List

---

## Task 8 
Canalice "Get-Command" en "Out-GridView". 

· Get-Command | Out-GridView

---

## Task 9 
Canalice los 5 cmdlets que descubrió en la tarea 1 en "Out GridView". 

· Get-Help | Out-GridView 

· Artículo nuevo | Out-GridView 

---
