## **Reflexión Final – Trabajo en Grupo**
#### **1. ¿Qué diferencia encontraron entre trabajar directamente en main y trabajar mediante ramas feature/*?**

Trabajar directamente en main genera una sensación de caos y presión constante, porque cualquier error afecta inmediatamente la versión "estable" del proyecto. En cambio, usar ramas feature/* nos dio libertad para experimentar, equivocarnos y ajustar sin miedo a romper lo que ya funciona. Además, el historial de commits queda mucho más limpio y comprensible, ya que cada rama agrupa cambios relacionados con una tarea específica.

#### **2. ¿Cuál consideran que es el propósito de la rama develop?**

develop actúa como un laboratorio de integración. Su propósito es reunir todas las funcionalidades terminadas (de las ramas feature) y probarlas juntas antes de pasarlas a main. Así nos aseguramos de que todo funcione en conjunto y de que la versión estable solo reciba cambios completamente validados. Es el puente entre el desarrollo diario y la entrega final.

#### **3. ¿Qué ventaja tiene que cada funcionalidad o cambio tenga su propia rama?**

Las principales ventajas son:

- Aislamiento: Sada cambio no interfiere con otros.
- Trazabilidad: Sabemos exactamente quién hizo qué y por qué.
- Facilidad para revisar código (pull requests) antes de integrar.
- Posibilidad de descartar o pausar una funcionalidad sin afectar el resto del proyecto.
- Paralelismo: Varios integrantes pueden trabajar al mismo tiempo sin pisarse.

#### **4. ¿Qué podría ocurrir en un proyecto si todos los integrantes modificaran directamente la versión estable?**

Sería un escenario de alto riesgo por las siguientes razones:

- Conflictos constantes y difíciles de resolver.
- La versión estable dejaría de ser confiable (se rompería con frecuencia).
- Pérdida de tiempo en arreglar errores urgentes en lugar de avanzar.
- Dificultad para identificar quién introdujo un error.
- Estrés y descoordinación en el equipo.

En el peor caso, se entregarían versiones defectuosas a los usuarios finales.

#### **5. ¿Cómo ayuda Markdown a mantener organizada la documentación dentro de un repositorio?**
Markdown permite escribir documentación clara, liviana y versionada junto al código. Al ser texto plano, se puede revisar en el historial de cambios, y al mismo tiempo se renderiza de forma legible en plataformas como GitHub. Facilita crear:

- README.md con instrucciones iniciales.
- CHANGELOG.md para registrar versiones.

Guías de contribución, wikis, etc.
Todo queda dentro del repositorio, accesible para todo el equipo y actualizable con cada commit.

#### **6. ¿Qué responsabilidad tiene la persona encargada de integrar los cambios del equipo?**

Su responsabilidad es garantizar que la integración no rompa el proyecto. Esto implica que debe: 

- Revisar que cada rama feature esté completa y probada.
- Resolver conflictos de fusión con cuidado.
- Verificar que la rama develop (y luego main) quede funcional después de cada merge.
- Asegurarse de que el historial sea claro y coherente.
- Comunicar al equipo el estado de la integración.
- Ser el guardián de la calidad y evitar que cambios inestables lleguen a producción.
