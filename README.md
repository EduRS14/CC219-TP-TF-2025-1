# Análisis de Sentimientos en Twitter con el Dataset Sentiment140

## 🎯 Objetivo del trabajo

El objetivo de este proyecto es desarrollar modelos de aprendizaje automático que permitan clasificar tweets según su polaridad (positiva o negativa) utilizando el conjunto de datos **Sentiment140**. A través de esta clasificación, se busca:

- Generar dashboards de vigilancia ante picos de sentimiento negativo.
- Apoyar al equipo de moderación en redes sociales.
- Contribuir a estudios sobre el impacto del discurso de odio en la salud mental.

## 👥 Alumnos participantes

- Alfredo Mauricio Aragón Ovalle – `u202210494`
- Tarik Gustavo Morales Oliveros – `u202210472`
- Rodrigo Alonso Ramírez Cesti – `u202210690`
- Eduardo José Rivas Siesquén – `u202216407`

## 📊 Descripción del dataset

El conjunto de datos utilizado es **Sentiment140**, creado por investigadores de Stanford. Contiene **1.6 millones de tweets** en inglés clasificados por polaridad:

- `0`: negativo  
- `2`: neutral  
- `4`: positivo

Para este proyecto se realizó una **binarización** de las etiquetas, creando una nueva columna `positive` (`True` para positivos, `False` para negativos).

**Columnas originales:**

- `target`: polaridad original
- `id`: ID del tweet
- `date`: fecha de publicación
- `query`: término de búsqueda
- `user`: autor del tweet
- `text`: contenido del tweet

Se eliminaron duplicados y se procesaron textos para normalizar datos. Finalmente, se usaron **TF-IDF** y **Regresión Logística** para clasificar los tweets.

📎 *(Puedes adjuntar el archivo PDF del informe completo aquí si se desea.)*

## ✅ Conclusiones

- El modelo alcanzó una **precisión del 78%**, con buen balance entre clases.
- LIME permitió entender los tokens clave que influían en la clasificación.
- Se evidenció mejor rendimiento clasificando tweets positivos que negativos, posiblemente por la ambigüedad o sarcasmo en los negativos.
- Se recomienda explorar modelos más potentes como **BERT** en futuras versiones, además de nuevas técnicas de preprocesamiento.

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](./LICENSE) para más detalles.
