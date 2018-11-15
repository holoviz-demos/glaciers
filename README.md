# OGGM Glacier Panel App

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/panel-demos/glaciers/master?urlpath=/proxy/5006/app)

Serves the `app.ipynb` which defines the panel application that will be served.

This repo contains:

- `environment.yml` installing bokeh and nbserverproxy
- a custom serverextension (`bokehserverextension.py`) that launches bokeh server
- a `postBuild` script to enable the server extensions and install the local one
  (this last step would go away if the local extension became a proper package)
- A [panel](https://github.com/pyviz/panel) based app which allows cross-filtering on all global glaciers
