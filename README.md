# Programa-3-FCFS


## Requerimientos

1. **Diagrama de Cinco Estados:**
   a. Nuevo: Procesos creados pero aún no admitidos por el sistema.
   b. Listos: Procesos preparados para ejecutarse en cuanto sea su turno.
   c. Ejecución: Proceso actualmente en ejecución.
   d. Bloqueado: Proceso que no puede ejecutar hasta que cierto suceso ocurra.
   e. Terminado: Proceso excluido del grupo de procesos activos.

2. **Algoritmo de Cola de Listos:**
   - FCFS (First Come, First Serve): Procesos se ordenan según su llegada.

3. **Número de Procesos Inicial:**
   - Se pregunta el número de procesos inicial, pudiendo ser N procesos.

4. **Máximo de Procesos en Memoria:**
   - 5 procesos (Estados considerados: Ejecución, Bloqueado, Listo).

5. **Cola de Nuevos y Admisión de Procesos:**
   - Procesos sin cupo en la cola de listos se quedan en la cola de Nuevos, esperando admisión.

6. **Atributos de Procesos Generados (Punto 3):**
   a. Identificador de proceso único (Puede ser secuencial).
   b. Tiempo Máximo Estimado (aleatorio, validado entre 6 y 18).
   c. Datos para operación aleatoria, validando error aritmético.

7. **Teclas de Operaciones:**

   | Tecla | ¿Qué Indica?                             | ¿Qué Hace?                                                  |
   |-------|------------------------------------------|------------------------------------------------------------|
   | I     | Interrupción por Entrada/Salida          | Proceso en ejecución va a la cola de Bloqueados, espera y luego va a la cola de Listos. |
   | E     | Error                                    | Proceso en ejecución termina por error, pasa a procesos terminados. Se libera espacio en memoria. |
   | P     | Pausa                                    | Detiene la ejecución del programa.                           |
   | C     | Continuar                                | Reanuda el programa pausado con "P".                         |

8. **Visualización en Pantalla:**
   a. Número de Procesos en Estado Nuevo.
   b. Cola de Listos:
      - Identificador de Proceso.
      - Tiempo Máximo Estimado.
      - Tiempo Transcurrido.
   c. Proceso en Ejecución:
      - Todos los datos del proceso.
      - Tiempo ejecutado.
      - Tiempo restante por ejecutar.
   d. Cola de Bloqueados:
      - Identificador de Proceso.
      - Tiempo transcurrido en bloqueado.
   e. Procesos Terminados:
      - Identificador de Proceso.
      - Operación.
      - Resultado de la operación o "ERROR" en caso de terminación con error.
   f. Reloj (Contador General): Tiempo total transcurrido desde el inicio de la simulación.

9. **Cálculo de Tiempos:**
   a. Tiempo de Llegada.
   b. Tiempo de Finalización.
   c. Tiempo de Retorno.
   d. Tiempo de Respuesta.
   e. Tiempo de Espera.
   f. Tiempo de Servicio (TME si termina normal, tiempo transcurrido si no).

10. **Finalización del Programa:**
    - El programa termina cuando todos los procesos se han ejecutado.

11. **Datos al Finalizar:**
    - Todos los datos de cada proceso.
    - Incluyendo los tiempos marcados en el punto 9.
    - Número de programa y si terminó por error o normal.
