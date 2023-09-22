---
title: Guia Rápida
icon: fas fa-stream
order: 1
tags: quickstart
---
## Registrar un nuevo dispositivo

Haz clic en el botón de agregar (el ícono de suma) en la barra de herramientas de dispositivos para registrar un nuevo dispositivo.

Debes completar los campos de nombre e identificador. El nombre puede ser cualquier cosa. El identificador debe coincidir con el ID único que tu dispositivo está informando al servidor. Para la mayoría de los dispositivos, debes utilizar el IMEI o el número de serie como identificador único.

Si no conoces el identificador de tu dispositivo, puedes configurar el dispositivo para que primero informe los datos y luego buscar el ID en el registro. Consulta la guía de solución de problemas para obtener más detalles.

___

## Configurar un dispositivo

Configura tu dispositivo para que comience a enviar los datos de ubicación a tu servidor. Para obtener más detalles sobre cómo configurar tu modelo específico, consulta el manual de tu dispositivo o comunícate con el soporte de tu proveedor de dispositivos.

Si alojas tu propio servidor, tu sistema debe tener una dirección IP pública. No todos los proveedores de internet asignan direcciones IP públicas. Tu dirección actual parece ser 2800:484:ea7f:c310:e8dd:ec16:a0c8:301e, pero podría no ser tu dirección dedicada si estás detrás de un NAT. Si no tienes una IP pública, puedes utilizar un servidor VPS o una de nuestras suscripciones en lugar de alojarlo localmente.

Para seleccionar el número de puerto correcto, busca tu dispositivo en la lista de dispositivos admitidos. La columna de puerto indica el número de puerto predeterminado en Traccar para tu dispositivo.

___

## Identificación del protocolo

Como primer paso, intenta encontrar tu dispositivo en la lista de dispositivos admitidos. La última columna contiene el número de puerto predeterminado para el dispositivo. Si tienes un dispositivo fabricado en China, asegúrate de verificar también la información sobre clones.

Si un puerto determinado no funciona para tu dispositivo o no puedes encontrar tu dispositivo en la lista de dispositivos admitidos, intenta recopilar algunas muestras siguiendo los siguientes pasos:

1. Configura tu dispositivo para enviar datos al puerto __5001__.
2. Espera a que el dispositivo envíe algunos mensajes al servidor.
3. Encuentra el mensaje en formato HEX del dispositivo en el archivo de registro.

Una vez que tengas algunas muestras y estés seguro de que son de tu dispositivo, puedes intentar compararlas con los patrones comunes a continuación o compararlas con casos de prueba que tenemos para varios protocolos:

Casos de prueba para protocolos.

Si el protocolo está basado en texto, primero debes convertir el formato HEX a texto.
