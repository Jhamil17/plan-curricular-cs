## 34. Exclusiones declaradas

Lo siguiente **no** forma parte del programa. El motivo es único en todos los casos: es infraestructura industrial, gestión o práctica operativa, no ciencia de la computación. Se adquiere en semanas de trabajo profesional; el contenido de este programa, no.

| Excluido | Por qué |
|---|---|
| Contenedores (Docker) como asignatura | Herramienta operativa. Sus mecanismos —namespaces, cgroups— están en SIS-501, que es donde corresponde entenderlos. |
| Infraestructura como código (Terraform, Kubernetes) | Configuración declarativa de proveedores. Cero contenido teórico transferible. |
| MLOps, orquestación de LLMs, bases vectoriales, pipelines RAG | Ingeniería de producto sobre modelos. Vida media de 18 meses. Los fundamentos están en IAP-602 e IAP-801. |
| SRE, SLIs/SLOs, chaos engineering | Práctica operativa. La inyección de fallos sí está incorporada, pero como método de evaluación en SIS-501, SIS-503 y SIS-701; **y la instrumentación de latencia, tasa de error y saturación también, pero como criterio de aprobación de la Prueba de Dominio en SIS-501 y SIS-701 (§15.7)**. Lo que queda fuera es el SRE como práctica de operación: guardias, error budgets, negociación de SLOs con terceros y gestión de incidentes. |
| Aprovisionamiento y gestión de costo de infraestructura | Función de compra. **El costo sí está incorporado, pero como cantidad analítica: acotar cómputo, memoria y precio por GPU-hora de un artefacto y derivar su escalamiento es análisis de complejidad en una segunda moneda (§15.8), no aprovisionamiento.** Queda fuera la elección de proveedor, la negociación de instancias reservadas y la optimización de facturación. |
| Emprendimiento, Lean Startup, métricas de producto | Fuera del dominio. |
| Desarrollo web y móvil | Fuera del dominio. |
| "Comunicación técnica" como asignatura independiente | Se ejercita en INV-801, INV-802 y en las defensas orales de los siete laboratorios integradores. Como curso separado es relleno. |
| Contribución open source obligatoria | Valiosa como actividad —figura en §22.3 y §23.5 como vía de revisión por pares real— pero no tiene criterio de dominio evaluable. Queda a criterio del estudiante. |
| Gestión de proyectos y metodologías ágiles | Fuera del dominio. |
| Certificaciones comerciales de proveedor | Acreditan operación de productos, no ciencia de la computación (§23.5). |

**Nota sobre el costo de estas exclusiones.** Son defendibles curricularmente y **caras en el mercado laboral inmediato**. Un egresado de este plan puede demostrar un kernel, un compilador y una cota de complejidad, y no haber desplegado nunca un servicio en producción. Eso es una decisión, no un descuido: lo excluido se aprende en semanas cuando se necesita, lo incluido no. Pero quien recorra este plan mientras trabaja debe saber que la brecha existe y que su trabajo la cubre —no que no exista.

---

