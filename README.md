# offline-swagger-ui
One html file that generate swagger UI by loading any given swagger spec. Even not connect to the Internet.
Took and modified slightly from [here](https://github.com/swagger-api/swagger-editor/issues/664#issuecomment-376512344).  
Only support swagger-spec 2.0 (OpenAPI spec 2.0) now.

## Usage

1. Download this repo as a zip file and unzip it.
2. Just open 'offline-swagger-ui.html' with ***Edge*** or ***Firefox***. 'petstore.yaml' will be loaded by default as an example.

## Config

You can place your own swagger spec files into the directory which 'offline-swagger-ui.html' resides in and change `url` field of the Swagger UI constructor in the html (almost at the end) to your yaml link.  
Of course you can also change the `url` field to any spec file available on the Internet such as [this](https://raw.githubusercontent.com/OAI/OpenAPI-Specification/master/examples/v2.0/yaml/uber.yaml).

## Limitations

* ***Google Chrome*** does not load local files by default due to security reasons. The following links may help:
    * <http://www.chrome-allow-file-access-from-file.com/>
    * <https://chrisbitting.com/2014/03/04/allow-local-file-access-in-chrome-windows/>
