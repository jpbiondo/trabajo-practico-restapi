# Trabajo Práctico REST API
Es un proyecto donde se realiza una API REST hecha con Spring. Provee endpoints para las operaciones CRUD de una entidad Persona

## Ejecución del proyecto
Los pasos 2 y 3 pueden omitirse si tu IDE provee plug-ins que se encarguen de las dependencias del proyecto y permitan ejecutarlo.

1. Clonar el repositorio.
```sh
git clone https://github.com/jpbiondo/trabajo-practico-restapi.git
cd trabajo-practico-restapi
```
2. Contruir el proyecto. Para armar el proyecto, instalar las dependencias requeridas:
```sh
./gradlew build
```
3. Correr el projecto.
```sh
./gradlew bootRun
```
## Uso
Una vez el proyecto esté en ejecución, podrás acceder a los endpoints de la API utilizando herramientas como Postman, cUrl o cualquier otro
cliente de HTTP.
## Endpoints 
### GET
- **GET /api/v1/personas**: Obtener lista de todas las personas
- **GET /api/v1/personas/{id}**: Obtener la persona con el ID especificado.
### POST
- **POST /api/v1/personas**: Crear una nueva persona
    - **Formato Body Request**:
```JSON
{
  "id": "number",
  "nombre": "string",
  "apellido": "string",
  "dni": "string",
  "domicilio": {
    "id": "number",
    "calle": "string",
    "numero": "number"
  }
}
```
### PUT
- **PUT /api/v1/personas/{id}**: Actualizar una persona con el ID especificado.
   - **Formato Body Request**:
```JSON
{
  "id": "number",
  "nombre": "string",
  "apellido": "string",
  "dni": "string",
  "domicilio": {
    "id": "number",
    "calle": "string",
    "numero": "number"
  }
}
```
### DELETE
- **DELETE /api/v1/personas/{id}**: Elimina la persona con el ID especificado.
<hr/>
