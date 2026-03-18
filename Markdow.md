# Reporte Técnico: Estructura y Funcionamiento de Redes Digitales

## I. Fundamentos de la Operación en Internet

### El Modelo de Comunicación: TCP/IP
La estabilidad de la red global se basa en el conjunto de protocolos **TCP/IP**, cuyas tareas se dividen en dos pilares estratégicos:

* **Internet Protocol (IP):** Gestiona el sistema de direccionamiento lógico, otorgando una **etiqueta numérica única** (nodo) a cada equipo vinculado a la red.
* **Transmission Control Protocol (TCP):** Se encarga de la **fragmentación de la información** en bloques transportables, asegurando que lleguen a su destino y se reorganicen correctamente según el tipo de contenido (web, correo o streaming).

---

### Sistemas de Soporte: DNS y DHCP

Para facilitar la interacción del usuario y la configuración de los equipos, existen dos servicios esenciales:

| Sistema | Propósito Operativo | Beneficio Clave |
| :--- | :--- | :--- |
| **DNS** | Resolución de nombres. | Traduce direcciones IP complejas en nombres de dominio fáciles de recordar (como google.com). |
| **DHCP** | Automatización de parámetros. | Asigna configuraciones de red de forma automática, evitando errores de configuración manual. |

> **Nota de Aplicación:** El DNS actúa como la "guía telefónica" de Internet; sin él, tendríamos que memorizar secuencias numéricas para acceder a cualquier sitio web.

---

## II. Protocolo HTTP y la Navegación en la Web

### Componentes de una URL
Para localizar cualquier dato en la red, se emplea una ruta estructurada denominada URL:

1.  **Protocolo:** `https` (Garantiza que el intercambio de información sea seguro y cifrado).
2.  **Host/Dominio:** `www.ejemplo.com` (El nombre del servidor donde reside la información).
3.  **Directorio/Ruta:** `/productos` (La carpeta o sección específica dentro de ese servidor).

---

### Comunicación Cliente-Servidor: Métodos de Petición

La transferencia de datos se realiza mediante comandos específicos conocidos como métodos HTTP:

* **GET:** Orientado exclusivamente a la **lectura y obtención de recursos**. Los datos de la consulta suelen aparecer en la URL del navegador.
* **POST:** Diseñado para **enviar información al servidor** (como contraseñas o archivos). Al viajar dentro del cuerpo de la petición, ofrece mayor seguridad y privacidad.

---

### Interpretación de Respuestas del Servidor

| Código | Categoría | Significado Técnico |
| :--- | :--- | :--- |
| `200` | **OK** | La solicitud fue exitosa y el contenido se carga sin problemas. |
| `301` | **Mudanza** | La página buscada se ha movido permanentemente a una nueva dirección. |
| `404` | **No Encontrado** | El servidor responde, pero no existe un archivo en la ruta indicada. |
| `500` | **Fallo Interno** | Existe un error en la programación o configuración del servidor remoto. |

---

## III. Créditos del Documento

### Autores y Revisores
Este análisis técnico ha sido consolidado por el equipo de **Arquitectura de Redes**, con el fin de estandarizar el conocimiento sobre los mecanismos de transporte y visualización de datos en entornos web.

* **Redacción Técnica:** Analistas de Sistemas e Infraestructura.
* **Documentación:** Especialistas en Protocolos de Comunicación.