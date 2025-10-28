# Control Domótico — Proyecto WinForms

Este directorio contiene el proyecto WinForms de Control Domótico desarrollado para la asignatura Programación 2.

---

## Estructura sugerida del proyecto

```
source/ControlDomotico/
├── ControlDomotico.sln          # Solución de Visual Studio
├── ControlDomotico/             # Proyecto principal
│   ├── ControlDomotico.csproj   # Archivo del proyecto
│   ├── Form1.cs                 # Formulario principal (código)
│   ├── Form1.Designer.cs        # Formulario principal (diseñador)
│   ├── Form1.resx               # Recursos del formulario
│   ├── Program.cs               # Punto de entrada de la aplicación
│   └── ...                      # Otros archivos del proyecto
└── README.md                    # Este archivo
```

---

## Cómo agregar el proyecto

1. **Si ya tienes un proyecto WinForms creado:**
   - Copia todos los archivos del proyecto (`.sln`, carpeta del proyecto con `.csproj`, `.cs`, etc.) a esta carpeta `source/ControlDomotico/`.
   - Asegúrate de que el archivo `.sln` esté en la raíz de esta carpeta.

2. **Si aún no has creado el proyecto:**
   - Desde la terminal, navega a esta carpeta:
     ```bash
     cd source/ControlDomotico
     ```
   - Crea un nuevo proyecto WinForms:
     ```bash
     dotnet new winforms -n ControlDomotico -f net8.0
     ```
   - Crea la solución:
     ```bash
     dotnet new sln -n ControlDomotico
     dotnet sln add ControlDomotico/ControlDomotico.csproj
     ```

---

## Compilación automática

Una vez que agregues los archivos del proyecto a esta carpeta, el workflow de GitHub Actions (`.github/workflows/build-windows.yml`) compilará automáticamente el proyecto cada vez que hagas un commit a la rama `main`.

El workflow genera un archivo ZIP con el ejecutable compilado que puedes descargar desde la sección "Actions" del repositorio en GitHub.

---

## Compilación local

Para compilar el proyecto localmente:

```bash
# Restaurar dependencias
dotnet restore ControlDomotico.sln

# Compilar el proyecto
dotnet build ControlDomotico.sln --configuration Release

# Ejecutar el proyecto
dotnet run --project ControlDomotico/ControlDomotico.csproj
```

---

## Notas

- El proyecto debe estar configurado para .NET 8.0 o compatible.
- Asegúrate de que todos los archivos necesarios estén incluidos en el repositorio (excepto `bin/`, `obj/` que deben estar en `.gitignore`).
- Si tienes recursos externos (imágenes, íconos), colócalos en la carpeta del proyecto o en `assets/images/` del repositorio.

---

Para más información sobre el sitio completo, consulta el [índice principal](../../index.md).
