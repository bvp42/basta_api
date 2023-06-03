# API de Verificación de categoría de una palabra

Esta API proporciona un punto final para verificar si una palabra corresponde a un animal,nombre,pais,flor-fruto y color en base al juego de Basta.

## Uso

Realiza una solicitud GET al los siguientes endpoints:

```/animal/{word}
/color/{palabra}
/pais/{word}
/nombre/{word}
/flor-fruto/{word}
```

Reemplaza `{word}` con la palabra que deseas verificar. 

La API devolverá una respuesta indicando si la palabra corresponde a la categoria o no diciendo solo la palabra de la categoria si es verdadero o "no existe en la categoria ..." si es falso.

### Ejemplo de solicitud

GET /animal/gato


### Ejemplo de respuesta

```json
{
  "palabra": "gato",
  "category": "animal"
}
```
En este caso, la palabra "gato" es reconocida como un animal.

Instalacion:

Descargar el codigo e instalar las dependencias fastapi y uvicorn.

Al correr el codigo la API estará disponible en http://localhost:10000.

#### Nota: La cantidad de palabras que puede validar es aún limitada
