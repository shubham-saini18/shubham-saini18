:root {
  --bg-main: #0f172a;
  --bg-surface: #1e293b;
  --accent: #10b981;
  --text-main: #f8fafc;
  --text-muted: #94a3b8;
}

body {
  background-color: var(--bg-main);
  color: var(--text-main);
  font-family: 'Inter', -apple-system, sans-serif;
  margin: 0;
  padding: 0;
}

/* Minimal Hero Container */
.hero {
  height: 60vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  max-width: 800px;
  margin: 0 auto;
  padding: 0 2rem;
}

.hero h1 {
  font-size: 3rem;
  font-weight: 800;
  margin-bottom: 1rem;
}

.hero span.accent-text {
  color: var(--accent);
}

/* Responsive Project Grid */
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  max-width: 1000px;
  margin: 4rem auto;
  padding: 0 2rem;
}

.project-card {
  background-color: var(--bg-surface);
  border: 1px solid #334155;
  border-radius: 8px;
  padding: 1.5rem;
  transition: transform 0.2s ease, border-color 0.2s ease;
}

.project-card:hover {
  transform: translateY(-4px);
  border-color: var(--accent);
}
