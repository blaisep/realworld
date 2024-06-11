# Tahoe LAFS sample apps

**Note: this is just a reference implementation and is not intended for production use.**

## Example Scenario: Django persistence using Tahoe LAFS

If you fit either of these descriptions, this example app is for you: 

    - the dev who wants to write an app using Tahoe for persistence.
    - the dev who wants to see how an existing app uses Tahoe for persistence.

## About the client, a Django app

Implementation of real-world application: https://github.com/gothinkster/realworld/ using Django and HTMX.
The app is based on the gothinkster/realworld app contributed by [Dan Jacobs](https://github.com/danjac/realworld/) 
because of the focus on Python.
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

---

## Integrate with Tahoe LAFS

### Excercises with realworld scenarios:

- Install tahoe LAFS to use the public Test Grid
- Extend the Django App to store account profiles on Tahoe LAFS
- Extend the Django App to store articles on Tahoe LAFS
- Extend the Django App to store login information on Tahoe LAFS

### Install and run Tahoe LAFS

Use the package from PyPi
```
pip install tahoe-lafs
tahoe --version
```
Configure the public test grid

