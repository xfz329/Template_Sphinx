bilingual
=============================


1. Write the documentation in English.
2. Change directory to the `/docs` and input two commands below.

.. code-block:: bash
    :linenos:

    sphinx-build -b gettext ./source ./build/gettext
    sphinx-intl update -p ./build/gettext -l zh_CN

3. Fetch the `*.po` files in `/docs/locales` and translate as needed.
4. Compile the documentation just in the target language.

.. code-block:: bash
    :linenos:

    sphinx-build -b html -D language=zh_CN ./source/ build/html/zh_CN
