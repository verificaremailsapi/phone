
    # Verificar Teléfonos ®

     La API de Verificar teléfonos permite validar en tiempo real la veracidad de un número de teléfono. La API de Verificar teléfonos permite validar en tiempo real la veracidad de un número de teléfono. 
      Disponemos de 3 métodos para verificar los números de teléfono:
      -  Verificación HLR
      -  Verificación MNP
      -  Verificación sintáctica
      
      Para las validaciones de teléfonos móviles (HLR, MNP) utilizamos un método que consulta las redes móviles para determinar el operador y ver si el número está activo. Ofrecemos información sobre la portabilidad (red actual y red emisora). 
      
      Con nuestro servicio de verificación podrás mantener tu base de datos limpia eliminando todos los números inactivos, falsos y comunicarse con tus clientes de forma fiable. Todas estas verificaciones se realizan sin que el usuario reciba una llamada o SMS.
      
      El API es capaz de identificar el tipo de número diferenciando entre móvil y fijo. Mostrando el resultado para cada una de las verificaciones.
      
      Puedes verificar los números de teléfono en tu Web o aplicación con nuestra API, a través de nuestra aplicación Web, con las integraciones de Zapier o nuestro Widget. Todo en tiempo real.


    
    ## Verificaciones Masivas
    Para verificar un volumen elevado  de teléfonos, debemos agrupar los números en un fichero CSV, TXY o Excel. Cada fila debe contener un teléfono con el prefijo internacional.


    ## Fácil Integración
    Hablamos tu lenguaje de programación. Las llamadas a nuestra API están disponibles para PHP, Python,
    Node.js, y .net. Puedes utilizar <a href="https://www.verificaremails.com/servicio-verificar-emails/como-utilizar-zapier-verificar-emails/" target="_blank">**la integración con Zapier**</a> para automatizar las validaciones de números de teléfono sin necesidad de programar. 
    
    Si lo prefieres puedes utilizar <a href="https://www.verificaremails.com/kb/utilizar-postman-para-el-api-de-verificaremails/" target="_blank">**Postman con ejemplos de código**</a> para la mayoría de los lenguajes de programación.

    # Empezar
    En los siguientes puntos descubre como utilizar Validaremails para verificar de forma
    sencilla, económica y eficaz tus números de teléfono y obtener informes detallados de
    tus contactos.

    ## Crear una cuenta en Verificaremails ®
    Para utilizar el servicio deberás <a href="https://dashboard.verificaremails.com/app/public/register" target="_blank">**crear una cuenta gratuita en Verificaremails**</a>.

    ![Sign Up Page](static/images/signup.png)

    ## Verificar Números de Teléfono
    Una vez hayas creado tu cuenta gratuita, debes iniciar sesión para empezar a utilizarla
    el servicio de *Verificaremails ®*. 

    Si deseas verificar teléfonos de forma individual, solo debes introducir el número de teléfono en el campo **Petición Rápida**. 
    
     ![Bulk Email Verification](static/images/telefonos_peticion_rapida.png)
    
    Si lo que deseas es verificar un listado de números de teléfono, lo más rápido es que utilices la verificación de ficheros. Solo tienes que arrastrar el fichero a la caja naranja que encontrarás en la pantalla principal y seleccionar en que columna se encuentran los mails. La primera columna es la 1 y así sucesivamente. 
    
    Puedes subir ficheros en formato Excel, TXT y CSV. Lo importante es que la información este organizada en columnas. Antes de verificar un fichero asegúrate que la información esté organizada en columnas ya que por cada registro te descontaremos un crédito de tu cuenta independientemente del valor que verifiquemos.
    Como mecanismo de seguridad, si no hay más de un 50% de números de teléfono en la columna. **No lanzaremos la verificación**. 
    
    Si durante la subida del fichero se muestra un error, en la mayoría de las ocasiones se debe a un error en el formato de los datos. Asegúrate que la información está bien tabulada. Si aun necesitas ayuda, puedes contactarnos por el chat que encontrarás en la parte inferior derecha.

    ![Bulk Email Verification](static/images/bulk-email-verification.png)

    ## Verificar Números de Teléfono utilizando el API para Validar Teléfono ®
    Puedes utilizar nuestra API para validar los números de teléfono de tus aplicaciones en tiempo real.
    Utilizar nuestra API solo requiere unas pocas líneas de código. Para más detalles
    visita la sección [**API Desarrolladores**](#section/Empezar/API-Desarrolladores).
    Antes de poder utilizar el API debes crear una ;-) 
    
    Dirrigete a la sección **APIs** y selecciona **+Crear nueva API**. Asegúrate que estás en la sección del servicio que deseas utilizar.
    Seleccionando el icono del "ojo" verás los últimos registros validados. Seleccionando el icono de la "rueda" puedes cambiar la clave del API y limitar las peticiones totales, peticiones por minuto que puede recibir el API o el estado de la misma.
    
    Recuerda que puedes utilizar el API en tus desarrollos, en las integraciones con Zapier, nuestro <a href="https://www.verificaremails.com/kb/como-utilizar-el-widget-para-validar-formularios/" target="_blank">Widget</a> o la verificación con terceras aplicaciones como Excel o Google Sheets.



    Nuestra API permite validar de forma individual direcciones de teléfonos o validar
    listas de números subiendo ficheros a nuestra plataforma.

    # Como funciona Verificar Emails ®
    Disponemos de 3 mecanismos para verificar los números de teléfono. La verificación más precisa es la Verificación de números HLR, la que proporciona un grado intermedio de precisión es la verificación de números MNP. La verificación más simple es la que solo verifica de forma sintáctica el número de teléfono.
    
    Los 3 mecanismos, utilizan los mismos campos, la principal diferencia es en el número de campos devueltos y la precisión de la formación.
    
    **Verificación teléfonos HLR**
    
    Es el método de verificación de números de teléfono más preciso. Permite saber si un número está actualmente conectado a la red móvil. Validar el estado y los detalles de los números de móvil en tiempo real. El término «HLR» significa Home Location Register, una base de datos central que contiene detalles de cada abonado de telefonía móvil autorizado por una red GSM. La búsqueda en el HLR, por tanto, es una forma de acceder a esta información para garantizar la validez y disponibilidad de un número de móvil. Esta tecnología ofrece el grado más alto de precisión, como contra partida tiene el coste de verificación más alto.
    
    **Verificación teléfonos MNP**
    

    La verificación de búsqueda de la portabilidad del número de móvil (MNP) es un proceso utilizado para validar los números y garantizar la identificación exacta de los proveedores de red.
    
    La búsqueda MNP ayuda a determinar el operador actual de un número de móvil. Las empresas utilizan esta información para enrutar los mensajes SMS de forma precisa y rentable.
    
    La verificación MNP ofrece un compromiso entre el grado de precisión y el coste de cada validación. Se puede utilizar como mecanismo indirecto para la verificación de teléfonos.
    
    **Verificación sintáctica de números de teléfono**
    

    La verificación sintáctica de los números de teléfono garantiza la exactitud y coherencia de los números de teléfono.
    
    Consiste en comprobar la estructura y el formato del número de teléfono para asegurarse de que se ajusta a un patrón o conjunto de normas específico. Este proceso ayuda a identificar y corregir errores.
    
    Este tipo de verificación es la más económica, pero a costa de obtener menos información de los números verificados.
    
    
     ![Sign Up Page](static/images/tipos_verificacion_telefonos.png)


    # Verificar Ficheros
    *Verificar Emails ®* ofrece distintas formas de importar los ficheros de contactos 
    para su verificación. Puedes subir ficheros CSV, XLS, XLSX y TXT 
    desde tu ordenador local.

    ![File Upload](static/images/file-upload.png)

    Para subir un fichero desplázate a la sección **_Dashboard_** o **_Validación_**. Utilizando la caja naranja, selecciona los ficheros a verificar. También puedes arrastrar y soltar los ficheros
    de tu ordenador.

  

    Una vez los ficheros han sido subidos, se harán visibles en la sección **_FICHEROS SUBIDOS_**.
    Los nuevos ficheros iniciarán su validación de forma automática. **IMPORTANTE:** Una vez inicies el proceso de validación, no se puede cancelar. Asegúrate que los emails están correctamente tabulados en tu fichero. Una vez finalice el proceso de verificación recibirás un mensaje de emails para proceder a la descarga del fichero verificado.
   

    Mientras subes un fichero asegura te que se cumplen las condiciones:

    * Los teléfonos están en una única columna columna.
    * Los teléfonos deben aparecer en la misma columna en las distintas filas.
    * Recomendamos que la lista sea inferior a 250.000 teléfonos. Para optimizar la velocidad recomendamos listas inferiores a 100.000 registros.
    * El nombre de los campos debe aparecer en la primera fila del fichero para poder
    categorizar los distintos campos.
    * Por temas de confidencialidad los ficheros validados se eliminarán de nuestro servidor al cabo de 30 días, dejando solo un resumen de la verificación. Debes guardar los datos verificados en tu entorno.

    En la imagen inferior dispones de un ejemplo de cómo debería ser el fichero a validar::

    ![File Upload 4](static/images/file-upload4-tel.png)
    
    Si no estás seguro de que tus datos están bien formateados, sube solo una parte de tus contactos y realiza una prueba con unos 5 mails. Los créditos que consumas en verificaciones con registros inválidos no pueden ser reembolsados.
    
    Si tu fichero no está bien formateado, copia la columna de los teléfonos en un bloc de notas o en una nueva hoja Excel y valida solo los emails.
    Una vez verificados, dispondrás de 2 columnas, una que contiene el teléfono y el resultado de la verificación. Estos valores los puedes volver a copiar en tu fichero Excel original.
    
    
    

    Una vez el fichero ha sido procesado por *Verificaremails ®*, aparece la columna **_Staus_**
    para categorizar el estado de los emails. Los únicos teléfonos 100% seguros son las "connected". En la columna "Result" podrás ver los detalles de la verificación. Puedes leer más sobre este tema en
    la sección [**Guia de Resultados**](#section/Guia-Resultados).

    Las listas procesadas tienen el siguiente aspecto:

    ![File Upload 5](static/images/file-upload5-tel.png)

    # Descargar y Exportar Resultados
    Una vez tu lista ha sido verificada, recibirás un correo. El formato del fichero será el mismo que has subido, pero con 2 columnas adicionales ("status" y "result").


    # Guía Resultados
    *Verificaremails ®* la respuesta de las llamadas, veien en formato JSON para poder explotar los datos de 
    forma cómoda (Excel permite convertir el formato JSON en columnas para facilitar la explotación de los 
    datos).
      
    | id                                | Tipo        |Valor Nulo          | Description                                                                            |
    |-----------------------------------|-------------|--------------------|----------------------------------------------------------------------------------------|
    | id                                | string      |                    | ID único de la petición.                                                               |
    | cost                              | float       |                    | Número de tokens utilizados en la verificación.                                        |
    | phone_number                      | string      |                    | Número de teléfono en formato E.164 format.                                            |
    | number_type                       | string      |                    | Tipo de número de teléfono (fijo o móvil) Number types                                 |
    | timezone                          | string      |                    | Zona horaria donde originalmente el número fue asignado. En ningún caso traza la zona horaria donde se encuentra el usuario en el momento de la verificación.                                        |
    | is_ported                         | bool        | ✓                  | Indica si el número ha sido portado. Se muestra null en caso de que no se disponga de esta información.                     |
    | reachable                         | string      |                    | Se indica la accesibilidad en el preciso momento de la verificación. Para más información ver Reachability State.                                       |
    | imsi                              | string                                        | ✓       | International Mobile Subscriber Identity (IMSI). Identificador único asociado a la tarjeta SIM. La disponibilidad del IMSI depende del operador móvil de la tarjeta.                                        |
    | format.e164                       | string                                        |        | El número en formato E.164 format.                                       |
    | format.international              | string                                        |        | El número en formato internacional.                                       |
    | format.national                   | string                                        |        | El número en formato nacional.                                      |
    | format.rfc3966                    | string                                        |        | El número formateado en RFC3966 format.                                       |
    | original_network.country_iso2     | string                                        |        | El Código de país (ISO2) donde originalmente el número fue asignado.                                       |
    | original_network.country_prefix   | string                                        |        | El prefijo internacional de llamada donde el número fue originalmente asignado.                                       |       
    | original_network.area             | string                                        | ✓       | El nombre del área donde el número fue asignado.                                       |
    | original_network.mccmnc           | string                                        | ✓       | Cinco o seis caracteres MCCMNC (mobile country code + mobile network code tuple) identificando la red original que emitió el número.                                       |
    | original_network.mcc              | string                                        | ✓       | Tres caracteres MCC (mobile country code) identificando donde la red donde fue emitido el número.                                      |
    | original_network.mnc              | string                                        | ✓       | Dos o tres caracteres MNC (mobile network code) identificando la red donde fue emitido el número.                                       |
    | original_network.network_name     | string                                        | ✓       | Nombre del operador que emitió el número, si se dispone de esta información.                                       |
    | current_network.country_iso2      | string                                        | ✓       | Código del país (ISO2) donde el numero actualmente este asignado.                                        |
    | current_network.country_prefix    | string                                        |        | El prefijo internacional donde actualmente el número este asignado.                                       |       
    | current_network.area              | string                                        | ✓       | Nombre del área donde actualmente el numero este asignado, si se dispone de esta información.                                       |
    | current_network.mccmnc            | string                                        |✓       | Cinco o seis caracteres MCCMNC (mobile country code + mobile network code tuple) identificando la red donde actualmente pertenece el número.                                        |
    | current_network.mcc               | string                                        | ✓       | Tres caracteres MCC (mobile country code) identificando el país donde actualmente pertenece el número.                                       |
    | current_network.mnc               | string                                        | ✓       | Dos o tres caractres MNC (mobile network code) identificando la red donde actualmente el número pertenece.                                       |
    | current_network.network_name      | string                                        |    ✓       | El nombre del operador donde actualmente el número este asignado, si se dispone de esta información.                                       |
            
    Si el número que tratamos de verificar es una línea fija, la respuesta que obtenemos es:
        
    | id              | Tipo           |Valor Nulo          | Description                                                                            |
    |-----------------|----------------|--------------------|----------------------------------------------------------------------------------------|
    | id                                | string                                        |        | ID único de la petición.                          |
    | cost                              | float                                         |        | Número de tokens utilizados en la verificación.  |
    | phone_number                      | string                                        |        | Número de teléfono en formato E.164 format.                                      |
    | number_type                       | string                                        |        | Tipo de número de teléfono (fijo o móvil) Number types                           |
    | timezone                          | string                                        |        | Zona horaria donde originalmente el número fue asignado. En ningún caso traza la zona horaria donde se encuentra el usuario en el momento de la verificación.                                        |
    | format.e164                       | string                                        |        | El número en formato E.164 format.                                       |
    | format.international              | string                                        |        | El número en formato internacional.                                       |
    | format.national                   | string                                        |        | El número en formato nacional.                                      |
    | format.rfc3966                    | string                                        |        | El número formateado en RFC3966 format.                                       |
    | original_network.country_iso2     | string                                        |        | El Código de país (ISO2) donde originalmente el número fue asignado.               
    | original_network.country_prefix   | string                                        |        | El prefijo internacional de llamada donde el número fue originalmente asignado. |  
    | original_network.area             | string                                        |✓       | El nombre del área donde el número fue asignado.                                 |
    | original_network.network_name     | string                                        |✓       | El operador original que asigno el número.                                       |
         
    Por cada número válido procesado a través de la API de verificación de números, devolveremos información sobre el estado de accesibilidad actual del número. Con esta información, puede determinar si el número está actualmente activo y localizable.
        
    | Estado                     | Description                                                                            |
    |----------------------------|----------------------------------------------------------------------------------------|
    | connected                  | Número móvil activo.                                       |
    | absent                     | El número no esta accesible en este momento. Para más detalles revisar la table Suscritores Ausentes                                               |
    | no-teleservice-provisioned | El número no puede recibir llamadas ni mensajes SMS. Suelen ser números asociados a una tarjeta SIM de datos. |
    | inconclusive               | No podemos obtener una respuesta de la red para este número. La red no proporciona esta información.                           |
    | missing parameters         | There are no validations remaining to complete this attempt.                           |
    | no-coverage failed          | There are no validations remaining to complete this attempt.                           | 
        
        
      ## Suscriptor Ausente
         
      Si su propiedad de accesibilidad devuelve que el número es “suscriptor ausente” (absent), entonces hay varias razones posibles para esto.
         <br><br>
         * El teléfono está apagado y se realizó una llamada al número durante este período. Cuando un intento de conectarse a un número falla porque está apagado, no tiene señal o está en modo avión, entonces la llamada al API se actualizará a un estado de Suscriptor ausente para reflejar que las llamadas no pueden conectarse actualmente o los SMS no pueden enviarse a ese número. Cuando el teléfono se vuelva a encender, se conectará a una torre celular y el API se actualizará y marcará que el número es accesible.
         <br><br>
         * Un largo período de inactividad en el número. Cada operador de red tiene diferentes umbrales al actualizar la base de datos del API para mostrar un número de móvil como “ausente”. Por lo general, si un número no se ha activado en un teléfono durante más de 4 días, se considerará como Ausente y una búsqueda lo reflejará.
         <br><br>
         * El número se ha asignado a una tarjeta SIM pero aún no se ha conectado (por ejemplo, un número de teléfono que todavía está en una tienda a la espera de ser vendido).

    ## Tipos de Números
        
    Por cada número válido procesado a través de la API de verificación de números, devolveremos información sobre el 
      estado de accesibilidad actual del número. Con esta información, puede determinar si el número está actualmente 
      activo y localizable.
        
      | Tipo                       | Description                                                                             |
      |-----------------------------|----------------------------------------------------------------------------------------|
      | landline                    | Número de teléfono fijo.                                                               |
      | mobile                      | Número de teléfono móvil.                                                              |
      | mobile_or_landline          | Número fijo o móvil.                                                                   |
      | toll_free                   | Número de teléfono gratuito.                                                           |
      | premium_rate                | Número de teléfono Premium con cargos extra                                            |
      | shared_cost                 | Número de teléfono de costo compartido. Por lo general, menos costoso que los números de teléfono de tarifa premium.  |     
      | personal_number             | Un número personal está asociado con una persona en particular y puede enrutarse a un número de teléfono fijo o móvil. Se puede encontrar más información aquí.here                                                                                                           |
      | voip                        | Número de teléfono de voz sobre IP. Incluye números de teléfono TSoIP (Servicio de Telefonía sobre IP).               |
      | pager                       | Número de teléfono del buscapersonas. Por lo general, no hay funcionalidad de voz.                                    |
      | uan                         | Número de Acceso Universal (Número de Empresa). Puede enrutarse a oficinas específicas, pero permite que se use un número para la empresa.                                                                                                                                    |
      | voicemail                   | Número de teléfono del correo de voz (voicemail)                                                                      |
      | unknown                     | El número no ha podido ser identificado.                                                                              |
