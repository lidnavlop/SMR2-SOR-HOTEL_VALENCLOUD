# Tarea 1: Creación de Cuentas Operativas (CE a)
```mermaid
flowchart TD
    A[Inicio de la fase de gestión de identidades del hotel] --> B[Analizamos los perfiles laborales necesarios para el funcionamiento del Hotel ValenCloud]
    B --> C[Identificamos los distintos roles operativos como recepción administración limpieza e IT]
    C --> D[Definimos una política de nomenclatura coherente para todas las cuentas de usuario]
    D --> E[He iniciado sesión en el controlador de dominio utilizando credenciales administrativas]
    E --> F[Abrimos la consola Active Directory Users and Computers]
    F --> G[Seleccionamos la Unidad Organizativa destinada a las cuentas operativas]

    G --> H[Creamos la cuenta Recepcion01 para el personal del front desk]
    H --> I[Asignamos una contraseña inicial segura cumpliendo los requisitos de complejidad]
    I --> J[Configuramos el cambio obligatorio de contraseña en el primer inicio de sesión]

    J --> K[Creamos la cuenta AdminHotel01 asociada al departamento administrativo]
    K --> L[Configuramos restricciones de acceso acordes a su función]

    L --> M[Creamos la cuenta Limpieza01 para el personal de housekeeping]
    M --> N[Limitamos los privilegios aplicando el principio de mínimo acceso]

    N --> O[Creamos la cuenta ITSupport01 destinada al soporte técnico]
    O --> P[Verificamos atributos como descripción departamento y nombre completo]

    P --> Q[Revisamos todas las cuentas creadas]
    Q --> R[Validamos que los objetos se han registrado correctamente en el dominio]
```


# Tarea 2: Definición de Entornos de Trabajo (CE b)

```mermaid
flowchart TD
    A[Inicio de la estructuración lógica del dominio] --> B[Analizamos la organización funcional del hotel]
    B --> C[Identificamos áreas operativas diferenciadas]

    C --> D[Creamos la OU Recepcion para agrupar los recursos del personal de atención al cliente]
    D --> E[Creamos la OU Administracion para el personal de gestión interna]
    E --> F[Creamos la OU Housekeeping para el personal de limpieza]
    F --> G[Creamos la OU IT para el departamento técnico]
    G --> H[Creamos la OU Direccion para las cuentas de alto nivel]

    H --> I[Asignamos descripciones claras a cada Unidad Organizativa]
    I --> J[Revisamos la jerarquía organizativa del dominio]

    J --> K[Movemos manualmente las cuentas de usuario a sus respectivas OU]
    K --> L[Validamos la correcta segmentación administrativa]
```

---

# Tarea 3: Registro de Dispositivos (CE c)

```mermaid
flowchart TD
    A[Inicio del proceso de integración de equipos] --> B[Preparamos las estaciones de trabajo del hotel]
    B --> C[Configuramos parámetros de red y DNS]

    C --> D[Unimos el equipo PC-Recepcion01 al dominio]
    D --> E[Autenticamos la operación mediante credenciales administrativas]
    E --> F[Reiniciamos el sistema para aplicar los cambios]

    F --> G[Unimos el equipo PC-Admin01 al dominio]
    G --> H[Verificamos su registro correcto en Active Directory]

    H --> I[Unimos el equipo PC-Housekeeping01]
    I --> J[Comprobamos la creación automática del objeto Computer]

    J --> K[Ubicamos manualmente los dispositivos en las OU correspondientes]
    K --> L[Validamos la consistencia del inventario lógico]
```

---

# Tarea 4: Diseño de la Estructura de Acceso (CE d)

```mermaid
flowchart TD
    A[Inicio de la planificación de accesos] --> B[Analizamos las necesidades de cada departamento]
    B --> C[Aplicamos el principio de mínimo privilegio]

    C --> D[Definimos los niveles de acceso para Recepcion]
    D --> E[Definimos los niveles de acceso para Administracion]
    E --> F[Definimos los niveles de acceso para IT]
    F --> G[Definimos restricciones específicas para Housekeeping]

    G --> H[Documentamos la política de accesos del dominio]
    H --> I[Validamos la coherencia entre roles y permisos]
```

