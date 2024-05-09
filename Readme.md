# Django OAUTH2 :closed_lock_with_key:

Este proyecto hace uso del protocolo OAUTH2 para el logeo de usuario.

## :wrench: Instalación

Para instalar y ejecutar este proyecto, sigue estos pasos:

1. Clona el repositorio: `git clone`
2. Navega al directorio del proyecto: `cd django-allauth`
3. Instala las dependencias: `pip install -r requirements.txt`
4. Verifica que se hayan realizado todas las migraciones con el comando `python manage.py makemigrations && python manage.py migrate`
5. Crear cuenta superusuario `python manage.py createsuperuser`
6. Registrar los provider desde el admin (Esta app funciona con Facebook y Google)
7. Ejecuta el servidor de desarrollo: `python manage.py runserver_plus --cert-file cert.crt`
8. Ir a https://127.0.0.1:8000 

El uso del comando en el paso 5 se realiza para generar un certificado SSL (no ideal para producción) puesto que OAUTH – RFC 6749 hace uso de conexiones HTTPS por motivos de seguridad.

## :warning: Notas

- Este proyecto está configurado para usar un certificado SSL auto-firmado para desarrollo. No es recomendable usar este tipo de certificado en un entorno de producción.

## :books: Recursos

- [Documentación de Django](https://docs.djangoproject.com/)
- [Documentación de Django Allauth](https://https://docs.allauth.org/en/latest/)
- [RFC 6749 - The OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749)