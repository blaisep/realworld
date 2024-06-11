# Tahoe LAFS sample apps

**Note: this is just a reference implementation and is not intended for production use.**

## About example: Django persistence

If you fit either of these descriptions, this example is for you: 
    A) the dev who wants to write an app using Tahoe for persistence.
    B) the dev who wants to see how an existing app uses Tahoe for persistence.

## About the client, a Django app

Implementation of real-world application: https://github.com/gothinkster/realworld/ using Django and HTMX.
The app is based on the gothinkster/realworld example contributed by https://github.com/danjac/realworld/
An in-depth discussion of this implementation can be found [here](https://danjacob.net/posts/anatomyofdjangohtmxproject/).

Tech Stack:

* [Django](https://djangoproject.com)
* [HTMX](https://htmx.org)
* [Alpine](https://alpinejs.dev)

To install and run locally:

```bash
git clone https://github.com/blaisep/realworld/ && cd realworld

python -m venv venv

source venv/bin/activate

pip install -r requirements.txt

./manage.py migrate && ./manage.py runserver
```

## About the persistence

