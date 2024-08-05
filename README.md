El Sistema de Registro de Correspondencia  se compone de flujos de procesos (bots) que supervisan tanto la bandeja de entrada como la de salida del correo de los colaboradores que hayan autorizado la herramienta. Esta opera mediante dos archivos de Google Sheets: "HOJA INICIO" y "PLANILLA".
En "HOJA INICIO" se configuran los parámetros de entrada para el registro de correos y se establece el enlace con el libro "PLANILLA", donde se registra la correspondencia enviada por externos al equipo de trabajo, así como los correos respondidos por el equipo que han autorizado el SRC. El archivo "PLANILLA" tiene 3 hojas: “Entradas”, “Salidas” y “Autorizaciones”.
Los colaboradores autorizan el acceso a sus correos desde "HOJA INICIO", por lo que esta se considera el punto de partida del sistema. Es importante destacar que ambos archivos son necesarios para cada proyecto o dependencia que requiera seguimiento de la correspondencia. Cada archivo debe estar ubicado en una ruta específica del servidor de Google Drive.
La verificación de las bandejas de entrada y salida de correo de los colaboradores se realizará diariamente en intervalos de tiempo específicos (en horas), los cuales se fijan al configurar la automatización.
Además, el SRC actualizará a diario el contador de días restantes para vencer el plazo de respuesta y lo registrará en "PLANILLA". Cuando el contador de plazo de respuesta sea igual o inferior a 1, se enviará una alerta vía correo electrónico a los líderes/coordinadores del proyecto o dependencia hasta que el sistema registre que el correo ha sido contestado. Una vez que el sistema detecte que el correo ha sido contestado, actualizará automáticamente el estado en "PLANILLA" y detendrá la cuenta regresiva del plazo de días para la respuesta del correo.
En caso de que el correo del cliente sea informativo y no sea necesaria la respuesta del equipo empresarial, solo los líderes/coordinadores del proyecto o dependencia podrán cambiar el estado del correo en "PLANILLA".
En capítulos posteriores se explicará con mayor profundidad el flujo de procesos del SRC y su configuración.
Cabe destacar que el SRC es un sistema cuyo objetivo principal es registrar las entradas y salidas de correos de los colaboradores; en ninguna circunstancia verificará/analizará el contenido de los correos recibidos/enviados por los colaboradores.
