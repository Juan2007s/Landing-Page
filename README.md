# Landing-Page
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Landing Page Bootstrap</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&display=swap" rel="stylesheet">
    <style>
        /* Aplica a fonte padrão */
        body {
            font-family: 'Roboto', sans-serif;
        }

        /* Navbar personalizada */
        .navbar {
            background-color: #000000;
        }
        .navbar-brand, .nav-link {
            color: white !important;
        }
        .nav-link:hover {
            color: #9db2ce !important;
        }

        /* Hero Section */
        .hero {
            background-color: #3239bf;
            color: white;
            padding: 80px 0;
        }
        .hero h1 {
            font-size: 3rem;
            font-weight: 500;
        }
        .hero p {
            font-size: 1.25rem;
        }
        .hero .btn {
            background-color: #000000;
            color: white;
            font-weight: 500;
        }
        .hero .btn:hover {
            background-color: #1f0fd7;
        }

        /* Seção Sobre */
        #sobre {
            background-color: #f4f6f7;
            padding: 60px 0;
        }
        #sobre h2 {
            font-size: 2.5rem;
            font-weight: 500;
        }
        #sobre p {
            font-size: 1.125rem;
            color: #555;
        }

        /* Seção de Serviços */
        #servicos {
            background-color: #ecf0f1;
            padding: 60px 0;
        }
        .card {
            border: none;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .card img {
            border-radius: 8px 8px 0 0;
        }
        .card-title {
            font-size: 1.25rem;
            font-weight: 500;
        }
        .card-text {
            font-size: 1rem;
            color: #010506;
        }

        /* Footer */
        footer {
            background-color: #1f0fd7;
            color: white;
            padding: 40px 0;
        }
        footer p {
            margin: 0;
        }
        footer ul {
            list-style: none;
            padding: 0;
        }
        footer ul li {
            margin-bottom: 10px;
        }
        footer ul li a {
            color: #f39c12;
            text-decoration: none;
        }
        footer ul li a:hover {
            text-decoration: underline;
        }

        /* Modal */
        .modal-content {
            border-radius: 10px;
        }

        /* Responsividade */
        @media (max-width: 767px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            .hero p {
                font-size: 1rem;
            }
            .card {
                margin-bottom: 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark">
        <a class="navbar-brand" href="#">Meu Projeto</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
                <li class="nav-item active">
                    <a class="nav-link" href="#">Início</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Sobre</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Serviços</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Contato</a>
                </li>
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="hero text-center">
        <div class="container">
            <h1 class="display-4">Bem-vindo ao Meu Site</h1>
            <p class="lead">Explore nossos serviços e saiba mais sobre o que fazemos.</p>
            <a href="#sobre" class="btn btn-lg">Saiba mais</a>
        </div>
    </header>

    <!-- Seção Sobre -->
    <section id="sobre" class="py-5">
        <div class="container">
            <h2 class="display-4 text-center">Sobre Nós</h2>
            <p class="text-center">Somos uma empresa dedicada a oferecer os melhores serviços para você. Conheça mais sobre nossa missão e valores.</p>
        </div>
    </section>

    <!-- Seção Serviços -->
    <section id="servicos" class="bg-light py-5">
        <div class="container">
            <h2 class="display-4 text-center">Nossos Serviços</h2>
            <div class="row">
                <div class="col-md-4">
                    <div class="card">
                        <img src="imagens/Capturar.PNG" class="-img-topcard" alt="Serviço 1">
                        <link rel="stylesheet" href="https://www.figma.com/proto/7l8CDj28yse5ONMO0RvhgV?node-id=0-1&t=tdJYh4kYNRVqAEvO-6">
                        <div class="card-body">
                            <h5 class="card-title">Serviço 1</h5>
                            <p class="card-text">PJ1.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card">
                        <img src="imagens/Capturar 2.PNG" class="card-img-top" alt="Serviço 2">
                        <div class="card-body">
                            <h5 class="card-title">Serviço 2</h5>
                            <p class="card-text">PJ2.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card">
                        <img src="imagens/Capturar 4.PNG" class="card-img-top" width="1200" alt="Serviço 3">
                        <div class="card-body">
                            <h5 class="card-title">Serviço 3</h5>
                            <p class="card-text">PJ3.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Meu Site | Todos os direitos reservados.</p>
        <ul>
            <li><a href="mailto:contato@meusite.com">contato@meusite.com</a></li>
            <li><a href="tel:+55 11 1234-5678">+55 11 1234-5678</a></li>
        </ul>
    </footer>

    <!-- Modal -->
    <button class="btn btn-danger" data-bs-toggle="modal" data-bs-target="#exemploModal">Abrir Modal</button>
    <div class="modal fade" id="exemploModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="exampleModalLabel">Título do Modal</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    Aqui está o conteúdo do seu modal.
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                    <button type="button" class="btn btn-primary">Salvar alterações</button>
                </div>
            </div>
        </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
</body>

</html>
