# Guía de uso

## Preparar la PC

Extrae el ZIP completo y ejecuta **S7FT.exe**. Si es necesario, abre **Ayuda → Preparar comunicaciones Siemens**, revisa la selección y completa los asistentes. Autoriza el acceso de administrador cuando Windows lo solicite y reinicia si se indica.

## Crear una conexión

Añade una conexión e introduce la IP, familia, rack, slot y puerto configurados para el PLC. En S7-1200/1500 suele utilizarse rack 0, slot 1 y puerto 102; confirma los valores de tu equipo.

En **Configurar mi NIC**, selecciona la Ethernet hacia el PLC. Si la PC ya tiene una dirección válida en esa subred, S7FT indica que no necesita otro ajuste. Cuando sea necesario, puedes añadir una IP secundaria temporal. Esta acción requiere administrador y no cambia la IP del PLC, DNS ni gateway de la PC.

## Consultar diagnóstico y eventos

Selecciona **Diagnóstico y eventos**. Pulsa **Actualizar interfaces**, elige la Ethernet y pulsa **Consultar PLC**.

En **Identificación** consulta las propiedades disponibles. En **Eventos de CPU**, selecciona una fila para ver el detalle completo. Utiliza **Copiar evento** o **Exportar diagnóstico** para guardar resultados. **Módulos reportados** muestra el inventario comunicado por el equipo.

Las fechas pertenecen al reloj del PLC. La consulta no ajusta su hora ni cambia su modo de funcionamiento.

## Memoria, bloques e inventario

Abre la vista correspondiente y ejecuta su acción de consulta. Para memoria y bloques comprueba compatibilidad, direcciones y permisos. Las escrituras y acciones de control son explícitas y pueden afectar al proceso conectado.

La consulta de inventario de red puede solicitar una comunidad de lectura: introduce la configurada por el administrador del equipo. S7FT no la guarda en el proyecto.

## Guardar y exportar

Guardar proyecto conserva conexiones y resultados. El analizador muestra las operaciones de S7FT; puedes buscar, copiar y exportar registros. Pausar el visor congela la presentación mientras la adquisición continúa.

Los controles generales actúan sobre conexiones guardadas; las consultas de diagnóstico e inventario son manuales. Seleccionar una vista no inicia operaciones. Revisa los informes antes de compartirlos: pueden contener datos de equipos.
