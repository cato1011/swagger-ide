## Swagger-IDE

The Swagger-UI and Swagger-Mock-API always use the current YAML of the Swagger-Editor. Also the Swagger-Editor saves the current YAML locally. So everything is persistence and stays up to date.


```bash
git clone https://github.com/cato1011/swagger-ide.git
cd swagger-ide
docker build -t swagger-ide .
docker run -d -i -p 8080:80 -p 8000:8000 swagger-ide
```

After that you can reach the Swagger-Editor and UI under:

* [docker-ip]:8080/swagger 
* [docker-ip]:8080/swagger-ui

The Swagger-Mock-Api is available under

* [docker-ip]:8000

### About Swagger

For further information about Swagger-Editor and -UI visit: http://swagger.io/

### About Swagger-Mock-API

For further information about the Mock-API and defining custom types in the Swagger-Editor, have a look at:

https://www.npmjs.com/package/swagger-mock-api#specifying-custom-chance-options

The chance types and options depend on http://chancejs.com/