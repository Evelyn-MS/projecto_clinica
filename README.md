## Proyecto de Clínica 
En qué consiste este proyecto:

Administrar médicos, especialidades y agendas.
Crear una agenda para disponibilizar las consultas.
Permitir al usuario elegir una consulta en día y horario de acuerdo con la agenda del médico.

## Configuración del entorno para ejecutar la aplicación web.
Descarga este repositorio:

```
$ git clone git@github.com:Dan-Source/projeto_clinica.git
```

Crea una máquina virtual e instala las bibliotecas disponibles en el archivo requirements.txt:

Entra en la carpeta creada e inicia un entorno virtual:

```
$ cd projeto_clinica
$ python3 -m venv venv
```
Luego debes activarlo con el siguiente comando:

```
$ source ./venv/bin/activate
```
Una vez activado, instala las bibliotecas necesarias para ejecutar el proyecto:
```
 (venv)$ pip install -r requirements.txt
```
Para poder tener el primer acceso y configurar la aplicación, ejecuta el comando migrate para generar la base de datos predeterminada de Django (SQLite). Luego, crea el superusuario:

```
(venv)$ ./manage.py migrate
(venv)$ ./manage.py createsuperuser
Apelido/Usuário: admin
E-mail: admin@mail.com
Password: 
Password (again):
```

Para iniciar el servidor después de este paso, debes ejecutar:
```
(venv)$ ./manage.py runserver
```


Para verificar si todo está funcionando como se espera, accede a la siguiente dirección:
[http://localhost:8000/](http://localhost:8000/)


O puedes acceder al panel de administración de Django en la siguiente dirección:
[http://localhost:8000/admin](http://localhost:8000/admin)

