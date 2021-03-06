---
ms.openlocfilehash: 6c87f1a68699de7852af56d7536f08b1a5f9bc14
ms.sourcegitcommit: 945a0f4bda02e3b4eb9a665379c2af9bd5285a53
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/18/2019
ms.locfileid: "58907567"
---
### <a name="register-your-app-in-microsoft-windows-dev-center-for-cross-device-experiences"></a>Registrar la aplicación en Microsoft Windows Dev Center para experiencias multidispositivo
A continuación, deberá registrar la aplicación para la [experiencias multidispositivo característica del panel del desarrollador de Microsoft](https://developer.microsoft.com/dashboard/crossplatform/web). Se trata de un procedimiento diferente desde el registro de aplicación AAD y MSA, que se trata en los pasos anteriores. El objetivo principal de este proceso consiste en asignar las identidades de aplicación específico de plataforma con una identidad de aplicación multiplataforma que es reconocido por la plataforma de dispositivos conectados y, al mismo tiempo, autoriza a Microsoft Graph notificaciones para enviar notificaciones con nativo Servicios de notificación de inserción correspondiente a cada plataforma de sistema operativo. En este caso, habilita las notificaciones de Graph enviar notificaciones a los extremos de la aplicación para UWP de Windows a través de WNS: servicio de notificación de Windows. Ir al panel del centro de desarrollo, vaya a experiencias multidispositivo desde el panel de navegación del lado izquierdo y seleccione Configurar una nueva aplicación entre dispositivos, que se muestra a continuación.
![Panel del centro de desarrollo: experiencias multidispositivo](../../notifications/media/dev_center_portal/dev_center_portal_1_overview.png)

El proceso de incorporación de centro de desarrollo requieren los siguientes pasos:
* Seleccione las plataformas admitidas: seleccione las plataformas donde la aplicación tendrá una presencia y habilitarse para experiencias multidispositivo. En el caso de integración de las notificaciones de gráfico, puede seleccionar desde Windows, Android o iOS. Se muestra como sigue.
![Plataformas compatibles con experiencias multidispositivo:](../../notifications/media/dev_center_portal/dev_center_portal_2_supported_platforms.png)

* Proporcione los identificadores de aplicación: proporcione los identificadores de aplicación para cada uno de la plataforma donde la aplicación tiene una presencia. Se muestra como sigue.
![Experiencias multidispositivo: identificadores de aplicación](../../notifications/media/dev_center_portal/dev_center_portal_3_app_ids.png)
> [!NOTE]
> Puede agregar distintos identificadores (hasta diez) por plataforma, que es en caso de tener varias versiones de la misma aplicación, o incluso diferentes aplicaciones, lo que quiere que sea capaz de recibir las mismas notificaciones enviadas por el servidor de aplicaciones de destino en el mismo usuario. 

* Proporcione o seleccione la aplicación de los identificadores de MSA o AAD registros de aplicaciones. Estos identificadores de cliente correspondientes al registro de aplicación AAD o de MSA se obtuvieron en los pasos de registro de aplicación AAD/MSA anteriores desde arriba. Se muestra como sigue. 
![Experiencias multidispositivo – MSA y registros de aplicaciones AAD](../../notifications/media/dev_center_portal/dev_center_portal_4_msa_aad_connections.png)
* Las notificaciones de Graph y otras capacidades de plataforma de dispositivos conectados aprovecha cada una de las plataformas de notificación nativa en las plataformas principales para enviar notificaciones a la aplicación de extremos de cliente, es decir, WNS (para Windows UWP), GCM (para Android) y Apple Push Notification Service (para iOS ). Proporcione sus credenciales para estas plataformas de notificación habilitar las notificaciones de Graph entregar las notificaciones para el servidor de aplicaciones, al publicar las notificaciones de usuario de destino. Se muestra como sigue. 
![Experiencias multidispositivo: credenciales de inserción](../../notifications/media/dev_center_portal/dev_center_portal_5_push_credentials.png)
> [!NOTE] 
> Para las aplicaciones de UWP de Windows, habilitar la notificación de inserción WNS es un requisito previo para usar notificaciones de Microsoft Graph. Consulte [información general de WNS](https://docs.microsoft.com/en-us/windows/uwp/design/shell/tiles-and-notifications/windows-push-notification-services--wns--overview) para obtener más detalles. Cuando haya completado la incorporación, a continuación, puede proporcionar las credenciales de inserción a través del centro de desarrollo de Windows para la plataforma de dispositivos conectados. 
* El último paso es comprobar el dominio de aplicación entre dispositivos, que actúa como un proceso de comprobación para demostrar que la aplicación tiene que actúa como una identidad de aplicación entre dispositivos de la aplicación que registró la propiedad de este dominio. Se muestra como sigue.  
![Experiencias multidispositivo: comprobación de dominio](../../notifications/media/dev_center_portal/dev_center_portal_6_domain_verification.png) ahora ya está todo preparado con la incorporación. Pase a la sección siguiente. 


