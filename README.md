Example for demoing a bokeh server with Binder

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/philippjfr/panel-glacier-app/master?urlpath=%2Fproxy%2F5006%2Fbokeh-app)

Create a `bokeh-app` directory in the repo with a `main.py`.
This is the application that will be served.


This repo contains:

- `environment.yml` installing bokeh and nbserverproxy
- a custom serverextension (`bokehserverextension.py`) that launches bokeh server
- a `postBuild` script to enable the server extensions and install the local one
  (this last step would go away if the local extension became a proper package)
- A [panel](https://github.com/pyviz/panel) based app which allows cross-filtering on all global glaciers
