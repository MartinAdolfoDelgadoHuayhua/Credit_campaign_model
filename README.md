# 🎯 Credit Card Campaign Response Model

Este proyecto simula un caso real de **modelamiento de propensión a respuesta** para campañas de tarjeta de crédito, similar a los problemas enfrentados por áreas de CRM o marketing bancario.

---

## 🚀 Objetivos
- Construir un dataset sintético realista de campañas comerciales.
- Realizar un análisis exploratorio (EDA) con visualizaciones.
- Entrenar un modelo predictivo (Random Forest / XGBoost).
- Evaluar su desempeño con métricas de clasificación y lift chart.
- Interpretar los resultados con SHAP y métricas de negocio.

---

## 📂 Estructura del proyecto
- **data/**: contiene la base sintética `credit_campaign_sintetico.csv` y el diccionario de variables.
- **notebooks/**: flujo completo de análisis y modelamiento (EDA → model → evaluación).
- **src/**: scripts modulares (preprocesamiento, model training, evaluación, visualización).
- **outputs/**: figuras y resultados finales del modelo.

---

## 🧰 Tecnologías utilizadas
- Python 3.10+
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- SHAP

---

## 📈 Métricas de ejemplo
- ROC-AUC: 0.65  
- PR-AUC: 0.43  
- Lift (Top 10%): 1.6x

---

## 💡 Interpretación del modelo
El modelo permitió identificar que los clientes con:
- Mayor uso digital (`digital_usage`)
- Contactos recientes (`last_contact_days`)
- Historial de respuesta positiva (`prev_response`)
tienen una probabilidad significativamente mayor de responder a nuevas campañas.

---

## 🧾 Cómo ejecutar
```bash
pip install -r requirements.txt
jupyter notebook notebooks/01_credit_campaign_EDA_Modeling.ipynb
```

---
