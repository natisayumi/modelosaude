# modelosaude
# Site Softwares no Setor de Saúde

Este projeto contém um site web moderno e responsivo sobre softwares no setor de saúde, criado com HTML, CSS e JavaScript.

## Estrutura do Projeto

```
site-softwares-saude/
├── index.html          # Página principal
├── styles.css          # Estilos CSS
├── script.js           # JavaScript para interatividade
└── README.md           # Este arquivo
```

## Características do Site

### Design
- Layout moderno e responsivo
- Gradientes e animações suaves
- Navegação fixa com efeito blur
- Cards interativos com hover effects
- Timeline visual para processo de desenvolvimento
- Paleta de cores profissional (azul e roxo)

### Funcionalidades
- Navegação suave entre seções
- Menu mobile responsivo
- Animações de entrada dos elementos
- Contadores animados nas estatísticas
- Efeitos parallax sutis
- Transições e micro-interações

### Seções
1. **Hero** - Apresentação principal com estatísticas
2. **Introdução** - Contexto sobre softwares de saúde
3. **Exemplos** - Três tipos de software com cards detalhados:
   - Prontuário Eletrônico do Paciente (PEP)
   - Plataformas de Telemedicina
   - Sistemas de Gestão Hospitalar
4. **Desenvolvimento** - Timeline do processo de desenvolvimento
5. **Footer** - Informações finais

### Tecnologias Utilizadas
- HTML5 semântico
- CSS3 com Flexbox e Grid
- JavaScript ES6+
- Font Awesome para ícones
- Google Fonts (Inter)

### Responsividade
- Design mobile-first
- Breakpoints para tablet e desktop
- Menu hamburger para dispositivos móveis
- Layout adaptativo para diferentes tamanhos de tela

## Como Usar no Visual Studio Code

1. **Abrir o projeto:**
   - Abra o Visual Studio Code
   - Use `File > Open Folder` e selecione a pasta `site-softwares-saude`

2. **Visualizar o site:**
   - Instale a extensão "Live Server" no VS Code
   - Clique com o botão direito no arquivo `index.html`
   - Selecione "Open with Live Server"
   - O site abrirá automaticamente no navegador

3. **Editar o código:**
   - `index.html` - Estrutura e conteúdo
   - `styles.css` - Estilos e layout
   - `script.js` - Interatividade e animações

## Personalização

### Cores
As cores principais estão definidas no CSS e podem ser facilmente alteradas:
- Azul principal: `#2563eb`
- Roxo secundário: `#7c3aed`
- Verde para ícones: `#10b981`

### Conteúdo
Todo o conteúdo pode ser editado diretamente no arquivo `index.html`. As seções estão bem organizadas e comentadas.

### Animações
As animações podem ser ajustadas no arquivo `script.js` e nas classes CSS correspondentes.

## Compatibilidade
- Chrome, Firefox, Safari, Edge (versões modernas)
- Dispositivos móveis (iOS e Android)
- Tablets e desktops

