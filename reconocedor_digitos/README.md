# Reconocimiento de dígitos mediante búsqueda heurística y algoritmos genéticos

Demostrador educativo en HTML + JavaScript (sin dependencias).

## Ejecutar
Abre `index.html` en el navegador (doble clic).

## Qué hace
- Carga PNG/JPG, lo reduce a 28×28, lo binariza, recorta y centra el trazo.
- Extrae rasgos: huecos, simetría, densidad por cuadrantes, extremos y componentes conexos.
- Grafo UNKNOWN → 0…9 con A*, BFS y DFS animados. Devuelve NULL si el coste mínimo supera τ.
- A*: g = coste de arista J(I,d); h = 0 (admisible y consistente), por lo que es óptimo.
- Evalúa 25 imágenes sintéticas y optimiza los pesos con un algoritmo genético (entrenamiento y validación separados).

## Limitaciones
Los prototipos se generan con una fuente del navegador; no es un clasificador entrenado con dígitos manuscritos (p. ej. MNIST).

## Publicar en GitHub Pages
Sube `index.html` y `README.md` a un repositorio, ve a Settings → Pages, elige la rama `main` y la carpeta `/ (root)`.
