# Encuesta del canal

Formulario de 10 preguntas para que los 3 socios decidan cómo arranca el canal de historias reales animadas.

## Cómo funciona

1. Cada socio abre la página (GitHub Pages), responde y toca **Guardar mi voto en GitHub**.
2. Se abre GitHub con el voto ya escrito como un issue `[VOTO] Nombre`. El socio toca **Create**.
3. La acción `.github/workflows/registrar-voto.yml` guarda el voto en `data/votos.json`, responde al issue y lo cierra.
4. La sección **Resultados** de la página lee `data/votos.json` y los issues, y muestra los conteos en vivo.

- Para votar hace falta una cuenta gratis de GitHub.
- Un voto por cuenta: si alguien vota otra vez, cuenta su último voto.
- Para que solo cuenten ciertas cuentas, pon sus usuarios en `CONFIG.permitidos` dentro de `index.html`.
- El repositorio es público (GitHub Pages gratis lo necesita): cualquiera con el enlace puede ver los votos.
