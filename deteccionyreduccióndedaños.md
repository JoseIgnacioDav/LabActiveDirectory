Que Monitorear en el Servidor
Para saber si alguien está intentando atacar el dominio, se revisan códigos específicos en el registro de eventos de Windows:

Evento 4768: Solicitud de acceso Kerberos (clave para detectar ataques a usuarios sin preautenticación).

Evento 4769: Solicitud de tickets de servicio (clave para ver peticiones masivas de servicios).

Evento 4625: Intentos fallidos de inicio de sesión (sirve para ver si intentan adivinar claves).