---

# Tarea 5: Implementación de Grupos Funcionales (CE e)

```mermaid
flowchart TD
    A[Inicio de la gestión de grupos de seguridad] --> B[Creamos el grupo RecepcionStaff]
    B --> C[Definimos su ámbito y tipo de grupo]

    C --> D[Creamos el grupo AdministracionStaff]
    D --> E[Creamos el grupo ITStaff]
    E --> F[Creamos el grupo HousekeepingStaff]

    F --> G[Añadimos los usuarios a sus grupos correspondientes]
    G --> H[Verificamos las membresías configuradas]
```

---

# Tarea 6: Asignación de Permisos (CE f)

```mermaid
flowchart TD
    A[Inicio de la configuración de permisos] --> B[Identificamos los recursos compartidos del hotel]
    B --> C[Configuramos permisos NTFS]

    C --> D[Asignamos permisos de lectura y escritura al grupo AdministracionStaff]
    D --> E[Asignamos permisos limitados al grupo RecepcionStaff]
    E --> F[Asignamos permisos técnicos ampliados al grupo ITStaff]

    F --> G[Realizamos pruebas de acceso con cuentas de usuario]
    G --> H[Corregimos posibles inconsistencias detectadas]
```

---

# Tarea 7: Auditoría de Seguridad Inicial (CE g)

```mermaid
flowchart TD
    A[Inicio del endurecimiento de la seguridad] --> B[Editamos las políticas de auditoría]
    B --> C[Habilitamos la auditoría de eventos de inicio de sesión]
    C --> D[Habilitamos la auditoría de gestión de cuentas]

    D --> E[Verificamos la generación de registros]
    E --> F[Validamos los eventos en el visor de sucesos]
```

---

# Tarea 8: Movilidad y Despliegue de Perfiles (CE h)

```mermaid
flowchart TD
    A[Inicio de la configuración de perfiles] --> B[Definimos una ubicación centralizada para perfiles móviles]
    B --> C[Configuramos el atributo Profile Path en las cuentas de usuario]

    C --> D[Probamos el inicio de sesión en distintos equipos]
    D --> E[Validamos la correcta carga del perfil]
```

---

# Tarea 9: Aplicación de Herramientas de Administración (CE i)

```mermaid
flowchart TD
    A[Inicio de la fase de administración avanzada] --> B[Utilizamos Active Directory Administrative Center]
    B --> C[Verificamos la estructura completa del dominio]

    C --> D[Utilizamos Group Policy Management]
    D --> E[Validamos la correcta aplicación de directivas]

    E --> F[Revisamos la configuración general del entorno]
    F --> G[Documentamos todas las tareas realizadas]
```


# Tarea 2: Definición de Entornos de Trabajo (CE b)

```mermaid
flowchart TD
    A[Inicio de la estructuración lógica del dominio] --> B[Analizamos la organización funcional del hotel]
    B --> C[Identificamos áreas operativas diferenciadas]

    C --> D[Creamos la OU Recepcion para agrupar los recursos del personal de atención al cliente]
    D --> E[Creamos la OU Administracion para el personal de gestión interna]
    E --> F[Creamos la OU Housekeeping para el personal de limpieza]
    F --> G[Creamos la OU IT para el departamento técnico]
    G --> H[Creamos la OU Direccion para las cuentas de alto nivel]

    H --> I[Asignamos descripciones claras a cada Unidad Organizativa]
    I --> J[Revisamos la jerarquía organizativa del dominio]

    J --> K[Movemos manualmente las cuentas de usuario a sus respectivas OU]
    K --> L[Validamos la correcta segmentación administrativa]
```

---

# Tarea 3: Registro de Dispositivos (CE c)

