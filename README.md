# 🚲 BiciMAD Predictor & Booking Assistant

A regression model and interactive application that forecasts urban bicycle demand based on location, weather conditions, and temporal data. Built as an end-to-end data science solution to optimize sustainable urban mobility management.

<p align="center">
  <a href="#-español">Español</a> • 
  <a href="#-english">English</a>
</p>

---

## 🇪🇸 Español

### 📝 Descripción del Proyecto
Plataforma predictiva e interactiva diseñada para optimizar la gestión del sistema de bicicletas compartidas **BiciMAD** en Madrid. La solución combina Machine Learning, datos meteorológicos y variables temporales para estimar la disponibilidad de bicicletas por estación, e incorpora un asistente de reservas y un cuadro de mando con analítica de uso.


🔗 **Documentación Interactiva de la Web:** [Visita nuestra web en Mintify / Documentation Link](https://vgg-14b474a8.mintlify.site)

Puedes acceder a la aplicación desplegada a través del siguiente enlace:
[🚀 Ir a BiciMAD Predictor](https://bicimad-bike-sharing-prediction.streamlit.app/)


### 🚀 Características Principales
* **Predicción de Disponibilidad (ML):** Simulación del estado de inventario de las estaciones basándose en variables climáticas reales (temperatura, humedad, precipitación), tipo de día (laborable/festivo) y franjas horarias.
* **Asistente de Reservas Integrado:** Sistema interactivo mediante ventanas emergentes (*pop-ups* de Streamlit) que valida la regla de antelación de 24 horas y genera localizadores únicos (`BM-XXXX`).
* **Persistencia de Datos:** Almacenamiento seguro e inmediato de las confirmaciones en un archivo local histórico (`booking_history.csv`).
* **Cuadro de Mando (Analítica):** Pestaña dedicada a la inteligencia de negocio que procesa el histórico de reservas con **Pandas** y muestra gráficos de barras y líneas adaptados a la paleta de colores corporativa (tonos azules apagados).

### 🛠️ Tecnologías Utilizadas
* **Frontend:** Streamlit
* **Análisis de Datos & Gráficos:** Pandas, Folium, Streamlit Components
* **Machine Learning:** Scikit-Learn (Random Forest Regressor)

### 👩‍💻 Mi contribución al proyecto

Este proyecto fue desarrollado de forma colaborativa. Mi aportación principal se centró en el modelado predictivo y en la integración final de la aplicación:

* Entrenamiento y comparación de diferentes modelos de regresión.
* Evaluación mediante métricas MAE, RMSE y R².
* Selección de **Random Forest Regressor** como modelo con mejor rendimiento.
* Exportación del pipeline entrenado mediante `joblib` para su utilización en la aplicación.
* Integración y mejora de funcionalidades en la aplicación desarrollada con Streamlit.
* Optimización de la interfaz, el mapa de estaciones y la experiencia de usuario.
* Resolución de conflictos de Git durante la integración de las distintas ramas del equipo.

El historial completo de commits y pull requests del repositorio permite consultar y verificar estas contribuciones.
  

---

## 🇬🇧 English

### 📝 Project Description
An interactive, predictive platform engineered to optimize and manage Madrid's **BiciMAD** bike-sharing network. This project merges **Machine Learning** (powered by a Random Forest algorithm) to anticipate bike availability, with an **Intelligent Booking Assistant** that allows users to secure future trips while enabling administrators to monitor real-time business analytics.

🔗 **Live Web Documentation:** [Visit our Mintify Web / Documentation Link](https://vgg-14b474a8.mintlify.site)

You can access the deployed application at the following link:
[🚀 Go to BiciMAD Predictor](https://bicimad-bike-sharing-prediction.streamlit.app/)

### 🚀 Key Features
* **Availability Prediction (ML):** Station inventory simulations based on real-time weather parameters (temperature, humidity, precipitation), day status (weekday/holiday), and specific time slots.
* **Integrated Booking Assistant:** An interactive modal workflow (Streamlit dialogs) that enforces a 24-hour advance notice policy and issues unique booking IDs (`BM-XXXX`).
* **Data Persistence:** Instantaneous, secure storage of user confirmations into a permanent local file (`booking_history.csv`).
* **Analytics Dashboard:** A business intelligence tab that processes data with **Pandas**, rendering customized line and bar charts aligned with the platform’s corporate color scheme (muted blue tones).

### 🛠️ Technologies Used
* **Frontend:** Streamlit
* **Data Analysis & Visualization:** Pandas, Folium, Streamlit Components
* **Machine Learning:** Scikit-Learn (Random Forest Regressor)

### 👩‍💻 My Contribution to the Project

This project was developed collaboratively. My main contribution focused on predictive modeling and the final integration of the application:

* Training and comparison of different regression models.
* Evaluation using MAE, RMSE, and R² metrics.
* Selection of **Random Forest Regressor** as the best-performing model.
* Export of the trained model using `joblib` for integration into the application.
* Development of functional and visual improvements in the Streamlit application.
* Optimization of the interface, station map, and user experience.
* Resolution of Git conflicts during the integration of the team’s branches.

These contributions can be verified through the repository’s commit and pull request history.


---

## 💻 Instalación y Uso / Installation & Setup

1. **Clonar el repositorio / Clone the repository:**
   ```bash
   git clone https://github.com/elenacarino-max/bike-sharing-prediction.git
   cd bike-sharing-prediction
   pip install -r requirements.txt
   streamlit run app/app.py
  
