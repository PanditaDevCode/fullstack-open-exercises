sequenceDiagram
    participant Usuario
    participant Navegador
    participant Servidor

    Usuario->>Navegador: Escribe texto y presiona en "Enviar"
    Navegador->>Servidor: Enviar solicitud POST con el nuevo texto
    Servidor-->>Navegador: Responde con redireccionar (302)
    Navegador->>Servidor: Solicita la lista de las notas
    Servidor-->>Navegador: Envía el HTML actualizado
    Navegador->>Usuario: Muestra la lista de notas actualizadas