```mermaid
flowchart TD
    A[Inicio del proceso de integración de equipos] --> B[Preparamos las estaciones de trabajo del hotel]
    B --> C[Configuramos parámetros de red y DNS]

    C --> D[Unimos el equipo PC-Recepcion01 al dominio]
    D --> E[Autenticamos la operación mediante credenciales administrativas]
    E --> F[Reiniciamos el sistema para aplicar los cambios]

    F --> G[Unimos el equipo PC-Admin01 al dominio]
    G --> H[Verificamos su registro correcto en Active Directory]

    H --> I[Unimos el equipo PC-Housekeeping01]
    I --> J[Comprobamos la creación automática del objeto Computer]

    J --> K[Ubicamos manualmente los dispositivos en las OU correspondientes]
    K --> L[Validamos la consistencia del inventario lógico]
```

---

# Tarea 4: Diseño de la Estructura de Acceso (CE d)

```mermaid
flowchart TD
    A[Inicio de la planificación de accesos] --> B[Analizamos las necesidades de cada departamento]
    B --> C[Aplicamos el principio de mínimo privilegio]

    C --> D[Definimos los niveles de acceso para Recepcion]
    D --> E[Definimos los niveles de acceso para Administracion]
    E --> F[Definimos los niveles de acceso para IT]
    F --> G[Definimos restricciones específicas para Housekeeping]

    G --> H[Documentamos la política de accesos del dominio]
    H --> I[Validamos la coherencia entre roles y permisos]
```

---

# Tarea 5: Implementación de Grupos Funcionales (CE e)

```mermaid
flowchart TD
    A[Inicio de la gestión de grupos de seguridad] --> B[Creamos el grupo RecepcionStaff]
    B --> C[Definimos su ámbito y tipo de grupo]

    C --> D[Creamos el grupo AdministracionStaff]
    D --> E[Creamos el grupo ITStaff]
    E --> F[Creamos el grupo HousekeepingStaff]

    F --> G[Añadimos los usuarios a sus grupos correspondientes]
    G --> H[Verificamos las membresías configuradas]
```

---

# Tarea 6: Asignación de Permisos (CE f)

```mermaid
flowchart TD
    A[Inicio de la configuración de permisos] --> B[Identificamos los recursos compartidos del hotel]
    B --> C[Configuramos permisos NTFS]

    C --> D[Asignamos permisos de lectura y escritura al grupo AdministracionStaff]
    D --> E[Asignamos permisos limitados al grupo RecepcionStaff]
    E --> F[Asignamos permisos técnicos ampliados al grupo ITStaff]

    F --> G[Realizamos pruebas de acceso con cuentas de usuario]
    G --> H[Corregimos posibles inconsistencias detectadas]
```

---

# Tarea 7: Auditoría de Seguridad Inicial (CE g)

```mermaid
flowchart TD
    A[Inicio del endurecimiento de la seguridad] --> B[Editamos las políticas de auditoría]
    B --> C[Habilitamos la auditoría de eventos de inicio de sesión]
    C --> D[Habilitamos la auditoría de gestión de cuentas]

    D --> E[Verificamos la generación de registros]
    E --> F[Validamos los eventos en el visor de sucesos]
```

---

# Tarea 8: Movilidad y Despliegue de Perfiles (CE h)

```mermaid
flowchart TD
    A[Inicio de la configuración de perfiles] --> B[Definimos una ubicación centralizada para perfiles móviles]
    B --> C[Configuramos el atributo Profile Path en las cuentas de usuario]

    C --> D[Probamos el inicio de sesión en distintos equipos]
    D --> E[Validamos la correcta carga del perfil]
```

---

# Tarea 9: Aplicación de Herramientas de Administración (CE i)

```mermaid
flowchart TD
    A[Inicio de la fase de administración avanzada] --> B[Utilizamos Active Directory Administrative Center]
    B --> C[Verificamos la estructura completa del dominio]

    C --> D[Utilizamos Group Policy Management]
    D --> E[Validamos la correcta aplicación de directivas]

    E --> F[Revisamos la configuración general del entorno]
    F --> G[Documentamos todas las tareas realizadas]
```
