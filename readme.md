Active Directory Security Laboratory (AD-Security-Lab)
Entorno de laboratorio de Active Directory diseñado para investigación y educación en ciberseguridad, simulando una red corporativa (corp.local) para auditoría, despliegue y ataques de identidad.

Objetivo
Implementar, auditar y documentar vulnerabilidades en infraestructuras de Active Directory, abarcando seguridad ofensiva (Red Teaming) y mecanismos de defensa (Blue Team).

Tecnologías y Herramientas
Virtualización: VirtualBox (Red aislada).

Controlador de Dominio: Windows Server Evaluation 2022 (DC01).

Clientes: Windows 11 Evaluation (Client01, Client02).

Atacante: Kali Linux.

Herramientas: Netexec, Ldapdomaindump, BloodHound-python, Impacket Toolkit.

Arquitectura
DC01 (192.168.56.10): Controlador de dominio principal y servidor DNS (corp.local).

Clientes: Equipos unidos al dominio.

Kali Linux: Nodo de pruebas de penetración.

Vectores de Ataque Documentados
Enumeración LDAP: Reconocimiento de usuarios, equipos y políticas.

AS-REP Roasting: Explotación de cuentas sin preautenticación Kerberos (DONT_REQ_PREAUTH).

Kerberoasting: Solicitud de tickets TGS para cuentas con SPNs expuestos.

BloodHound: Análisis gráfico de rutas de ataque.

Mitigación y Hardening
Deshabilitar preautenticación nula y control de sesiones anónimas.

Políticas estrictas y rotación de contraseñas para cuentas de servicio.

Monitoreo de eventos de Windows (Event IDs 4768 y 4769).

Reproducción
Consulta la documentación en la carpeta docs/ para el paso a paso del despliegue y ejecución de ataques.
