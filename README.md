# Tipo de datos primitivo 

Al iniciar la practica no me salia toda la ayuda para el comando así que hice un `Update-Help` que también creo un error por que se tenían que actualizar los parámetros del idioma lo cual se soluciona introduciendo `Update-Help -Verbose -Force -ErrorAction -SilentlyContinue`, aun que después de introducir lo anterior ssaldra un error volvemos a introducir un `Get-Help` el que sea y ya funcionan al completo.

Al empezar salia muy poca o ninguna información:

![image](https://user-images.githubusercontent.com/91567318/160452045-89398108-bda8-40c7-b10e-59cb0b7d2cac.png)

El resultado de toda la información después del `Update-Help -Verbose -Force -ErrorAction -SilentlyContinue`:

![image](https://user-images.githubusercontent.com/91567318/160465826-b7f88191-172d-49c0-ba71-36c3f51cecc8.png)


## Tarea 1 
### Use "Get-Help" para obtener más información sobre 5 cmdlets.  

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
### Use "Get-Help" con el parámetro "–Example" para los 5 cmdletsmás en la tarea 1. 
 
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
### Cree un nuevo archivo de texto llamado "TestFile. txt” en C:\ Maximo\PowerShell\Workshop1\%USERNAME%.

·`md C:\Maximo\PowerShell\Workshop1\Belén`

·`cd C:\Maximo\PowerShell\Workshop1\Belén`

·`New-item -Path C:\Maximo\PowerShell\Workshop1\Belén -Name Testfile.txt -ItemType File`

![image](https://user-images.githubusercontent.com/91567318/160489024-96b83f08-da9e-4953-ad6b-3dd6ec2846b9.png)

---

## Tarea 4 
### El archivo de texto que creó en la tarea 3 con los tres tipos de datos que hemos cubierto: "Booleano", " String” e “Int” El cmdlet que necesita comienza con “Add”.

![image](https://user-images.githubusercontent.com/91567318/160490133-1d8a4394-b8cf-4195-9f18-820e28cca41f.png)

---

## Tarea 5 
### Leer de el archivo de texto y use "Get-Member" para encontrar el tipo de datos devuelto , El cmdlet que necesita para leer los datos del archivo de texto comienza a "Get".

· `Get-Content -Path C:\Maximo\PowerShell\Workshop1\Belén\Testfile.txt | Get-Member`

![image](https://user-images.githubusercontent.com/91567318/160490434-d62405a6-901a-4582-b6a3-a09b5ac23749.png)

---

## Task 6 
### Sobrescriba todos los datos dentro del archivo de texto que creó en la tarea 3. El cmdlet que necesita comienza con "Set".

· `Set-Content -Path C:\Maximo\PowerShell\Workshop1\Belén\Testfile.txt - Valor "Boooooo"`

![image](https://user-images.githubusercontent.com/91567318/160491962-0239ea70-c9b8-4131-a013-fbc85b57ca27.png)

---

## Tarea 7 
### Formato a los datos devueltos por un cmdlet en una lista, Deberá canalizar el cmdlet original y luego usar el cmdlet "Format-List".

· `Get-Service | Format-List`

![image](https://user-images.githubusercontent.com/91567318/160494992-e4fa9f5d-a4b0-4aab-a675-de265f3cfae8.png)

---

## Task 8 
### Canalice "Get-Command" en "Out-GridView". 

· Get-Command | Out-GridView

![image](https://user-images.githubusercontent.com/91567318/160492384-cfef58f8-7307-4b92-b1f3-0fad9a9ebc2c.png)

---

## Task 9 
### Canalice los 5 cmdlets que descubrió en la tarea 1 en "Out GridView". 

· Get-Help Get-Help | Out GridView

![image](https://user-images.githubusercontent.com/91567318/160493795-a4f6ae3d-4faf-4d9a-953d-417a6dd946c1.png)

· Get-Help New-Item | Out GridView

![image](https://user-images.githubusercontent.com/91567318/160494316-baf4ecf6-e173-4155-9466-6c197158ed28.png)

· Get-Help Get-Alias | Out GridView

![image](https://user-images.githubusercontent.com/91567318/160494626-4d74766b-f991-48cd-9e59-e59dc1f1d5f9.png)

· Get-Help Get-AuthenticodeSignature | Out GridView

![image](https://user-images.githubusercontent.com/91567318/160494737-ae267518-e07d-4523-8359-e6d71229b363.png)

· Get-Help Get-ControlPanelItem | Out GridView

![image](https://user-images.githubusercontent.com/91567318/160494824-b9c6bfbb-abb4-491f-95ac-a15451cf2d5c.png)

---

## Task  10
### Busque la biblioteca de documentación oficial de PowerShell en microsoft Google MSDN PowerShell. La URL comienza con “https://docs.microsoft.com”.

· https://docs.microsoft.com/es-es/powershell/

![image](https://user-images.githubusercontent.com/91567318/160495130-e5083deb-e08c-4ba9-826c-764e482b64dc.png)

---
