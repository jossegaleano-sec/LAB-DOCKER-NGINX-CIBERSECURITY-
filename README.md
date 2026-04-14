# LAB-DOCKER-NGINX-CIBERSECURITY-
Laboratorio experimental, donde se usa la herramienta docker desde un kali linux, en una maquina virtual

1. Preparación del Entorno
Imagen: config_red.jpeg y status_docker.jpeg

Descripción: Configuración del adaptador NAT en VirtualBox y validación del demonio de Docker en Kali Linux. Demuestra que el sistema está listo y el servicio habilitado (enabled).

2. Despliegue del Activo
Imagen: (La que tenías de docker run y docker ps)

Descripción: Creación del contenedor Nginx con mapeo de puertos. El puerto 8080 queda expuesto para auditoría.

3. Verificación de Disponibilidad
Imagen: pagina inicio nginx.jpeg

Descripción: Acceso inicial exitoso al servidor. Se confirma que el servicio es funcional y responde a peticiones HTTP externas.

4. Administración e Intervención (La joya del repo)
Imagen: navegacion por el contenedor y edicion del contenido.jpg y modificacion de contenido.jpeg

Descripción: Este es el núcleo técnico. Muestra cómo usaste exec -it para navegar el sistema de archivos de Linux y cómo alteraste el index.html. El resultado es el mensaje: "Propiedad de la Prefectura - Guardia de Jose".

5. Auditoría y Análisis Forense
Imagen: analisis de los logs de evidencia.jpg

Descripción: Análisis de los registros de acceso. Se explican los códigos HTTP 304 (cache) y 200 (éxito post-modificación), identificando el tamaño de la respuesta de 54 bytes.

6. Higiene del Sistema
Imagen: higiene y cierre de docker.jpeg

Descripción: Cierre del ciclo de vida del contenedor mediante stop y rm. Muestra responsabilidad en la gestión de recursos del sistema.
