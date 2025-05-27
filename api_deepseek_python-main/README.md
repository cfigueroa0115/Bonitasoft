## API Gratuita para Lanzar modelo de DeepSeek

Esta api permite disponibilizar una API con el modelo gratuito de DeepSeek haciendo uso de openroute.

### Indicaciones:
- En un archivo .env poner la el api key generado en open route con el nombre: OPENROUTER_API_KEY. Deberia quedar algo asi: OPENROUTER_API_KEY=sk-or-v1-******
- Crear un entorno virutal e instalar las dependencias de requeriments necesarias con pip3 install -r requirements.txt.
- Correr el siguiente comando: uvicorn main:app --reload -> El cual disponibiliza la api en el puerto http://127.0.0.1:8000

### Consumo de api:
- Se puede consumir directamente desde postman o insomnia con haciendo una petición post a la urL: http://127.0.0.1:8000/chat
- El body debe ser un JSON con un parametro "content" así:
 ```javascript
  {
    "content": "Hola, como estas?"
  }
```
Otra opción de consumo de la API es abrir el /docs de FastAPI() que permite directamente con una documentación hacer peticiones a la API disponibilizada de una forma mas sencilla
para esto solo basta con entrar a la dirección: http://127.0.0.1:8000/docs
