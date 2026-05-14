# Chatbot Web con Flask + OpenAI Mi primer proyecto portfolio: un chatbot web funcional desplegado en producción.
 
## Características
- ✨ Backend en Flask con API REST
- 🤖 Integración con OpenAI GPT-4
- 💬 Historial de conversación por sesión
- 🔒 Protección contra prompt injection
- 🚀 Desplegado en Render (URL pública)
## Requisitos
- Python 3.10+
- Cuenta OpenAI con API key 

## Instalación Local 
```bash git clone [tu-repo] cd chatbot-web python -m venv venv source venv/bin/activate # En Windows: venv\Scripts\activate pip install -r requirements.txt ``` 

## Configuración
Crea un archivo `.env` en la raíz: ``` OPENAI_API_KEY=sk-... ``` 

## Ejecutar localmente
```bash python app.py ``` 
Abre http://localhost:5000 en tu navegador.
## Desplegar en Render
1. Push a GitHub (sin .env)
2. Ve a render.com, crea "New Web Service"
3. Conecta tu repo 
4. Build:`pip install -r requirements.txt`
5. Start: `gunicorn app:app` 
6. Añade env var `OPENAI_API_KEY` en Render dashboard 
7. ¡Listo! Tu chatbot está en Internet 
## Stack Tecnológico 
- **Backend:** Flask 
- **API:** OpenAI GPT-4 
- **Frontend:** HTML/CSS/JavaScript vanilla 
- **Deployment:** Render + GitHub 
## Autor Juan Querol León — Curso IA para Web Developers