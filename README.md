/* ==========================================================================
   Variables Globales y Configuración Base
   ========================================================================== */
:root {
    --primary-color: #2563eb;
    --primary-hover: #1d4ed8;
    --bg-color: #f8fafc;
    --card-bg: #ffffff;
    --text-color: #0f172a;
    --text-muted: #64748b;
    --border-color: #e2e8f0;
    --font-sans: 'Inter', system-ui, -apple-system, sans-serif;
    --radius: 8px;
    --transition: all 0.3s ease;
}

/* Modo Oscuro (Dynamic Theme) */
[data-theme="dark"] {
    --bg-color: #0f172a;
    --card-bg: #1e293b;
    --text-color: #f8fafc;
    --text-muted: #94a3b8;
    --border-color: #334155;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: var(--font-sans);
    background-color: var(--bg-color);
    color: var(--text-color);
    line-height: 1.6;
    transition: var(--transition);
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1.5rem;
}

/* ==========================================================================
   Componentes: Navbar
   ========================================================================== */
.navbar {
    background-color: var(--card-bg);
    border-bottom: 1px solid var(--border-color);
    position: sticky;
    top: 0;
    z-index: 100;
}

.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 70px;
}

.brand-logo {
    font-size: 1.5rem;
    font-weight: 700;
    color: var(--text-color);
    text-decoration: none;
}

.brand-logo span {
    color: var(--primary-color);
}

.nav-links {
    display: flex;
    list-style: none;
    gap: 2rem;
}

.nav-links a {
    text-decoration: none;
    color: var(--text-muted);
    font-weight: 500;
    transition: var(--transition);
}

.nav-links a:hover,
.nav-links a.active {
    color: var(--primary-color);
}

/* ==========================================================================
   Componentes: Botones
   ========================================================================== */
.btn {
    padding: 0.6rem 1.2rem;
    border-radius: var(--radius);
    font-weight: 600;
    cursor: pointer;
    border: none;
    transition: var(--transition);
}

.btn-primary {
    background-color: var(--primary-color);
    color: #ffffff;
}

.btn-primary:hover {
    background-color: var(--primary-hover);
}

.btn-secondary {
    background-color: transparent;
    border: 1px solid var(--border-color);
    color: var(--text-color);
}

.btn-outline {
    background: transparent;
    border: 1px solid var(--primary-color);
    color: var(--primary-color);
    text-decoration: none;
    display: inline-block;
}

/* ==========================================================================
   Secciones
   ========================================================================== */
.hero-section {
    padding: 5rem 0;
    text-align: center;
}

.hero-content h1 {
    font-size: 2.8rem;
    margin-bottom: 1rem;
}

.hero-content p {
    color: var(--text-muted);
    font-size: 1.2rem;
    max-width: 600px;
    margin: 0 auto 2rem;
}

.cta-buttons {
    display: flex;
    gap: 1rem;
    justify-content: center;
}

.features-section {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
    padding: 2rem 0 5rem;
}

.card {
    background-color: var(--card-bg);
    padding: 2rem;
    border-radius: var(--radius);
    border: 1px solid var(--border-color);
    transition: var(--transition);
}

.card:hover {
    transform: translateY(-5px);
}

.card h3 {
    margin-bottom: 0.8rem;
}

.card p {
    color: var(--text-muted);
}

.footer {
    text-align: center;
    padding: 2rem 0;
    border-top: 1px solid var(--border-color);
    color: var(--text-muted);
}