## Otimizações Incluídas
- Carregamento otimizado de fontes
- Animações performáticas com CSS transforms
- Código JavaScript modular e eficiente
- Imagens e ícones otimizados
- SEO básico implementado

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Softwares no Setor de Saúde</title>
    <link rel="stylesheet" href="styles.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>
    <!-- Header -->
    <header class="header">
        <nav class="nav">
            <div class="nav-container">
                <div class="nav-logo">
                    <i class="fas fa-heartbeat"></i>
                    <span>NS health </span>
                </div>
                <ul class="nav-menu">
                    <li><a href="#introducao" class="nav-link">Introdução</a></li>
                    <li><a href="#exemplos" class="nav-link">Exemplos</a></li>
                    <li><a href="#desenvolvimento" class="nav-link">Desenvolvimento</a></li>
                </ul>
                <div class="nav-toggle">
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-container">
            <div class="hero-content">
                <h1 class="hero-title">Softwares no Setor de Saúde</h1>
                <p class="hero-subtitle">Transformando a medicina através da tecnologia</p>
                <div class="hero-stats">
                    <div class="stat">
                        <i class="fas fa-laptop-medical"></i>
                        <span class="stat-number">3</span>
                        <span class="stat-label">Tipos de Software</span>
                    </div>
                    <div class="stat">
                        <i class="fas fa-code"></i>
                        <span class="stat-number">6</span>
                        <span class="stat-label">Etapas de Desenvolvimento</span>
                    </div>
                    <div class="stat">
                        <i class="fas fa-hospital"></i>
                        <span class="stat-number">100%</span>
                        <span class="stat-label">Foco na Saúde</span>
                    </div>
                </div>
            </div>
            <div class="hero-visual">
                <div class="floating-card">
                    <i class="fas fa-stethoscope"></i>
                </div>
                <div class="floating-card">
                    <i class="fas fa-chart-line"></i>
                </div>
                <div class="floating-card">
                    <i class="fas fa-shield-alt"></i>
                </div>
            </div>
        </div>
    </section>

    <!-- Introdução -->
    <section id="introducao" class="section">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Introdução</h2>
                <div class="section-line"></div>
            </div>
            <div class="intro-content">
                <p class="intro-text">
                    O setor de saúde tem se beneficiado significativamente da evolução tecnológica, 
                    especialmente com a implementação de diversos tipos de softwares que otimizam 
                    processos, melhoram a qualidade do atendimento e facilitam a gestão de informações.
                </p>
                <p class="intro-text">
                    Este trabalho apresenta três exemplos reais de softwares utilizados no setor de saúde, 
                    explicando como contribuem para a eficiência, inovação e conectividade, além de 
                    detalhar o processo de desenvolvimento de um deles.
                </p>
            </div>
        </div>
    </section>

    <!-- Exemplos de Software -->
    <section id="exemplos" class="section section-dark">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Exemplos de Softwares no Setor de Saúde</h2>
                <div class="section-line"></div>
            </div>
            
            <div class="software-grid">
                <!-- PEP -->
                <div class="software-card" data-software="pep">
                    <div class="card-icon">
                        <i class="fas fa-file-medical"></i>
                    </div>
                    <h3 class="card-title">Prontuário Eletrônico do Paciente (PEP)</h3>
                    <p class="card-description">
                        Sistema digital que armazena todas as informações de saúde do paciente, 
                        incluindo histórico médico, resultados de exames e prescrições.
                    </p>
                    <div class="card-examples">
                        <div class="example-item">
                            <strong>ProDoctor</strong> - Sistema brasileiro para diversas especialidades
                        </div>
                        <div class="example-item">
                            <strong>Tasy (Philips)</strong> - Solução completa para grandes hospitais
                        </div>
                        <div class="example-item">
                            <strong>Amplimed</strong> - Com assinatura digital ICP-Brasil
                        </div>
                    </div>
                    <div class="card-benefits">
                        <div class="benefit">
                            <i class="fas fa-tachometer-alt"></i>
                            <span>Eficiência</span>
                        </div>
                        <div class="benefit">
                            <i class="fas fa-lightbulb"></i>
                            <span>Inovação</span>
                        </div>
                        <div class="benefit">
                            <i class="fas fa-network-wired"></i>
                            <span>Conectividade</span>
                        </div>
                    </div>
                </div>

                <!-- Telemedicina -->
                <div class="software-card" data-software="telemedicina">
                    <div class="card-icon">
                        <i class="fas fa-video"></i>
                    </div>
                    <h3 class="card-title">Plataformas de Telemedicina</h3>
                    <p class="card-description">
                        Sistemas que permitem consultas médicas remotas, diagnósticos à distância 
                        e monitoramento de pacientes através de tecnologias de comunicação.
                    </p>
                    <div class="card-examples">
                        <div class="example-item">
                            <strong>Conexa Saúde</strong> - Maior plataforma de telemedicina do Brasil
                        </div>
                        <div class="example-item">
                            <strong>Telemedicina Morsch</strong> - Especializada em telediagnóstico
                        </div>
                        <div class="example-item">
                            <strong>Portal Telemedicina</strong> - Sistema integrado completo
                        </div>
                    </div>
                    <div class="card-benefits">
                        <div class="benefit">
                            <i class="fas fa-tachometer-alt"></i>
                            <span>Eficiência</span>
                        </div>
                        <div class="benefit">
                            <i class="fas fa-lightbulb"></i>
                            <span>Inovação</span>
                        </div>
                        <div class="benefit">
                            <i class="fas fa-network-wired"></i>
                            <span>Conectividade</span>
                        </div>
                    </div>
                </div>

                <!-- SGH -->
                <div class="software-card" data-software="sgh">
                    <div class="card-icon">
                        <i class="fas fa-hospital"></i>
                    </div>
                    <h3 class="card-title">Sistemas de Gestão Hospitalar</h3>
                    <p class="card-description">
                        Softwares abrangentes que integram processos administrativos, financeiros 
                        e assistenciais de instituições de saúde.
                    </p>
                    <div class="card-examples">
                        <div class="example-item">
                            <strong>SOUL MV Hospitalar</strong> - Plataforma completa para grandes hospitais
                        </div>
                        <div class="example-item">
                            <strong>Philips Tasy</strong> - Sistema integrado com múltiplos módulos
                        </div>
                        <div class="example-item">
                            <strong>SisHOSP Core</strong> - Software nacional personalizável
                        </div>
                    </div>
                    <div class="card-benefits">
                        <div class="benefit">
                            <i class="fas fa-tachometer-alt"></i>
                            <span>Eficiência</span>
                        </div>
                        <div class="benefit">
                            <i class="fas fa-lightbulb"></i>
                            <span>Inovação</span>
                        </div>
                        <div class="benefit">
                            <i class="fas fa-network-wired"></i>
                            <span>Conectividade</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Processo de Desenvolvimento -->
    <section id="desenvolvimento" class="section">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Processo de Desenvolvimento</h2>
                <p class="section-subtitle">Sistema de Prontuário Eletrônico do Paciente (PEP)</p>
                <div class="section-line"></div>
            </div>

            <div class="development-timeline">
                <div class="timeline-item" data-step="1">
                    <div class="timeline-icon">
                        <i class="fas fa-clipboard-list"></i>
                    </div>
                    <div class="timeline-content">
                        <h3>Planejamento</h3>
                        <p>Definição de objetivos, identificação de stakeholders e levantamento de requisitos.</p>
                        <ul class="timeline-details">
                            <li>Pesquisa com usuários</li>
                            <li>Análise de fluxos de trabalho</li>
                            <li>Definição de arquitetura de segurança</li>
                            <li>Estabelecimento de cronograma</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item" data-step="2">
                    <div class="timeline-icon">
                        <i class="fas fa-palette"></i>
                    </div>
                    <div class="timeline-content">
                        <h3>Design</h3>
                        <p>Criação de interfaces intuitivas e definição da arquitetura técnica do sistema.</p>
                        <ul class="timeline-details">
                            <li>Design centrado no usuário</li>
                            <li>Layout responsivo</li>
                            <li>Funcionalidades-chave</li>
                            <li>Arquitetura em nuvem</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item" data-step="3">
                    <div class="timeline-icon">
                        <i class="fas fa-code"></i>
                    </div>
                    <div class="timeline-content">
                        <h3>Codificação</h3>
                        <p>Implementação do sistema usando tecnologias modernas e práticas ágeis.</p>
                        <ul class="timeline-details">
                            <li>Backend: Java/Spring Boot ou Node.js</li>
                            <li>Frontend: React.js ou Angular</li>
                            <li>Banco de dados criptografado</li>
                            <li>Metodologia Scrum</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item" data-step="4">
                    <div class="timeline-icon">
                        <i class="fas fa-bug"></i>
                    </div>
                    <div class="timeline-content">
                        <h3>Testes</h3>
                        <p>Validação completa do sistema incluindo funcionalidade, segurança e desempenho.</p>
                        <ul class="timeline-details">
                            <li>Testes de funcionalidade</li>
                            <li>Testes de segurança</li>
                            <li>Testes de desempenho</li>
                            <li>Validação em ambiente real</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item" data-step="5">
                    <div class="timeline-icon">
                        <i class="fas fa-rocket"></i>
                    </div>
                    <div class="timeline-content">
                        <h3>Implementação</h3>
                        <p>Implantação gradual do sistema com treinamento e suporte aos usuários.</p>
                        <ul class="timeline-details">
                            <li>Migração de dados</li>
                            <li>Rollout gradual</li>
                            <li>Treinamento de usuários</li>
                            <li>Suporte presencial</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item" data-step="6">
                    <div class="timeline-icon">
                        <i class="fas fa-tools"></i>
                    </div>
                    <div class="timeline-content">
                        <h3>Manutenção</h3>
                        <p>Suporte contínuo, atualizações e melhorias baseadas no feedback dos usuários.</p>
                        <ul class="timeline-details">
                            <li>Suporte técnico</li>
                            <li>Atualizações regulares</li>
                            <li>Conformidade contínua</li>
                            <li>Análise de dados</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-logo">
                    <i class="fas fa-heartbeat"></i>
                    <span>NS health</span>
                </div>
                <p class="footer-text">
                    Transformando a medicina através da tecnologia
                </p>
            </div>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>

