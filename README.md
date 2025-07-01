 README - Auto_Super Galería de Productos
 Descripción general
Este es un sitio web de galería de productos desarrollado en HTML y CSS puro, diseñado para una tienda ficticia llamada Auto_Super. El diseño tiene una estética oscura y moderna, centrada en mostrar autos en venta, de forma atractiva y completamente responsive (adaptable a dispositivos móviles).

 Estructura del documento HTML
1. <!DOCTYPE html> y <html lang="es">
Define el documento como HTML5 y establece el idioma del sitio en español.

2. <head>
Contiene los metadatos del documento:

<meta charset="UTF-8">: codificación de caracteres UTF-8.

<meta name="viewport"...>: asegura que el sitio sea responsive en dispositivos móviles.

<title>: nombre que aparece en la pestaña del navegador.

<style>: incluye todo el CSS embebido (interno) para el diseño.

 Explicación del CSS
Variables CSS con :root
Se definen variables globales para colores, tamaños, espaciados, bordes y tipografías. Esto permite cambiar fácilmente el tema o estilo.

Ejemplos:

--bg-dark: fondo oscuro.

--primary: color principal (celeste).

--accent: color de acento (rosado fuerte).

--radius: bordes redondeados.

Estilos globales
* { box-sizing: border-box }: evita errores en tamaños al sumar padding y borde.

body: establece el fondo oscuro, color de texto claro y fuente legible.

Contenedor principal .container
Limita el ancho máximo del contenido y aplica espaciado lateral automático.

Encabezado .header
Barra superior negra que incluye:

Logo con el nombre "Auto_Super".

Ruta de navegación (breadcrumb) que muestra la categoría actual.

Título de sección .section-title
Un título grande, centrado y colorido que introduce la sección de productos ("Carros En Venta").

Parrilla de productos .products-grid
Usa display: grid para organizar los productos en columnas automáticas según el tamaño de pantalla, con espacio entre ellos. Responsive con @media.

Tarjeta de producto .product-card
Cada producto es una "tarjeta" visual:

Fondo oscuro con borde y sombra.

Interactividad visual al pasar el mouse: se eleva y la imagen se amplía ligeramente.

Imagen del producto .product-image-container
Usa aspect-ratio para mantener proporción de imagen.

Contiene la imagen y un distintivo visual (badge).

Imagen .product-image
Escalable, ocupa todo el contenedor.

Tiene object-fit: cover para no deformarse.

Insignia del producto .product-badge
Etiqueta como "Nuevo", "Oferta", "Premium", etc. Posicionada arriba a la derecha, con fondo rosado.

Contenido de producto .product-content
Contiene:

Título del producto (.product-title)

Descripción breve (.product-description)

Precio (.product-price), mostrando precio original tachado si aplica.

Botones (.product-actions) para "Agregar al carrito" o "Ver detalles".

Botones .btn, .btn-primary, .btn-secondary
Estilizados para diferenciar acciones principales y secundarias:

Botón principal con fondo celeste.

Botón secundario con borde celeste y fondo transparente.

Responsividad
Con media queries:

En pantallas menores a 768px, la cuadrícula se convierte en una sola columna.

La imagen del smartwatch (si se usara) cambia su posición de fondo.

 Productos incluidos
Carro Deportivo Rojo
Estilo deportivo, motor potente.

Carro Familiar Azul 2024
Ideal para familia, amplio y moderno.

Auto Urbano Compacto
Ahorro de combustible, ideal para ciudad.

SUV Familiar 2025
Motor híbrido, asistencias inteligentes.

Tecnologías utilizadas
HTML5

CSS3 (Variables, Grid, Media Queries)

Responsive Images (<picture>, srcset, loading="lazy")

Diseño UI moderno con estilos visuales oscuros

 Buenas prácticas aplicadas
Uso de :root para variables globales y fácil mantenimiento.

Diseño responsive adaptado a móviles y tablets.

Separación clara entre estructura (HTML) y estilo (CSS).

Accesibilidad básica con alt en imágenes.

Eficiencia en carga con loading="lazy".