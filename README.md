# 🎯 CAPITRIVIAL - CEIP Capitulaciones

## 📋 Descripción
Juego de trivial educativo para Educación Primaria con 540 preguntas organizadas por ciclos y categorías.

## 📂 Archivos incluidos
- **capitrivial.html** - Archivo principal del juego
- **questions.js** - Base de datos con todas las preguntas
- **manifest.json** - Configuración para PWA
- **sw.js** - Service Worker para funcionamiento offline

## 🎮 Cómo usar

1. **Instalar**: Coloca todos los archivos en la misma carpeta
2. **Abrir**: Abre `capitrivial.html` en cualquier navegador
3. **Jugar**: 
   - Selecciona el ciclo (1º, 2º o 3º)
   - Elige número de equipos (2, 3 o 4)
   - ¡Empieza a jugar!

## 📊 Estructura de preguntas

### Ciclos incluidos:
- **Primer ciclo** (1º-2º): 180 preguntas
- **Segundo ciclo** (3º-4º): 180 preguntas  
- **Tercer ciclo** (5º-6º): 180 preguntas

### Categorías (30 preguntas cada una):
1. 📚 **Lengua** (Azul)
2. 🔢 **Matemáticas** (Verde)
3. 🔬 **Ciencias Naturales** (Amarillo)
4. 🌍 **Ciencias Sociales** (Rojo)
5. 🇬🇧 **Inglés** (Morado)
6. 🎨 **Arte y Cultura** (Naranja)

## ✏️ Cómo añadir o modificar preguntas

### Formato de una pregunta:
```javascript
{
    q: "Texto de la pregunta",
    answers: ["Opción 1", "Opción 2", "Opción 3", "Opción 4"],
    correct: 0  // Índice de la respuesta correcta (0-3)
}
```

### Ejemplo práctico:
```javascript
{
    q: "¿Cuánto es 2 + 2?",
    answers: ["3", "4", "5", "6"],
    correct: 1  // La respuesta correcta es "4" (índice 1)
}
```

### Pasos para modificar:
1. Abre el archivo `questions.js`
2. Busca el ciclo y categoría que quieres modificar
3. Añade o modifica preguntas siguiendo el formato
4. Guarda el archivo
5. Recarga el juego en el navegador

## 🎲 Mecánica del juego

1. Los equipos se turnan para tirar el dado (1-6)
2. Cada número corresponde a una categoría:
   - 1 = Lengua
   - 2 = Matemáticas
   - 3 = Ciencias Naturales
   - 4 = Ciencias Sociales
   - 5 = Inglés
   - 6 = Arte y Cultura
3. Responder correctamente da un "quesito" de esa categoría
4. Gana el primer equipo que consiga los 6 quesitos

## 🌐 PWA (Progressive Web App)

El juego funciona como PWA, lo que significa:
- ✅ Se puede instalar en tablets y pizarras digitales
- ✅ Funciona sin conexión a internet (offline)
- ✅ Experiencia como app nativa

## 💡 Características técnicas

- Diseño responsive (funciona en móviles, tablets y ordenadores)
- Interfaz amigable con Capitulín (mascota del cole)
- Sin dependencias externas (funciona offline)
- Fácil personalización de preguntas
- Sistema de preguntas no repetidas hasta agotar banco

## 🔧 Solución de problemas

**Problema**: No cargan las preguntas
- **Solución**: Asegúrate de que `questions.js` está en la misma carpeta que `capitrivial.html`

**Problema**: No funciona offline
- **Solución**: Abre el juego una vez con internet, luego funcionará sin conexión

**Problema**: Quiero cambiar los colores o el diseño
- **Solución**: Edita la sección `<style>` en el archivo `capitrivial.html`

## 📝 Notas importantes

- Las preguntas se seleccionan aleatoriamente
- No se repiten preguntas hasta agotar el banco de la categoría
- Cada partida puede ser diferente
- El juego está adaptado al nivel de cada ciclo

## 👨‍🏫 Para profesores

Este juego puede usarse para:
- Repasar contenidos de forma lúdica
- Competiciones entre grupos
- Evaluación formativa
- Actividad de fin de trimestre
- Juegos en pizarra digital

## 📧 Créditos

**CEIP Capitulaciones - Santa Fe (Granada)**
Desarrollado para el uso educativo en el centro

---

¡Que disfrutéis jugando y aprendiendo con Capitrivial! 🎉
