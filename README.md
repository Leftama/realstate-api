# RealEstate API

Una API REST simple para gestionar inmuebles construida con Node.js y Express.

## 📋 Descripción

Esta API proporciona endpoints para consultar información sobre inmuebles disponibles, incluyendo apartamentos, casas y estudios con sus respectivos precios y direcciones.

## Tecnologías

- **Node.js** - Entorno de ejecución
- **Express.js** - Framework web
- **Jest** - Testing framework
- **Supertest** - Testing HTTP

## Estructura del proyecto

```bash
realstate-api/
├── node_modules/
├── src/
│   └── app.js          # Aplicación principal
├── tests/
│   └── app.test.js     # Pruebas unitarias
├── package.json
├── package-lock.json
└── README.md
```

## 🛠️ Instalación

1. Clona el repositorio:

```bash
git clone <url-del-repositorio>
cd realstate-api
```

1. Instala las dependencias:

```bash
npm install
```

## Uso

### Iniciar el servidor

```bash
npm start
```

### Ejecutar las pruebas

```bash
npm test
```

### Ejecutar las pruebas en modo watch

```bash
npm run test:watch
```

## API Endpoints

### GET /api/inmuebles

Obtiene la lista completa de inmuebles disponibles.

**Respuesta exitosa (200):**

```json
[
  {
    "id": 1,
    "direccion": "Calle 123",
    "precio": 150000,
    "tipo": "Apartamento"
  },
  {
    "id": 2,
    "direccion": "Avenida 456",
    "precio": 230000,
    "tipo": "Casa"
  },
  {
    "id": 3,
    "direccion": "Carrera 789",
    "precio": 120000,
    "tipo": "Estudio"
  }
]
```

## Testing

El proyecto incluye pruebas unitarias que verifican:

- ✅ Respuesta exitosa del endpoint
- ✅ Estructura correcta de los datos
- ✅ Propiedades requeridas en cada inmueble

Para ejecutar las pruebas:

```bash
npm test
```

## Dependencias

### Dependencias de producción

- `express`: Framework web para Node.js

### Dependencias de desarrollo

- `jest`: Framework de testing
- `supertest`: Biblioteca para testing HTTP

## Scripts disponibles

```bash
npm start          # Inicia el servidor
npm test           # Ejecuta las pruebas
npm run test:watch # Ejecuta las pruebas en modo watch
```

## Próximas características

- [ ] Endpoint para obtener inmueble por ID
- [ ] Endpoint para crear nuevos inmuebles
- [ ] Endpoint para actualizar inmuebles
- [ ] Endpoint para eliminar inmuebles
- [ ] Filtros por tipo y rango de precios
- [ ] Paginación de resultados
- [ ] Validación de datos de entrada
- [ ] Conexión a base de datos

## Contribución

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## Autor

Cristián R. Araya - [caraya.salazar@gmail.com](mailto:caraya.salazar@gmail.com)

Enlace del proyecto: [https://github.com/Leftama/realstate-api](https://github.com/Leftama/realstate-api)
