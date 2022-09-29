API
===

.. autosummary::
   :toctree: generated

   lumache

Projects
~~~~~~~~

Projects list
+++++++++++++

.. http:get:: /api/v3/projects/

    Retrieve a list of all the projects for the current logged in user.

    **Example request**:

    .. tabs::

        .. code-tab:: bash

            $ curl -H "Authorization: Token <token>" https://readthedocs.org/api/v3/projects/

        .. code-tab:: python

            import requests
            URL = 'https://readthedocs.org/api/v3/projects/'
            TOKEN = '<token>'
            HEADERS = {'Authorization': f'token {TOKEN}'}
            response = requests.get(URL, headers=HEADERS)
            print(response.json())