// Navegação móvel
document.addEventListener('DOMContentLoaded', function() {
    const navToggle = document.querySelector('.nav-toggle');
    const navMenu = document.querySelector('.nav-menu');
    const navLinks = document.querySelectorAll('.nav-link');

    // Toggle menu mobile
    navToggle.addEventListener('click', function() {
        navMenu.classList.toggle('active');
        
        // Animação do hamburger
        const spans = navToggle.querySelectorAll('span');
        spans.forEach((span, index) => {
            if (navMenu.classList.contains('active')) {
                if (index === 0) span.style.transform = 'rotate(45deg) translate(5px, 5px)';
                if (index === 1) span.style.opacity = '0';
                if (index === 2) span.style.transform = 'rotate(-45deg) translate(7px, -6px)';
            } else {
                span.style.transform = 'none';
                span.style.opacity = '1';
            }
        });
    });

    // Fechar menu ao clicar em link
    navLinks.forEach(link => {
        link.addEventListener('click', () => {
            navMenu.classList.remove('active');
            const spans = navToggle.querySelectorAll('span');
            spans.forEach(span => {
                span.style.transform = 'none';
                span.style.opacity = '1';
            });
        });
    });

    // Scroll suave para seções
    navLinks.forEach(link => {
        link.addEventListener('click', function(e) {
            e.preventDefault();
            const targetId = this.getAttribute('href');
            const targetSection = document.querySelector(targetId);
            
            if (targetSection) {
                const headerHeight = document.querySelector('.header').offsetHeight;
                const targetPosition = targetSection.offsetTop - headerHeight;
                
                window.scrollTo({
                    top: targetPosition,
                    behavior: 'smooth'
                });
            }
        });
    });

    // Efeito de scroll no header
    window.addEventListener('scroll', function() {
        const header = document.querySelector('.header');
        if (window.scrollY > 100) {
            header.style.background = 'rgba(255, 255, 255, 0.98)';
            header.style.boxShadow = '0 2px 20px rgba(0, 0, 0, 0.1)';
        } else {
            header.style.background = 'rgba(255, 255, 255, 0.95)';
            header.style.boxShadow = 'none';
        }
    });

    // Animação de entrada dos elementos
    const observerOptions = {
        threshold: 0.1,
        rootMargin: '0px 0px -50px 0px'
    };

    const observer = new IntersectionObserver(function(entries) {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.style.opacity = '1';
                entry.target.style.transform = 'translateY(0)';
            }
        });
    }, observerOptions);

    // Observar elementos para animação
    const animatedElements = document.querySelectorAll('.software-card, .timeline-item, .section-header');
    animatedElements.forEach(el => {
        el.style.opacity = '0';
        el.style.transform = 'translateY(30px)';
        el.style.transition = 'all 0.6s ease';
        observer.observe(el);
    });

    // Efeito hover nos cards de software
    const softwareCards = document.querySelectorAll('.software-card');
    softwareCards.forEach(card => {
        card.addEventListener('mouseenter', function() {
            this.style.transform = 'translateY(-10px) scale(1.02)';
        });
        
        card.addEventListener('mouseleave', function() {
            this.style.transform = 'translateY(0) scale(1)';
        });
    });

    // Contador animado para estatísticas
    function animateCounter(element, target, duration = 2000) {
        let start = 0;
        const increment = target / (duration / 16);
        
        function updateCounter() {
            start += increment;
            if (start < target) {
                element.textContent = Math.floor(start);
                requestAnimationFrame(updateCounter);
            } else {
                element.textContent = target;
            }
        }
        
        updateCounter();
    }

    // Observar seção hero para iniciar contadores
    const heroObserver = new IntersectionObserver(function(entries) {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                const statNumbers = document.querySelectorAll('.stat-number');
                statNumbers.forEach(stat => {
                    const target = stat.textContent.includes('%') ? 100 : parseInt(stat.textContent);
                    if (!isNaN(target)) {
                        stat.textContent = '0';
                        setTimeout(() => {
                            animateCounter(stat, target);
                            if (stat.textContent === '100') {
                                stat.textContent = '100%';
                            }
                        }, 500);
                    }
                });
                heroObserver.unobserve(entry.target);
            }
        });
    }, { threshold: 0.5 });

    const heroSection = document.querySelector('.hero');
    if (heroSection) {
        heroObserver.observe(heroSection);
    }

    // Efeito parallax sutil no hero
    window.addEventListener('scroll', function() {
        const scrolled = window.pageYOffset;
        const heroVisual = document.querySelector('.hero-visual');
        if (heroVisual && scrolled < window.innerHeight) {
            heroVisual.style.transform = `translateY(${scrolled * 0.3}px)`;
        }
    });

    // Destacar link ativo na navegação
    window.addEventListener('scroll', function() {
        const sections = document.querySelectorAll('section[id]');
        const navLinks = document.querySelectorAll('.nav-link');
        
        let current = '';
        sections.forEach(section => {
            const sectionTop = section.offsetTop - 100;
            const sectionHeight = section.clientHeight;
            if (window.scrollY >= sectionTop && window.scrollY < sectionTop + sectionHeight) {
                current = section.getAttribute('id');
            }
        });

        navLinks.forEach(link => {
            link.classList.remove('active');
            if (link.getAttribute('href') === `#${current}`) {
                link.classList.add('active');
            }
        });
    });

    // Adicionar classe active ao CSS
    const style = document.createElement('style');
    style.textContent = `
        .nav-link.active {
            color: #2563eb !important;
        }
        .nav-link.active::after {
            width: 100% !important;
        }
    `;
    document.head.appendChild(style);

    // Efeito de digitação no título hero (opcional)
    function typeWriter(element, text, speed = 100) {
        let i = 0;
        element.textContent = '';
        
        function type() {
            if (i < text.length) {
                element.textContent += text.charAt(i);
                i++;
                setTimeout(type, speed);
            }
        }
        
        type();
    }

    // Smooth reveal para timeline items
    const timelineItems = document.querySelectorAll('.timeline-item');
    const timelineObserver = new IntersectionObserver(function(entries) {
        entries.forEach((entry, index) => {
            if (entry.isIntersecting) {
                setTimeout(() => {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateX(0)';
                }, index * 200);
            }
        });
    }, { threshold: 0.3 });

    timelineItems.forEach((item, index) => {
        item.style.opacity = '0';
        item.style.transition = 'all 0.6s ease';
        
        if (index % 2 === 0) {
            item.style.transform = 'translateX(-50px)';
        } else {
            item.style.transform = 'translateX(50px)';
        }
        
        timelineObserver.observe(item);
    });

    // Adicionar efeito de loading
    window.addEventListener('load', function() {
        document.body.style.opacity = '0';
        document.body.style.transition = 'opacity 0.5s ease';
        
        setTimeout(() => {
            document.body.style.opacity = '1';
        }, 100);
    });

    // Efeito de clique nos botões/links
    document.addEventListener('click', function(e) {
        if (e.target.matches('.nav-link, .software-card')) {
            // Criar efeito ripple
            const ripple = document.createElement('span');
            const rect = e.target.getBoundingClientRect();
            const size = Math.max(rect.width, rect.height);
            const x = e.clientX - rect.left - size / 2;
            const y = e.clientY - rect.top - size / 2;
            
            ripple.style.cssText = `
                position: absolute;
                width: ${size}px;
                height: ${size}px;
                left: ${x}px;
                top: ${y}px;
                background: rgba(37, 99, 235, 0.3);
                border-radius: 50%;
                transform: scale(0);
                animation: ripple 0.6s linear;
                pointer-events: none;
                z-index: 1000;
            `;
            
            e.target.style.position = 'relative';
            e.target.style.overflow = 'hidden';
            e.target.appendChild(ripple);
            
            setTimeout(() => {
                ripple.remove();
            }, 600);
        }
    });

    // Adicionar animação ripple ao CSS
    const rippleStyle = document.createElement('style');
    rippleStyle.textContent = `
        @keyframes ripple {
            to {
                transform: scale(4);
                opacity: 0;
            }
        }
    `;
    document.head.appendChild(rippleStyle);
});



