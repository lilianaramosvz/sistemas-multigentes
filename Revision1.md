# Evidencia 2. Revisión 1

## Modelación de sistemas multiagentes con gráficas computacionales (Gpo 302)

**Actividad:** Evidencia 2. Revisión 1  
**Profesores:** Jesús I. Hernández | Iván A. Dounce | Javier F. Rendón | Eduardo Morales  

**Equipo:**
- José Emilio Inzunza García | A01644973  
- Yael García Morelos | A01352461  
- Juan Pablo Torres Guillén | A01743268  
- Liliana Ramos Vázquez | A01644969  
- Diana Fernanda Delgado Salcedo | A01644911  

**Fecha:** 10 de noviembre del 2025  

---

## Conformación del equipo

### José Emilio
- **Fortalezas:** Trabajo en equipo, excelente comunicación, trabajador, apertura al diálogo.  
- **Áreas de oportunidad:**  Procrastinación, concentración e impaciencia.

### Yael García Morelos
- **Fortalezas:** Comunicación activa, toma de decisiones, escucha activa, pensamiento crítico.  
- **Áreas de oportunidad:** Impuntualidad, procrastinación.  

### Juan Pablo
- **Fortalezas:** Comunicación clara, escucha activa, cooperación, compromiso.  
- **Áreas de oportunidad:**  Procrastinación, concentración.

### Liliana
- **Fortalezas:** Responsabilidad, compromiso, respeto, toma de decisiones, comunicación efectiva.  
- **Áreas de oportunidad:** Procrastinación, concentración.  

### Diana Fernanda
- **Fortalezas:** Perseverancia, responsabilidad, comunicación efectiva, respeto por los demás.  
- **Áreas de oportunidad:** Impaciencia, procrastinación, dispersión.  

---

En el transcurso de este periodo, esperamos adquirir conocimientos relevantes y realistas sobre el uso y aplicaciones de sistemas multiagentes, al ser un bloque donde el trabajo colaborativo es primordial, se espera el apoyo mutuo entre compañeros, una comunicación asertiva y delegación de responsabilidades de forma equitativa. Sabemos las dificultades que implica este periodo, por lo que es necesario para el cumplimiento de nuestros objetivos realizar investigaciones y usar herramientas que complementen lo visto en clase, siempre buscar realizar trabajos de calidad y evitar ser conformistas con nuestro desempeño, además de saber pedir ayuda cuando sea necesario.
---

## Herramientas de trabajo colaborativo

