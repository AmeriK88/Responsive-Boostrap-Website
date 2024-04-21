# Página web responsiva con bootstrap:
En este repositorio muestro un ejemplo de página básica con Bootstrap, compatible con múltiples dispositivos; escritorio, tablets y teléfonos mobiles.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## A second-level heading:
1. Primero debemos crear una plantilla básica de html en nuestro editor de código, añadir los "links" para poder utilizar las librearías de Bootstrap:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carshop</title>
    
    <!--Añadimos Bootstrap + iconos con los links-->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
</head>
<body>

<!--Añadimos el link de Javascript de Bootstrap-->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
</body>
</html>

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Navegación:
2. Debemos añadir las clases de bootstrap correspondientes para darle estilo deseado:
   
<nav class="navbar navbar-expandlg navbar-light bg-light fixed-top">
        <div class="container">
            <a href="#" class="navbar-brand"><span class="text-danger">PM</span>Motors</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" 
            data-bs-target="#navbar-start" aria-controls="navbar-start" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbar-start">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link" href="#">Inicio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Nosotros</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Servicios</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Contacto</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
    ## Galería - carousel:
    3. Ahora añadiremos una galería de imágenes al cuerpo del documento:

    <!--Añadimos el contenido - una galería de imágenes - con sus botones respectivos-->
    <div id="carouselE1" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselE1" class="active" data-bs-slide-to="0" aria-current="true" aria-label="Slide 1"></button>
            <button type="button" data-bs-target="#carouselE1" data-bs-slide-to="1" aria-label="Slide 2"></button>
            <button type="button" data-bs-target="#carouselE1" data-bs-slide-to="2" aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
            <!--Imágenes de la galería con leyendas -->
            <div class="carousel-item d-block 100 active">
            <!--Usar ruta personalizada para las imágenes o crear una carpeta img donde guardarlas -->
                <img src="img/car1.jpg" class="d-block w-100" alt="Imagen coche">
                <div class="carousel-caption">
                    <h5>El mejor servicio garantizado</h5>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Illum, atque minima! 
                    Dicta dolorem minima a laudantium consequatur at architecto quaerat omnis, 
                    aliquid iure tempora quam dolores est dolor esse sint.</p>
                    <p><a href="#" class="btn btn-primary mt-3">Leer Más</a></p>
                </div>
            </div>
            <div class="carousel-item">
                <img src="img/car2.jpg" class="d-block w-100" alt="Imagen coche">
                <div class="carousel-caption">
                    <h5>Calidad al mejor precio</h5>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Illum, atque minima! 
                    Dicta dolorem minima a laudantium consequatur at architecto quaerat omnis, 
                    aliquid iure tempora quam dolores est dolor esse sint.</p>
                    <p><a href="#" class="btn btn-primary mt-3">Leer</a></p>
                </div>
            </div>
            <div class="carousel-item">
                <img src="img/car3.jpg" class="d-block w-100" alt="Imagen coche">
                <div class="carousel-caption">
                    <h5>Garantía en todos nuestros productos</h5>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Illum, atque minima! 
                    Dicta dolorem minima a laudantium consequatur at architecto quaerat omnis, 
                    aliquid iure tempora quam dolores est dolor esse sint.</p>
                    <p><a href="#" class="btn btn-primary mt-3">Leer</a></p>
                </div>
            </div>
            <div class="carousel-item">
                <img src="img/car4.jpg" class="d-block w-100" alt="Imagen coche">
                <div class="carousel-caption">
                    <h5>Motores de calidad</h5>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Illum, atque minima! 
                    Dicta dolorem minima a laudantium consequatur at architecto quaerat omnis, 
                    aliquid iure tempora quam dolores est dolor esse sint.</p>
                    <p><a href="#" class="btn btn-primary mt-3">Leer</a></p>
                </div>
            </div>
        </div>

        -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

        ## Sección envíos y devoluciones:
        4. Debemos asegurar que hemos importado el link de iconos como mostrado en el paso nº 1 para poder visualizarlos:

        <section class="section-icons">
        <div class="container">
            <div class="row">
                <div class="col-12 col-md-12 col-lg-4 box-icons">
                    <div class="d-flex align-items-center">
                        <i class="bi bi-airplane"></i>
                        <div class="ms-4">
                            <h3>Envío incluido</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-md-12 col-lg-4 box-icons">
                    <div class="d-flex align-items-center">
                        <i class="bi bi-cash-coin"></i>
                        <div class="ms-4">
                            <h3>Devoluciones</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

     -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

     ## Footer de página:

     5. Tu footer es una oportunidad para incluir enlaces internos a otras páginas web o partes de tu sitio y hacer la navegación sea más fácil en dispositivos móviles. 

      <!-- Footer y estilos -->
    <footer class="bg-body-tertiary align-items-center">
        <p class="footer-company-motto">Proyecto personal</p>
        <p class="footer-derechos">Derechos &copy; 2017</p>
    </footer>

    
    
