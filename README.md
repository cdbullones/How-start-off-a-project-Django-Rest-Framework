# Como iniciar un Proyecto Basico de API Django Rest Framework

### **Comando de creacion de entorno de trabajo virtualenv para python3**
`$ virtualenv env --python=python3`

### **Comando de activacion del entorno**
`$ cd env`

`$ source bin/activate`

`(env)$`

### **Comando de ejecucion de archivo requirements.txt**
`(env)$pip install -r requirements.txt`

#### **Contenido de ejemplo del archivo requirements.txt con los paquetes que se instalaran en el entorno de Django**

* Django
* djangorestframework
* psycopg2
* python-dotenv
* django-filter
* djangorestframework_simplejwt
* requests

### **Comando creacion de proyecto django**
`(env)$ django-admin startproject ApiDRF`

### **Comando para crear un aplicacion**
`(env)$ python manage.py startapp users`

### **Comando para crear migraciones**
`(env)$ python manage.py makemigrations users`

### **Comando para correr migraciones**
`(env)$ python manage.py migrate`

### **Comando para ejecutar el proyecto django** 
`(env)$ python manage.py runserver`

##### Documentación Oficial: [https://www.django-rest-framework.org/](https://www.django-rest-framework.org/)

##### Se debe agregar en el archivo *settings.py* el paquete rest framework para trabjar con APIs en Django y las app creadas para que todo funcione correctamente.

```
INSTALLED_APPS = [
    ...
    'rest_framework',
    'users',
]
