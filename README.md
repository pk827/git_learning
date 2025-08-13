# Flask + React App

## Development
- Backend: Flask on http://localhost:5000
- Frontend: Vite React on http://localhost:5173 (proxy /api to backend)

### Start both servers
1. Install Python deps (user-level):
   - `pip3 install --user Flask Flask-Cors python-dotenv`
2. Frontend deps:
   - `cd frontend && npm install`
3. Run both:
   - `npm run dev:full` (from `frontend` directory)

### Test API
- Visit http://localhost:5173 and click "Call Flask API"
- Or: `curl http://localhost:5000/api/hello`

## Production build
- `cd frontend && npm run build` creates `frontend/dist` static assets.
- Serve Flask separately and static assets via any HTTP server or Vite preview:
  - `npm run preview`