- **Repositorio en GitHub:** [https://github.com/lilianaramosvz/sistemas-multigentes.git](https://github.com/lilianaramosvz/sistemas-multigentes.git)  
- **Herramienta de comunicación:** [https://discord.gg/9RqkRpZa](https://discord.gg/9RqkRpZa)  

---

## Propuesta formal del reto

La agricultura, que es esencial para el desarrollo de la economía y la seguridad alimentaria, representa entre el 20 % y el 40 % de la producción mundial, según indica la Organización de las Naciones Unidas para la Alimentación y la Agricultura (FAO). 

Esta actividad se enfrenta a pérdidas importantes a causa de enfermedades, plagas y estrés en los cultivos. En México, donde la recolección rápida es necesaria para preservar el valor de productos de alta rotación como la mora o la fresa, y debido a que no hay suficiente personal formado y se depende de las inspecciones visuales, se complica el hallazgo oportuno, lo cual eleva los costos y hace que se desperdicien recursos. 

Para optimizar la productividad y el empleo eficaz de los insumos, se propone crear un sistema multiagente que sea capaz de detectar irregularidades en la vegetación y llevar a cabo acciones de manejo autónomamente. La simulación de este sistema permitirá valorar su efecto en la eficacia y reacción dentro del invernadero.

Para dar frente a nuestra problemática, se va a desarrollar un **digital environment** donde se simula un invernadero con agentes autónomos que permitan representar fenómenos biológicos, ambientales y operativos de manera realista, facilitando la detección temprana de anomalías en los cultivos y la optimización del uso de recursos.

En este entorno, los agentes como plantas, sensores, robots y un supervisor central, van a interactuar para monitorear las condiciones del invernadero, identificar posibles plagas o enfermedades y ejecutar acciones de manejo adecuadas. De esta manera, la simulación permitirá analizar el comportamiento colectivo de los agentes, evaluar estrategias de respuesta y demostrar cómo la automatización puede mejorar la eficiencia y productividad agrícola.

En el desarrollo de nuestra propuesta se espera la implementación de cuatro agentes:  

---

### 1. Planta (agente)
Representa el producto que se esté plantando en el invernadero con una arquitectura reactiva, su rol puede cambiar dependiendo de su estado, el cual puede variar dependiendo de la humedad, temperatura, nutrientes o presencia de anomalías como plagas. Interactúa con Sensores y Supervisor. 

**Capas:**
- Percepción: recibe estímulos del entorno.  
- Acción: actualiza su estado según el comportamiento definido.  

---

### 2. Sensor (agente)
Simula los dispositivos que monitorean condiciones ambientales y del cultivo, tienen una arquitectura reactiva. Su rol se basa en la recolección de datos de temperatura, humedad, color y textura de hojas, tras obtener los datos del entorno, los comunica al Supervisor.

**Capas:**
- Percepción: obtiene datos del entorno.  
- Acción: las comunica al supervisor.  

---

### 3. Supervisor (agente)
El rol del supervisor es detectar anomalías con base en la información transmitida por los sensores y decidir si se requiere intervención, su arquitectura es deliberativa, este desea mantener los cultivos saludables y minimizar pérdidas, para lograrlo, puede llegar a activar otros agentes.

- Creencias: estados actuales del invernadero y cada planta.  
- Deseo: mantener cultivos saludables y minimizar pérdidas.  
- Intenciones: ejecutar acciones correctivas al activar otros agentes.  

---

### 4. Robot (agente)
Con una arquitectura híbrida, ejecuta las decisiones del Supervisor, ya sea riego, fumigación o recolección, además, es el encargado de actualizar el estado de las plantas. 

**Capas:**
- Percepción: datos de sensores locales, detección del entorno como lo pueden ser obstáculos, posición actual, estado del cultivo objetivo o condiciones ambientales locales.  
- Acción: ejecuta movimientos y tareas físicas según las indicaciones del Supervisor.  

**Componentes BDI:**
- Creencias: información actualizada sobre su ubicación, zonas atendidas, estado de las plantas y órdenes recibidas.  
- Deseos: cubrir el invernadero en su totalidad, atender plantas afectadas y optimizar el uso de recursos.  
- Intenciones: priorizar áreas con mayor anomalías detectadas, planificar rutas eficientes para intervenir y coordinar con otros agentes (Robots) para evitar que haya conflictos en la realización de tareas.  

---

## Plan de trabajo

| Actividad | Responsable(s) | Fecha de inicio | Tiempo estimado | Fecha de entrega | Evidencia |
|------------|----------------|-----------------|------------------|------------------|------------|
| Evidencia 2. Revisión 1 | Equipo | 07/11/2025 | 2 horas | 10/11/2025 | Documento colaborativo |
| Evidencia 2. Revisión 2 | Equipo | 10/11/2025 | 4 horas | 17/11/2025 |  |
| Evidencia 2. Revisión 3 | Equipo | 17/11/2025 | 20 horas | 29/11/2025 |  |
| Evidencia 2. Entrega Final | Equipo | 29/11/2025 | 20 horas | 05/12/2025 |  |
| Evidencia 2. Presentación Final | Equipo | 05/12/2025 | 1 hora | 05/12/2025 |  |

---

**Documento colaborativo:**  
[https://docs.google.com/document/d/1SbTslzLJ_hNPMtW4_Dgy7Zhos4_iLNJA7Zx5ZNniF9I/edit?usp=sharing](https://docs.google.com/document/d/1SbTslzLJ_hNPMtW4_Dgy7Zhos4_iLNJA7Zx5ZNniF9I/edit?usp=sharing)
