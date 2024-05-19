# Aplicação Blog


## Ativando Aplicação 

~~~ 
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'blog.apps.BlogConfig'
]
~~~

## Models


### Enum

O código abaixo, se trata de ENUM sobre o status da publicação, que seria rascunho (draft) e publicado 
~~~ python
    class Status(models.TextChoices):
        DRAFT = 'DF', 'Draft'
        PUBLISHED = 'PB', 'Published'

~~~ 