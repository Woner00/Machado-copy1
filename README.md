<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Machado Design | Sites Profissionais que Convertem Visitantes em Clientes</title>
    <meta name="description" content="Criamos seu site profissional + identidade visual em 7 dias. Design focado em resultados para pequenas empresas e empreendedores.">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #e74c3c;
            --accent: #3498db;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --gray: #95a5a6;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: #333;
        }
        
        /* HEADER COM CTA */
        header {
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
        }
        
        .logo span {
            color: var(--secondary);
        }
        
        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }
        
        nav a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 600;
            transition: color 0.3s;
        }
        
        nav a:hover {
            color: var(--secondary);
        }
        
        .cta-header {
            background: var(--secondary);
            color: white;
            padding: 0.7rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 700;
            transition: transform 0.3s, background 0.3s;
        }
        
        .cta-header:hover {
            background: #c0392b;
            transform: translateY(-2px);
        }
        
        /* HERO SECTION CONVERSORA */
        .hero {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 8rem 2rem 5rem;
            text-align: center;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 1.5rem;
            color: var(--primary);
        }
        
        .hero h1 span {
            color: var(--secondary);
        }
        
        .hero p {
            font-size: 1.3rem;
            color: var(--gray);
            margin-bottom: 2rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .hero-btns {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
            margin-bottom: 2rem;
        }
        
        .btn-primary {
            background: var(--secondary);
            color: white;
            padding: 1rem 2.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1.1rem;
            display: inline-block;
            transition: transform 0.3s, background 0.3s;
        }
        
        .btn-primary:hover {
            background: #c0392b;
            transform: translateY(-3px);
            color: white;
        }
        
        .btn-secondary {
            background: white;
            color: var(--primary);
            padding: 1rem 2.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1.1rem;
            border: 2px solid var(--primary);
            display: inline-block;
            transition: all 0.3s;
        }
        
        .btn-secondary:hover {
            background: var(--primary);
            color: white;
        }
        
        .hero-features {
            display: flex;
            justify-content: center;
            gap: 3rem;
            margin-top: 3rem;
            flex-wrap: wrap;
        }
        
        .feature {
            display: flex;
            align-items: center;
            gap: 0.7rem;
            color: var(--primary);
        }
        
        .feature i {
            color: var(--secondary);
        }
        
        /* SERVIÇOS COM PREÇOS */
        .services {
            padding: 5rem 2rem;
            background: white;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }
        
        .section-title p {
            color: var(--gray);
            max-width: 600px;
            margin: 0 auto;
        }
        
        .services-grid {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .service-card {
            background: #f8f9fa;
            border-radius: 10px;
            padding: 2rem;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
            border-top: 4px solid var(--accent);
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        .service-icon {
            font-size: 2.5rem;
            color: var(--accent);
            margin-bottom: 1.5rem;
        }
        
        .service-card h3 {
            color: var(--primary);
            margin-bottom: 1rem;
            font-size: 1.5rem;
        }
        
        .price {
            font-size: 2rem;
            color: var(--secondary);
            font-weight: 700;
            margin: 1rem 0;
        }
        
        .price-note {
            color: var(--gray);
            font-size: 0.9rem;
            margin-bottom: 1.5rem;
        }
        
        .service-features {
            list-style: none;
            margin: 1.5rem 0;
            text-align: left;
        }
        
        .service-features li {
            margin-bottom: 0.7rem;
            padding-left: 1.5rem;
            position: relative;
        }
        
        .service-features li:before {
            content: "✓";
            color: var(--secondary);
            position: absolute;
            left: 0;
            font-weight: bold;
        }
        
        /* PORTFÓLIO */
        .portfolio {
            padding: 5rem 2rem;
            background: #f8f9fa;
        }
        
        .portfolio-grid {
            max-width: 1200px;
            margin: 2rem auto 0;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .portfolio-item {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .portfolio-img {
            height: 200px;
            background: #ddd;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--gray);
            font-weight: 600;
        }
        
        .portfolio-content {
            padding: 1.5rem;
        }
        
        .portfolio-content h4 {
            color: var(--primary);
            margin-bottom: 0.5rem;
        }
        
        /* FORMULÁRIO DE CONTATO OTIMIZADO */
        .contact {
            padding: 5rem 2rem;
            background: white;
        }
        
        .contact-container {
            max-width: 800px;
            margin: 0 auto;
            background: #f8f9fa;
            padding: 3rem;
            border-radius: 10px;
        }
        
        .contact h2 {
            text-align: center;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }
        
        .contact-subtitle {
            text-align: center;
            color: var(--secondary);
            font-weight: 700;
            margin-bottom: 2rem;
            font-size: 1.2rem;
        }
        
        .contact-form {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }
        
        .form-group {
            display: flex;
            flex-direction: column;
        }
        
        .form-group label {
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: var(--primary);
        }
        
        .form-group input,
        .form-group select,
        .form-group textarea {
            padding: 1rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
        
        .form-group textarea {
            min-height: 150px;
        }
        
        .submit-btn {
            background: var(--secondary);
            color: white;
            border: none;
            padding: 1.2rem;
            font-size: 1.1rem;
            font-weight: 700;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
            margin-top: 1rem;
        }
        
        .submit-btn:hover {
            background: #c0392b;
        }
        
        /* FOOTER */
        footer {
            background: var(--primary);
            color: white;
            padding: 3rem 2rem 1.5rem;
            text-align: center;
        }
        
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .footer-logo {
            font-size: 2rem;
            font-weight: 700;
            margin-bottom: 1.5rem;
        }
        
        .footer-links {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin: 2rem 0;
            flex-wrap: wrap;
        }
        
        .footer-links a {
            color: white;
            text-decoration: none;
        }
        
        .footer-links a:hover {
            color: var(--secondary);
        }
        
        .copyright {
            margin-top: 2rem;
            padding-top: 1.5rem;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: rgba(255,255,255,0.7);
        }
        
        /* RESPONSIVO */
        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
                gap: 1rem;
                padding: 1rem;
            }
            
            nav ul {
                gap: 1rem;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero-btns {
                flex-direction: column;
                align-items: center;
            }
            
            .btn-primary, .btn-secondary {
                width: 100%;
                max-width: 300px;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <!-- HEADER COM CTA CLARO -->
    <header>
        <div class="nav-container">
            <div class="logo">Machado<span>Design</span></div>
            <nav>
                <ul>
                    <li><a href="#home">Início</a></li>
                    <li><a href="#services">Serviços</a></li>
                    <li><a href="#portfolio">Portfólio</a></li>
                    <li><a href="#contact">Contato</a></li>
                </ul>
            </nav>
            <a href="#contact" class="cta-header">ORÇAMENTO GRÁTIS</a>
        </div>
    </header>

    <!-- HERO SECTION CONVERSORA -->
    <section class="hero" id="home">
        <div class="hero-content">
            <h1>Seu Site Profissional Pronto em <span>7 Dias</span></h1>
            <p>Design + Desenvolvimento + Hospedagem. Tudo otimizado para converter visitantes em clientes.</p>
            
            <div class="hero-btns">
                <a href="#contact" class="btn-primary">
                    <i class="fas fa-calendar-check"></i> QUERO MEU SITE AGORA
                </a>
                <a href="#portfolio" class="btn-secondary">
                    <i class="fas fa-images"></i> VER PORTFÓLIO
                </a>
            </div>
            
            <div class="hero-features">
                <div class="feature">
                    <i class="fas fa-check-circle"></i>
                    <span>Design Responsivo</span>
                </div>
                <div class="feature">
                    <i class="fas fa-check-circle"></i>
                    <span>Otimizado para SEO</span>
                </div>
                <div class="feature">
                    <i class="fas fa-check-circle"></i>
                    <span>Suporte 30 Dias</span>
                </div>
            </div>
        </div>
    </section>

    <!-- SERVIÇOS COM PREÇOS CLAROS -->
    <section class="services" id="services">
        <div class="section-title">
            <h2>Serviços com Resultados</h2>
            <p>Soluções específicas para suas necessidades, com prazos e investimentos transparentes</p>
        </div>
        
        <div class="services-grid">
            <!-- Serviço 1 -->
            <div class="service-card">
                <div class="service-icon">
                    <i class="fas fa-laptop-code"></i>
                </div>
                <h3>Site Institucional</h3>
                <p>Presença online profissional para seu negócio</p>
                <div class="price">R$ 1.499</div>
                <div class="price-note">ou 12x de R$ 149</div>
                
                <ul class="service-features">
                    <li>Até 5 páginas</li>
                    <li>Design responsivo</li>
                    <li>Formulário de contato</li>
                    <li>Otimização básica SEO</li>
                    <li>Treinamento para uso</li>
                </ul>
                
                <a href="#contact" class="btn-secondary" style="width: 100%; text-align: center;">
                    QUERO ESTE PACOTE
                </a>
            </div>
            
            <!-- Serviço 2 -->
            <div class="service-card">
                <div class="service-icon">
                    <i class="fas fa-store"></i>
                </div>
                <h3>Loja Virtual</h3>
                <p>Comece a vender online hoje mesmo</p>
                <div class="price">R$ 2.499</div>
                <div class="price-note">ou 12x de R$ 249</div>
                
                <ul class="service-features">
                    <li>Até 50 produtos</li>
                    <li>Gateway de pagamento</li>
                    <li>Painel administrativo</li>
                    <li>Configuração de frete</li>
                    <li>Suporte por 60 dias</li>
                </ul>
                
                <a href="#contact" class="btn-primary" style="width: 100%; text-align: center;">
                    <i class="fas fa-shopping-cart"></i> CRIAR MINHA LOJA
                </a>
            </div>
            
            <!-- Serviço 3 -->
            <div class="service-card">
                <div class="service-icon">
                    <i class="fas fa-palette"></i>
                </div>
                <h3>Identidade Visual</h3>
                <p>Logo + Papelaria completa para sua marca</p>
                <div class="price">R$ 899</div>
                <div class="price-note">ou 10x de R$ 89</div>
                
                <ul class="service-features">
                    <li>Logo em 3 versões</li>
                    <li>Cartão de visita</li>
                    <li>Papel timbrado</li>
                    <li>Manual de aplicação</li>
                    <li>Arquivos editáveis</li>
                </ul>
                
                <a href="#contact" class="btn-secondary" style="width: 100%; text-align: center;">
                    CRIAR MINHA MARCA
                </a>
            </div>
        </div>
    </section>

    <!-- PORTFÓLIO -->
    <section class="portfolio" id="portfolio">
        <div class="section-title">
            <h2>Trabalhos Recentes</h2>
            <p>Projetos reais que ajudaram nossos clientes a crescer</p>
        </div>
        
        <div class="portfolio-grid">
            <div class="portfolio-item">
                <div class="portfolio-img" style="background: #a3d9ff;">
                    <span>LOJA DE SUPPLEMENTS</span>
                </div>
                <div class="portfolio-content">
                    <h4>Power Supplements</h4>
                    <p>Loja virtual com mais de 40 produtos. Aumentou vendas em 300% no primeiro mês.</p>
                </div>
            </div>
            
            <div class="portfolio-item">
                <div class="portfolio-img" style="background: #ffd6a3;">
                    <span>CLÍNICA ESTÉTICA</span>
                </div>
                <div class="portfolio-content">
                    <h4>Clínica Belle Santé</h4>
                    <p>Site institucional com agendamento online. Capta 15+ leads por semana.</p>
                </div>
            </div>
            
            <div class="portfolio-item">
                <div class="portfolio-img" style="background: #caffbf;">
                    <span>CONSULTORIA</span>
                </div>
                <div class="portfolio-content">
                    <h4>Consultoria Financeira Pro</h4>
                    <p>Site com blog integrado. Aumentou autoridade no mercado local.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- FORMULÁRIO DE CONTATO OTIMIZADO -->
    <section class="contact" id="contact">
        <div class="contact-container">
            <h2>Solicite Seu Orçamento</h2>
            <p class="contact-subtitle">Resposta em até 2 horas úteis • Orçamento gratuito • Sem compromisso</p>
            
            <form class="contact-form" id="contactForm">
                <div class="form-group">
                    <label for="name">Nome Completo *</label>
                    <input type="text" id="name" name="name" required>
                </div>
                
                <div class="form-group">
                    <label for="email">E-mail *</label>
                    <input type="email" id="email" name="email" required>
                </div>
                
                <div class="form-group">
                    <label for="phone">WhatsApp *</label>
                    <input type="tel" id="phone" name="phone" required placeholder="(11) 99999-9999">
                </div>
                
                <div class="form-group">
                    <label for="service">Qual serviço precisa? *</label>
                    <select id="service" name="service" required>
                        <option value="">Selecione uma opção</option>
                        <option value="site-institucional">Site Institucional</option>
                        <option value="loja-virtual">Loja Virtual (E-commerce)</option>
                        <option value="identidade-visual">Identidade Visual</option>
                        <option value="outro">Outro</option>
                    </select>
                </div>
                
                <div class="form-group">
                    <label for="message">Conte mais sobre seu projeto *</label>
                    <textarea id="message" name="message" required placeholder="Ex: Preciso de um site para meu restaurante com cardápio online e sistema de reservas..."></textarea>
                </div>
                
                <button type="submit" class="submit-btn">
                    <i class="fas fa-paper-plane"></i> ENVIAR SOLICITAÇÃO
                </button>
            </form>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <div class="footer-content">
            <div class="footer-logo">MachadoDesign</div>
            
            <div class="footer-links">
                <a href="#home">Início</a>
                <a href="#services">Serviços</a>
                <a href="#portfolio">Portfólio</a>
                <a href="#contact">Contato</a>
                <a href="https://wa.me/5511999999999" target="_blank">WhatsApp</a>
            </div>
            
            <p>Transformamos ideias em resultados digitais</p>
            <p>contato@machadodesign.com.br | (11) 9999-9999</p>
            
            <div class="copyright">
                &copy; 2023 Machado Design. Todos os direitos reservados.
            </div>
        </div>
    </footer>

    <script>
        // Form submission
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Simulação de envio
            const submitBtn = this.querySelector('.submit-btn');
            const originalText = submitBtn.innerHTML;
            
            submitBtn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> ENVIANDO...';
            submitBtn.disabled = true;
            
            // Simulação de delay
            setTimeout(() => {
                alert('Solicitação enviada com sucesso! Entraremos em contato em até 2 horas úteis.');
                submitBtn.innerHTML = originalText;
                submitBtn.disabled = false;
                document.getElementById('contactForm').reset();
            }, 1500);
        });
        
        // Smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Adiciona classe ao scroll para header
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if(window.scrollY > 100) {
                header.style.boxShadow = '0 5px 15px rgba(0,0,0,0.1)';
            } else {
                header.style.boxShadow = '0 2px 10px rgba(0,0,0,0.1)';
            }
        });
    </script>
</body>
</html># Machado-copy1
