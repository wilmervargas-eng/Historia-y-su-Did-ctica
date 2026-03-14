# Historia-y-su-Did-ctica
metodologias activas
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HISTORIA Y SU DIDÁCTICA - Grupo #4</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        header {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            text-align: center;
            margin-bottom: 30px;
        }

        header h1 {
            color: #667eea;
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        header h2 {
            color: #764ba2;
            font-size: 1.5em;
            margin-bottom: 20px;
        }

        .info-box {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 5px;
            margin: 10px 0;
            border-left: 4px solid #667eea;
        }

        .team-photo {
            text-align: center;
            margin: 30px 0;
        }

        .team-photo img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            border: 5px solid white;
        }

        .team-members {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }

        .member-card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            text-align: center;
        }

        .member-card h3 {
            color: #667eea;
            margin-bottom: 10px;
        }

        .objective {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            margin: 30px 0;
        }

        .objective h2 {
            color: #667eea;
            margin-bottom: 15px;
            text-align: center;
        }

        .nav-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 30px 0;
            flex-wrap: wrap;
        }

        .nav-btn {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 50px;
            font-size: 1.1em;
            cursor: pointer;
            text-decoration: none;
            display: inline-block;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .nav-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.3);
        }

        .section {
            background: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            margin: 30px 0;
            display: none;
        }

        .section.active {
            display: block;
        }

        .section h2 {
            color: #667eea;
            font-size: 2em;
            margin-bottom: 20px;
            border-bottom: 3px solid #764ba2;
            padding-bottom: 10px;
        }

        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            margin: 30px 0;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }

        .skills {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
            border-left: 4px solid #764ba2;
        }

        .skills h3 {
            color: #764ba2;
            margin-bottom: 15px;
        }

        .skill-item {
            margin: 15px 0;
            padding-left: 20px;
        }

        .skill-item strong {
            color: #667eea;
        }

        .reflection {
            background: #fff3cd;
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
            border-left: 4px solid #ffc107;
        }

        .reflection h3 {
            color: #856404;
            margin-bottom: 15px;
        }

        .reflection ol {
            padding-left: 20px;
        }

        .reflection li {
            margin: 10px 0;
            color: #856404;
        }

        .methodology-info {
            margin: 20px 0;
        }

        .methodology-info h3 {
            color: #667eea;
            margin: 20px 0 10px 0;
        }

        .phases {
            background: #e7f3ff;
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
        }

        .phases h3 {
            color: #0066cc;
            margin-bottom: 15px;
        }

        .phase-item {
            margin: 15px 0;
            padding-left: 30px;
            position: relative;
        }

        .phase-item::before {
            content: attr(data-number);
            position: absolute;
            left: 0;
            top: 0;
            background: #667eea;
            color: white;
            width: 25px;
            height: 25px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
        }

        .purpose {
            background: #d4edda;
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
            border-left: 4px solid #28a745;
        }

        .purpose h3 {
            color: #155724;
            margin-bottom: 10px;
        }

        .purpose ul {
            list-style: none;
            padding-left: 0;
        }

        .purpose li::before {
            content: "✓ ";
            color: #28a745;
            font-weight: bold;
            margin-right: 5px;
        }

        footer {
            background: white;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            margin-top: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .back-btn {
            background: #6c757d;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin-bottom: 20px;
            font-size: 1em;
        }

        .back-btn:hover {
            background: #5a6268;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.8em;
            }
            
            header h2 {
                font-size: 1.2em;
            }
            
            .section {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- PÁGINA DE INICIO -->
        <div id="home" class="page">
            <header>
                <h1> HISTORIA Y SU DIDÁCTICA</h1>
                <h2>Módulo 7 - Grupo #4</h2>
                
                <div class="info-box">
                    <strong>Maestría en Educación de Bachillerato con mención en Pedagogía de las Ciencias Sociales</strong><br>
                    Cohorte II 2025 - Paralelo C2 - Modalidad en Línea
                </div>
                
                <div class="info-box">
                    <strong>Docente:</strong> MSc. Johanna Alexandra Bonilla Guachamín<br>
                    <strong>Año Lectivo:</strong> 2026-2027
                </div>
            </header>

            <div class="team-photo">
                <img src="https://i.imgur.com/placeholder.jpg" alt="Grupo #4 - Integrantes" onerror="this.src='data:image/svg+xml,%3Csvg xmlns=%22http://www.w3.org/2000/svg%22 width=%22800%22 height=%22400%22%3E%3Crect fill=%22%23667eea%22 width=%22800%22 height=%22400%22/%3E%3Ctext fill=%22white%22 x=%2250%25%22 y=%2250%25%22 text-anchor=%22middle%22 dy=%22.3em%22 font-size=%2224%22%3EGRUPO N° 4%3C/text%3E%3C/svg%3E'">
            </div>

            <div class="team-members">
                <div class="member-card">
                    <h3>CARTUCHE PUGLLA</h3>
                    <p><strong>BYRON VINICIO</strong></p>
                </div>
                <div class="member-card">
                    <h3>MERINO DELGADO</h3>
                    <p><strong>GABRIELA ISABEL</strong></p>
                </div>
                <div class="member-card">
                    <h3>TORRES ACOSTA</h3>
                    <p><strong>NARCISA STEFANIA</strong></p>
                </div>
                <div class="member-card">
                    <h3>VARGAS CAÑAR</h3>
                    <p><strong>WILMER HELI</strong></p>
                </div>
            </div>

            <div class="objective">
                <h2>🎯 OBJETIVO DEL SITIO WEB</h2>
                <p>Proporcionar recursos multimedia interactivos que faciliten la comprensión de procesos históricos mediante las metodologías de <strong>Debate Guiado</strong> y <strong>Juego de Roles</strong>, fomentando la participación activa y el pensamiento crítico de los estudiantes del 9no año de Educación Básica de la Unidad Educativa "Leónidas García".</p>
            </div>

            <div class="nav-buttons">
                <a href="#" class="nav-btn" onclick="showSection('debate')">💬 DEBATE GUIADO</a>
                <a href="#" class="nav-btn" onclick="showSection('roles')">🎭 JUEGO DE ROLES</a>
            </div>
        </div>

        <!-- METODOLOGÍA 1: DEBATE GUIADO -->
        <div id="debate" class="section">
            <button class="back-btn" onclick="showSection('home')">← Volver al Inicio</button>
            
            <h2>💬 METODOLOGÍA DE DEBATE GUIADO</h2>
            
            <div class="methodology-info">
                <p>El debate guiado es una estrategia de aprendizaje activo en la que los estudiantes analizan un tema histórico desde diferentes puntos de vista mediante la argumentación y el diálogo.</p>
            </div>

            <div class="video-container">
                <iframe src="https://www.youtube.com/embed/KM9Vo9vsXdU" 
                        title="Metodología Debate Guiado" 
                        frameborder="0" 
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                        allowfullscreen>
                </iframe>
            </div>

            <div class="skills">
                <h3>🎯 DESTREZAS A DESARROLLAR</h3>
                <div class="skill-item">
                    <strong>1. Pensamiento Crítico y Argumentativo</strong>
                    <ul>
                        <li>Capacidad para analizar diferentes perspectivas históricas</li>
                        <li>Construcción de argumentos basados en evidencia histórica</li>
                    </ul>
                </div>
                <div class="skill-item">
                    <strong>2. Comunicación Oral y Expresión</strong>
                    <ul>
                        <li>Desarrollo de habilidades para expresar ideas de forma clara y estructurada</li>
                        <li>Capacidad de escucha activa y respuesta a contraargumentos</li>
                    </ul>
                </div>
            </div>

            <div class="phases">
                <h3>📋 FASES METODOLÓGICAS</h3>
                <div class="phase-item" data-number="1">
                    <strong>Planteamiento del Problema</strong><br>
                    El docente formula una pregunta o problema relacionado con un hecho histórico para generar discusión.
                </div>
                <div class="phase-item" data-number="2">
                    <strong>Organización de Grupos</strong><br>
                    Los estudiantes se dividen en equipos y cada grupo adopta una postura o perspectiva diferente.
                </div>
                <div class="phase-item" data-number="3">
                    <strong>Investigación y Preparación</strong><br>
                    Los grupos investigan información utilizando fuentes históricas o material proporcionado por el docente.
                </div>
                <div class="phase-item" data-number="4">
                    <strong>Desarrollo del Debate</strong><br>
                    Cada grupo presenta sus argumentos, escucha a los demás y responde preguntas o contraargumentos.
                </div>
                <div class="phase-item" data-number="5">
                    <strong>Síntesis y Reflexión</strong><br>
                    El docente realiza una conclusión del debate y promueve la reflexión colectiva sobre lo aprendido.
                </div>
            </div>

            <div class="purpose">
                <h3>✨ PROPÓSITO</h3>
                <ul>
                    <li>Desarrollar pensamiento crítico</li>
                    <li>Fortalecer habilidades argumentativas</li>
                    <li>Promover participación activa</li>
                    <li>Fomentar el análisis de múltiples perspectivas históricas</li>
                </ul>
            </div>

            <div class="reflection">
                <h3>💭 PREGUNTAS DE REFLEXIÓN</h3>
                <p><em>Después de ver el video, responde:</em></p>
                <ol>
                    <li>¿Cómo contribuye el debate guiado a desarrollar el pensamiento crítico en los estudiantes de 9no año?</li>
                    <li>¿Qué desafíos podrías enfrentar al implementar esta metodología en un aula con recursos limitados y sin internet?</li>
                    <li>¿De qué manera el debate permite que los estudiantes conecten los hechos históricos con su realidad actual?</li>
                    <li>¿Cómo evaluarías la participación de estudiantes que son más tímidos o tienen dificultades para expresarse oralmente?</li>
                </ol>
            </div>
        </div>

        <!-- METODOLOGÍA 2: JUEGO DE ROLES -->
        <div id="roles" class="section">
            <button class="back-btn" onclick="showSection('home')">← Volver al Inicio</button>
            
            <h2>🎭 METODOLOGÍA DE JUEGO DE ROLES</h2>
            
            <div class="methodology-info">
                <p>El juego de roles es una estrategia didáctica en la que los estudiantes representan personajes o grupos sociales de un acontecimiento histórico para comprender diferentes perspectivas.</p>
            </div>

            <div class="video-container">
                <iframe src="https://www.youtube.com/embed/QTOf76p-HYg" 
                        title="Metodología Juego de Roles" 
                        frameborder="0" 
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                        allowfullscreen>
                </iframe>
            </div>

            <div class="skills">
                <h3>🎯 DESTREZAS A DESARROLLAR</h3>
                <div class="skill-item">
                    <strong>1. Empatía Histórica</strong>
                    <ul>
                        <li>Comprensión de diferentes perspectivas y contextos históricos</li>
                        <li>Capacidad de ponerse en el lugar de personajes históricos</li>
                    </ul>
                </div>
                <div class="skill-item">
                    <strong>2. Trabajo Colaborativo y Creatividad</strong>
                    <ul>
                        <li>Desarrollo de habilidades para trabajar en equipo</li>
                        <li>Creatividad en la representación y dramatización de hechos históricos</li>
                    </ul>
                </div>
            </div>

            <div class="phases">
                <h3>📋 FASES METODOLÓGICAS</h3>
                <div class="phase-item" data-number="1">
                    <strong>Selección del Acontecimiento Histórico</strong><br>
                    El docente elige un hecho relevante (por ejemplo, colonización o independencia).
                </div>
                <div class="phase-item" data-number="2">
                    <strong>Asignación de Roles</strong><br>
                    Los estudiantes se organizan en grupos y a cada grupo se le asigna un personaje o grupo social histórico.
                </div>
                <div class="phase-item" data-number="3">
                    <strong>Investigación del Personaje</strong><br>
                    Cada grupo investiga el contexto, intereses y postura de su personaje.
                </div>
                <div class="phase-item" data-number="4">
                    <strong>Simulación o Dramatización</strong><br>
                    Los estudiantes representan el papel asignado defendiendo sus ideas dentro de una situación histórica simulada.
                </div>
                <div class="phase-item" data-number="5">
                    <strong>Reflexión Final</strong><br>
                    Se realiza un análisis colectivo de las distintas perspectivas presentadas.
                </div>
            </div>

            <div class="purpose">
                <h3>✨ PROPÓSITO</h3>
                <ul>
                    <li>Comprender procesos históricos desde diferentes perspectivas</li>
                    <li>Desarrollar empatía histórica</li>
                    <li>Fomentar aprendizaje significativo</li>
                    <li>Promover el trabajo colaborativo</li>
                </ul>
            </div>

            <div class="reflection">
                <h3>💭 PREGUNTAS DE REFLEXIÓN</h3>
                <p><em>Después de ver el video, responde:</em></p>
                <ol>
                    <li>¿Cómo ayuda el juego de roles a que los estudiantes comprendan mejor los procesos históricos desde múltiples perspectivas?</li>
                    <li>¿Qué estrategias utilizarías para asignar roles de manera que todos los estudiantes participen activamente, considerando las diferentes personalidades del grupo?</li>
                    <li>¿De qué manera esta metodología fomenta la empatía histórica y la comprensión del contexto social de diferentes épocas?</li>
                    <li>¿Cómo adaptarías el juego de roles para que sea efectivo en un aula con 13 estudiantes y recursos materiales limitados?</li>
                </ol>
            </div>
        </div>

        <footer>
            <p><strong>GRUPO #4</strong> - Maestría en Educación de Bachillerato</p>
            <p>Unidad Educativa "Leónidas García" - 2026-2027</p>
        </footer>
    </div>

    <script>
        function showSection(sectionId) {
            // Ocultar todas las páginas/secciones
            document.getElementById('home').style.display = 'none';
            document.getElementById('debate').classList.remove('active');
            document.getElementById('roles').classList.remove('active');
            
            // Mostrar la sección seleccionada
            if (sectionId === 'home') {
                document.getElementById('home').style.display = 'block';
                window.scrollTo(0, 0);
            } else {
                document.getElementById(sectionId).classList.add('active');
                window.scrollTo(0, 0);
            }
        }

        // Inicializar mostrando la página de inicio
        document.addEventListener('DOMContentLoaded', function() {
            showSection('home');
        });
    </script>
</body>
</html>
