Example for demoing a bokeh server with Binder

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/minrk/binder-bokeh-server/master?urlpath=%2Fproxy%2F5006%2Fbokeh-app)

Create a `bokeh-app` directory in the repo with a `main.py`.
This is the application that will be served.


This repo contains:

- `environment.yml` installing bokeh and nbserverproxy
- a custom serverextension (`bokehserverextension.py`) that launches bokeh server
- a `postBuild` script to enable the server extensions and install the local one
  (this last step would go away if the local extension became a proper package)
- the [weather example](https://github.com/bokeh/bokeh/tree/master/examples/app/weather) from the bokeh repo in the `bokeh-app` directory.
