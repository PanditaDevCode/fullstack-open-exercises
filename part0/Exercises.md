# Ejercicio 0.6 - Nueva Nota Pagina SPA

```mermaid

sequenceDiagram
    participant Usuario
    participant Navegador
    participant Servidor

    Usuario->>Navegador: Escribe la nota y presiona "Guardar"
    Navegador->>Servidor: Enviar solicitud POST con la nueva nota en formato JSON
    Servidor-->>Navegador: Confirmación de éxito en la creación de la nota (respuesta JSON)
    Navegador->>Usuario: Actualiza el DOM para mostrar la nueva nota sin recargar la página
