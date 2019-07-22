{% set is\_open\_source = cookiecutter.open\_source\_license != \'Not
open source\' -%} {% for \_ in cookiecutter.project\_name %}={% endfor
%} {{ cookiecutter.project\_name }} {% for \_ in
cookiecutter.project\_name %}={% endfor %}

{% if is\_open\_source %} .. image:: <https://img.shields.io/pypi/v/>{{
cookiecutter.project\_slug }}.svg :target:
<https://pypi.python.org/pypi/>{{ cookiecutter.project\_slug }}

[![image]]

[![Documentation Status]]

{%- endif %}

{% if cookiecutter.add\_pyup\_badge == \'y\' %} .. image::
<https://pyup.io/repos/github/>{{ cookiecutter.github\_username }}/{{
cookiecutter.project\_slug }}/shield.svg :target:
<https://pyup.io/repos/github/>{{ cookiecutter.github\_username }}/{{
cookiecutter.project\_slug }}/ :alt: Updates {% endif %}

{{ cookiecutter.project\_short\_description }}

{% if is\_open\_source %} \* Free software: {{
cookiecutter.open\_source\_license }} \* Documentation: <https://>{{
cookiecutter.project\_slug \| replace(\"\_\", \"-\") }}.readthedocs.io.
{% endif %}

Features
========

-   TODO

Credits
=======

This package was created with [Cookiecutter] and the
[audreyr/cookiecutter-pypackage] project template.

  [image]: https://img.shields.io/travis/%7B%7B%20cookiecutter.github_username%20%7D%7D/%7B%7B%20cookiecutter.project_slug%20%7D%7D.svg
  [![image]]: https://travis-ci.org/%7B%7B%20cookiecutter.github_username%20%7D%7D/%7B%7B%20cookiecutter.project_slug%20%7D%7D
  [Documentation Status]: https://readthedocs.org/projects/%7B%7B%20cookiecutter.project_slug%20%7C%20replace(%22_%22,%20%22-%22)%20%7D%7D/badge/?version=latest
  [![Documentation Status]]: https://%7B%7B%20cookiecutter.project_slug%20%7C%20replace(%22_%22,%20%22-%22)%20%7D%7D.readthedocs.io/en/latest/?badge=latest
  [Cookiecutter]: https://github.com/audreyr/cookiecutter
  [audreyr/cookiecutter-pypackage]: https://github.com/audreyr/cookiecutter-pypackage


