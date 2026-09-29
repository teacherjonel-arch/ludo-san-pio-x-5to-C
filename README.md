# Ludo Matemático San Pío X — Online + Administrador

- Juego online con salas y Socket.IO.
- Administrador protegido con contraseña: `1234`.
- Las preguntas editadas por el administrador se envían al servidor y se sincronizan con todos los jugadores conectados.
- Las preguntas se guardan en `data/questions.json` durante la ejecución del servidor.

## Ejecutar

```bash
npm install
npm start
```

Abrir `http://localhost:3000`.

### Importante sobre Render
El archivo `data/questions.json` está en el sistema de archivos del servidor. En servicios con filesystem efímero, un reinicio/redeploy puede restaurar el archivo inicial. Para persistencia permanente conviene conectar una base de datos o almacenamiento persistente.
