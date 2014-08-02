============
Installation
============

At the command line::

    $ pip {{ cookiecutter.repo_name }}

Installing in your project specific `virtualenv
<https://virtualenv.pypa.io/en/latest/virtualenv.html>_` is highly recommended.

Add `{{ cookiecutter.app_name }}` to your `INSTALLED_APPS` tuple::

    INSTALLED_APPS = (
        ...
        '{{ cookiecutter.app_name }}'.
    )

Add in the app URLs using the endpoint which makes the most sense for
your project::

    urlpatterns = patterns('',
        url(r'^{{ cookiecutter.app_name }}/', include('{{ cookiecutter.app_name }}.urls')),
    )
