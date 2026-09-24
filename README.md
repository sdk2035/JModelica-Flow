# JModelica-Flow 🧩🚁

**JModelica-Flow** es una interfaz visual *low-code* de código abierto diseñada para construir, simular y monitorear modelos dinámicos complejos de JModelica a través de componentes gráficos de arrastrar y soltar (drag-and-drop).

Inspirado en la reactividad de frameworks web como Genie/Stipple, **JModelica-Flow** permite a ingenieros y diseñadores conectar bloques físicos de hidrógeno ($\text{H}_2$), celdas de combustible y motores eléctricos, generando automáticamente los scripts de ejecución en Python (`pyjmi`) y tableros interactivos de control.

---

### 🌟 Funcionalidades Low-Code

* **Lienzo Visual Drag-and-Drop:** Arrastra componentes de la biblioteca libre (tanques $H_2$, convertidores DC/DC, rotores) y conéctalos visualmente.
* **Binding Reactivo en Tiempo Real:** Modifica parámetros de simulación (presión de $H_2$, carga de batería) con sliders y dials sin reiniciar el kernel de simulación.
* **Compilación Automática a PyJMI:** Genera código Python/JModelica optimizado en segundo plano a partir del diagrama de flujo.
* **Dashboard No-Code Integrado:** Visualizadores gráficos e indicadores de rendimiento térmico y eléctrico listos para usar.

---

### 🎛️ Comparativa de Enfoque Low-Code

| Concepto Genie / Stipple (Julia) | Equivalente Low-Code en JModelica-Flow | Función en el Diagrama del Helicóptero |
| :--- | :--- | :--- |
| **Reactive Canvas / UI** | **Web-Canvas (Vue/Node-RED Engine)** | Arrastrar la pila de hidrógeno y conectar al intercambiador térmico. |
| **Reactive State (`@app`)** | **JModelica Model State Manager** | Sincronización de variables de estado ($H_2$ flow, DC voltage) con la UI. |
| **Low-Code Plot Components** | **Auto-Generated Plotly Charts** | Gráficas instantáneas de consumo de hidrógeno vs. autonomía. |
