# WinFormsApp — paso a paso (en visual studio code)

1) Ir a la carpeta del proyecto (raíz del workspace)

```powershell
cd 'c:\Users\Juan\Progra\3_C'
```

2) Crear la app WinForms

```powershell
dotnet new winforms -o WinFormsApp -f net10.0
```

3) Entrar a la carpeta del proyecto recién creada

```powershell
cd 'c:\Users\Juan\Progra\3_C\WinFormsApp'
```

4) Compilar para verificar que todo quedó bien

```powershell
dotnet build
```

5) Ejecutar la aplicación (se abre la ventana WinForms)

```powershell
dotnet run
```
