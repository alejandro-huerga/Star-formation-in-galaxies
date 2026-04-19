# Análisis de Formación Estelar - Modelo de Capas Cilíndricas

Este proyecto implementa un modelo numérico avanzado para simular la evolución química y dinámica de una galaxia (enfocado en un anillo local a 8 kpc). Utiliza un sistema de ecuaciones diferenciales acopladas para rastrear la masa de gas, la masa estelar y la evolución de la energía turbulenta.

## 🌌 Descripción del Proyecto
El código resuelve la evolución de:
- **Masa de Gas ($M_g$):** Considerando la caída de gas externo (*infall*) y el consumo por formación estelar.
- **Masa Estelar ($M_s$):** Siguiendo la tasa de formación estelar (SFR) a lo largo del tiempo.
- **Energía ($E$):** Balance entre la inyección por supernovas y la disipación.

### Parámetros Físicos Clave:
- **Eficiencia de Formación Estelar (SFE):** Basada en una distribución log-normal.
- **Estabilidad del Disco:** Cálculo del parámetro $Q$ de Toomre y el ratio Virial.
- **Geometría:** Modelo de altura de escala ($z_0$) y densidad central ($\rho_0$).

## 🛠️ Requisitos e Instalación
Para ejecutar el notebook `Analysis_star_formation_1.ipynb`, se recomienda usar un entorno de Python 3.10+ (como Conda).

Las librerías necesarias son:
- `numpy`: Cálculos numéricos.
- `scipy`: Integración de ecuaciones diferenciales (ODE).
- `matplotlib`: Generación de gráficas de diagnóstico.
- `astropy`: Gestión de unidades físicas y constantes constantes astronómicas.

## 📈 Gráficas Generadas
El código produce automáticamente una figura con 3 paneles:
1. Evolución de masas ($M_g$, $M_s$).
2. Evolución de la velocidad de dispersión ($\sigma$).
3. Tasa de formación estelar (SFR).
