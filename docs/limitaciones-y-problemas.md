# Compatibilidad y ayuda

## El PLC aparece, pero no responde a todas las consultas

Detectar un equipo no implica acceso a todas sus funciones. Comprueba familia de CPU, firmware, dirección IP, permisos y configuración. Un equipo puede ofrecer identificación y rechazar otras operaciones.

## No aparecen interfaces o no se puede consultar

Completa **Ayuda → Preparar comunicaciones Siemens**, reinicia si el asistente lo solicita y vuelve a **Actualizar interfaces**. Selecciona la Ethernet conectada al PLC. Comprueba cableado, subred y acceso de red.

Si Windows rechaza el permiso de administrador o la instalación informa un error, conserva el mensaje y consulta [soporte](../SUPPORT.md).

## Estado y fechas

RUN/STOP corresponde al estado leído. Un fallo de comunicación no significa que la CPU esté en STOP, ERROR o STANDBY. Las fechas de eventos provienen del reloj del PLC y no se ajustan al consultar.

Un listado vacío de módulos o eventos no confirma que el equipo carezca de ellos. La disponibilidad depende del PLC y sus permisos.

## Memoria y programas

El acceso a memoria requiere direcciones y protección compatibles. S7FT no habilita PUT/GET ni modifica automáticamente la configuración de los bloques.

Las funciones de bloques y respaldo binario se orientan a S7-300/400 compatibles y no recuperan un proyecto fuente. No incluye descarga de proyectos TIA S7-1200/1500, edición LAD/FBD/SCL, actualización de firmware ni programación F-CPU.

## Analizador

Registra operaciones realizadas por S7FT. No es un monitor pasivo de todo el tráfico de la red. Pausar el visor no detiene la adquisición.
