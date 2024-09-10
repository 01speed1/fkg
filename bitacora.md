Mi objetivo es crear una aplicación que permita a usuarios **SupportOperators**, generar casos de soporte
desde una interfaz bonita e intuitiva

igual necesito una tabla con la que los **SupportOperation** puedan
interactuar es por eso que he creado un tabla para un flujo basico de
transacciones, con **Provider**, **Customer**, **Service**, **Transaction**

tambien tengo un par de tablas para el manejo de los usuarios **User**,
**Role**, con el cual podre controlar el acceso a la aplicación

[Model Entidad-relación](https://app.chartdb.io/diagrams/u08voxk2h9r8p4jaeg32q94d5)

paso siguiente sera montar la api y probar el login

```
fastapi-app/
├── app/
│   ├── __init__.py
│   ├── main.py          # Punto de entrada de la aplicación
│   ├── api/
│   │   ├── __init__.py
│   │   ├── v1/
│   │   │   ├── __init__.py
│   │   │   ├── endpoints/
│   │   │   │   ├── __init__.py
│   │   │   │   ├── items.py  # Ejemplo de endpoint
│   │   │   │   └── users.py  # Ejemplo de endpoint
│   ├── core/
│   │   ├── __init__.py
│   │   ├── config.py    # Configuraciones de la aplicación
│   ├── models/
│   │   ├── __init__.py
│   │   ├── item.py      # Modelos de base de datos
│   │   ├── user.py      # Modelos de base de datos
│   ├── schemas/
│   │   ├── __init__.py
│   │   ├── item.py      # Modelos de Pydantic
│   │   ├── user.py      # Modelos de Pydantic
│   ├── services/
│   │   ├── __init__.py
│   │   ├── item.py      # Lógica de negocio
│   │   ├── user.py      # Lógica de negocio
│   ├── db/
│   │   ├── __init__.py
│   │   ├── base.py      # Configuración de la base de datos
│   │   ├── session.py   # Sesiones de la base de datos
│   ├── tests/
│   │   ├── __init__.py
│   │   ├── test_items.py # Pruebas para los endpoints de items
│   │   ├── test_users.py # Pruebas para los endpoints de users
├── .env                 # Variables de entorno
├── requirements.txt     # Dependencias del proyecto
├── alembic/             # Migraciones de la base de datos
│   ├── versions/
│   ├── env.py
│   ├── script.py.mako
└── README.md            # Documentación del proyecto

```

https://www.psycopg.org/psycopg3/docs/basic/usage.html

despues de luchas con los endpoint en python,no me voy a complicar con la vista, voy hacer que cargue primero el login, si ya esta auth que cargue la interfaz de de reporte, luego volvera a la api para agregar los endpoint y poder guardar y consultar los reportes

agregar las diferentes vistas por roles, 

---

---

---
