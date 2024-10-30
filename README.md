# Verificar Teléfonos ®

La <a href="https://www.verificaremails.com/docs/index_telefonos.html">API para Verificar teléfonos</a> permite validar en tiempo real la veracidad de un número de teléfono. 


# Como funciona Verificar Teléfonos ®
Disponemos de 3 mecanismos para verificar los números de teléfono. La verificación más precisa es la Verificación de números HLR, la que proporciona un grado intermedio de precisión es la verificación de números MNP. La verificación más simple es la que solo verifica de forma sintáctica el número de teléfono.
    
Los 3 mecanismos, utilizan los mismos campos, la principal diferencia es en el número de campos devueltos y la precisión de la formación.
    

**Validación HLR:** La más precisa

La verificación HLR (Home Location Register) es nuestra opción más avanzada. Este método:

- Comprueba en tiempo real si un número está activo en la red móvil
- Accede a una base de datos central con información de todos los abonados GSM autorizados
- Proporciona la máxima precisión en la validación de números móviles
- Tiene un costo más elevado debido a su alta fiabilidad

**Verificación MNP:** Equilibrio entre precisión y costo

La búsqueda de portabilidad de números móviles (MNP) ofrece:

- Identificación exacta del proveedor de red actual
- Ayuda en el enrutamiento eficiente de mensajes SMS
- Una solución intermedia entre precisión y costo
- Utilidad como método indirecto de verificación telefónica

**Verificación sintáctica:** Opción económica

Este método básico se centra en:

- Analizar la estructura y formato del número telefónico
- Identificar errores evidentes en la composición del número
- Ofrecer una opción de bajo costo para validación básica
- Proporcionar menos información detallada sobre el número verificado

Cada uno de estos mecanismos utiliza campos similares, pero difieren en la cantidad de información que devuelven y en la precisión de los datos obtenidos. La elección del método dependerá de sus necesidades específicas de validación y presupuesto.


# Guía Resultados
*Verificaremails ®* la respuesta de las llamadas, veien en formato JSON para poder explotar los datos de forma cómoda (Excel permite convertir el formato JSON en columnas para facilitar la explotación de los datos).
      
    | id                                | Tipo        |Valor Nulo          | Description                                                                            |
    |-----------------------------------|-------------|--------------------|----------------------------------------------------------------------------------------|
    | id                                | string      |                    | ID único de la petición.                                                               |
    | cost                              | float       |                    | Número de tokens utilizados en la verificación.                                        |
    | phone_number                      | string      |                    | Número de teléfono en formato E.164 format.                                            |
    | number_type                       | string      |                    | Tipo de número de teléfono (fijo o móvil) Number types                                 |
    | timezone                          | string      |                    | Zona horaria donde originalmente el número fue asignado. En ningún caso traza la zona horaria donde se encuentra el usuario en el momento de la verificación.                                        |
    | is_ported                         | bool        | ✓                  | Indica si el número ha sido portado. Se muestra null en caso de que no se disponga de esta información.                     |
    | reachable                         | string      |                    | Se indica la accesibilidad en el preciso momento de la verificación. Para más información ver Reachability State.                                       |
    | imsi                              | string      | ✓       | International Mobile Subscriber Identity (IMSI). Identificador único asociado a la tarjeta SIM. La disponibilidad del IMSI depende del operador móvil de la tarjeta.                                        |
    | format.e164                       | string      |        | El número en formato E.164 format.                                       |
    | format.international              | string      |        | El número en formato internacional.                                       |
    | format.national                   | string      |        | El número en formato nacional.                                      |
    | format.rfc3966                    | string      |        | El número formateado en RFC3966 format.                                       |
    | original_network.country_iso2     | string      |        | El Código de país (ISO2) donde originalmente el número fue asignado.                                       |
    | original_network.country_prefix   | string      |        | El prefijo internacional de llamada donde el número fue originalmente asignado.                                       |       
    | original_network.area             | string      | ✓       | El nombre del área donde el número fue asignado.                                       |
    | original_network.mccmnc           | string      | ✓       | Cinco o seis caracteres MCCMNC (mobile country code + mobile network code tuple) identificando la red original que emitió el número.                                       |
    | original_network.mcc              | string      | ✓       | Tres caracteres MCC (mobile country code) identificando donde la red donde fue emitido el número.                                      |
    | original_network.mnc              | string      | ✓       | Dos o tres caracteres MNC (mobile network code) identificando la red donde fue emitido el número.                                       |
    | original_network.network_name     | string      | ✓       | Nombre del operador que emitió el número, si se dispone de esta información.                                       |
    | current_network.country_iso2      | string      | ✓       | Código del país (ISO2) donde el numero actualmente este asignado.                                        |
    | current_network.country_prefix    | string      |        | El prefijo internacional donde actualmente el número este asignado.                                       |       
    | current_network.area              | string      | ✓       | Nombre del área donde actualmente el numero este asignado, si se dispone de esta información.                                       |
    | current_network.mccmnc            | string      | ✓       | Cinco o seis caracteres MCCMNC (mobile country code + mobile network code tuple) identificando la red donde actualmente pertenece el número.                                        |
    | current_network.mcc               | string      | ✓       | Tres caracteres MCC (mobile country code) identificando el país donde actualmente pertenece el número.                                       |
    | current_network.mnc               | string      | ✓       | Dos o tres caractres MNC (mobile network code) identificando la red donde actualmente el número pertenece.                                       |
    | current_network.network_name      | string      | ✓       | El nombre del operador donde actualmente el número este asignado, si se dispone de esta información.                                       |
            
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

* Un largo período de inactividad en el número. Cada operador de red tiene diferentes umbrales al actualizar la base de datos del API para mostrar un número de móvil como “ausente”. Por lo general, si un número no se ha activado en un teléfono durante más de 4 días, se considerará como Ausente y una búsqueda lo reflejará.
       
* El número se ha asignado a una tarjeta SIM pero aún no se ha conectado (por ejemplo, un número de teléfono que todavía está en una tienda a la espera de ser vendido).

## Tipos de Números
        
Por cada número válido procesado a través de la API de verificación de números, devolveremos información sobre el estado de accesibilidad actual del número. Con esta información, puede determinar si el número está actualmente activo y localizable.
        
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


Para más información visita la sección Web <a href="https://www.verificaremails.com/validar-numeros-telefono/">servicios de validación de números de teléfono</a> para conocer as caraterísticas del servicio y tener acceso a los créditos de demo.
