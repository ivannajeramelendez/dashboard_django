# [Dashboard Django](https://soyivan.vtesta.info)

 ![version](https://img.shields.io/badge/version-1.0.0-blue.svg)

Aplicación Dashboard Web con Django.

<br />

## Despliegue de Aplicación

> Instala los modulos via `VENV`  

```bash
virtualenv env
source env/bin/activate
pip install -r requirements.txt
```

<br />

> Configura la base de datos

```bash
python manage.py makemigrations
python manage.py migrate
```

<br />

> Crea el Superuser

```bash
python manage.py createsuperuser
```

<br />

> Inicia la Aplicación

```bash
$ python manage.py runserver 0.0.0.0:80
```

Dentro del navegador: `http://127.0.0.1:8000/`. 

<br />

## Estructura

```bash
< PROJECT ROOT >
   |
   |-- core/                            
   |    |-- settings.py                  # Project Configuration  
   |    |-- urls.py                      # Project Routing
   |
   |-- home/
   |    |-- views.py                     # APP Views 
   |    |-- urls.py                      # APP Routing
   |    |-- models.py                    # APP Models 
   |    |-- tests.py                     # Tests  
   |    |-- templates/                   # Theme Customisation 
   |         |-- includes                # 
   |              |-- custom-footer.py   # Custom Footer      
   |     
   |-- requirements.txt                  # Project Dependencies
   |
   |-- env.sample                        # ENV Configuration (default values)
   |-- manage.py                         # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />

## Customizar

```bash
< LIBRARY_ROOT >                      # This exists in ENV: LIB/admin_soft
   |
   |-- templates/                     # Root Templates Folder 
   |    |          
   |    |-- accounts/       
   |    |    |-- login.html           # Sign IN Page
   |    |    |-- register.html        # Sign UP Page
   |    |
   |    |-- includes/       
   |    |    |-- footer.html          # Footer component
   |    |    |-- sidebar.html         # Sidebar component
   |    |    |-- navigation.html      # Navigation Bar
   |    |    |-- scripts.html         # Scripts Component
   |    |
   |    |-- layouts/       
   |    |    |-- base.html            # Masterpage
   |    |    |-- base-fullscreen.html # Masterpage for Auth Pages
   |    |
   |    |-- pages/       
   |         |-- index.html           # Dashboard page
   |         |-- profile.html         # Settings  Page
   |         |-- *.html               # All other pages
   |    
   |-- ************************************************************************
```
