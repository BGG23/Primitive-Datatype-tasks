# Tipo de datos primitivo 

Al iniciar la practica no me salia toda la ayuda para el comando así que hice un `Update-Help` que también creo un error por que se tenían que actualizar los parámetros del idioma lo cual se soluciona introduciendo `Update-Help -Verbose -Force -ErrorAction -SilentlyContinue`, aun que después de introducir lo anterior ssaldra un error volvemos a introducir un `Get-Help` el que sea y ya funcionan al completo.

Al empezar salia muy poca o ninguna información:

![image](https://user-images.githubusercontent.com/91567318/160452045-89398108-bda8-40c7-b10e-59cb0b7d2cac.png)

El resultado de toda la información después del `Update-Help -Verbose -Force -ErrorAction -SilentlyContinue`:

![image](https://user-images.githubusercontent.com/91567318/160465826-b7f88191-172d-49c0-ba71-36c3f51cecc8.png)


## Tarea 1 Use "Get-Help" para obtener más información sobre 5 cmdlets.  

· Get-Help Get-Help

![image](https://user-images.githubusercontent.com/91567318/160466135-d97b4584-d6a7-4493-85ef-2b838fc050a3.png)

· Get-Help New-Item 

![image](https://user-images.githubusercontent.com/91567318/160465839-3a172ac4-c53f-4977-855d-c1d21566df85.png)

· Get-Help Get-Alias

![image](https://user-images.githubusercontent.com/91567318/160466382-a50ca6ae-80c2-4aa8-a7a5-31be962143f4.png)

· Get-Help Get-AuthenticodeSignature

![image](https://user-images.githubusercontent.com/91567318/160466589-8835e607-ba61-4060-ad67-6fe6ddf67f29.png)

· Get-Help Get-ControlPanelItem

![image](https://user-images.githubusercontent.com/91567318/160466711-d19f7a17-522a-4fca-9eb7-359a51b4141c.png)

---

## Tarea 2 

Use "Get-Help" con el parámetro "–Example" para los 5 cmdletsmás en la tarea 1. 
 
· Get-Help Get-Help -Examples

![image](https://user-images.githubusercontent.com/91567318/160467291-ee56ae6b-63c5-427d-9796-e569a22e3573.png)

· Get-Help New-Item -Examples

![image](https://user-images.githubusercontent.com/91567318/160467487-0fb1c8c3-3538-4aca-937a-9b974052141d.png)

· Get-Help Get-Alias -Examples

![image](https://user-images.githubusercontent.com/91567318/160467635-5cabe205-62af-4e10-93cb-32827303fd97.png)

· Get-Help Get-AuthenticodeSignature -Examples

![image](https://user-images.githubusercontent.com/91567318/160467709-b84e0de7-3028-4e3b-9bbb-f163c88f1a5c.png)

· Get-Help Get-ControlPanelItem -Examples

![image](https://user-images.githubusercontent.com/91567318/160467793-874af37e-e6e4-4f8b-91b3-2218e18cbe58.png)

---

## Tarea 3 
Cree un nuevo archivo de texto llamado "TestFile. txt” en C:\ Maximo\PowerShell\Workshop1\%USERNAME%, El cmdlet para crear un archivo y un nuevo directorio comienza con “Nuevo”.

md C:\Maximo\PowerShell\Workshop1\jordiop | New-item -Path C:\Maximo\PowerShell\Workshop1\jordiop -Name Testfile.txt -ItemType File

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
