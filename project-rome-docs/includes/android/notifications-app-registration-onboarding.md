---
title: Archivo de inclusión
description: Archivo de inclusión
ms.topic: include
ms.assetid: bbef84bf-a6b7-44be-879d-0fa6065e37b1
ms.localizationpriority: medium
ms.openlocfilehash: 598807ac37079456ac28948a9f5bc419e65095a3
ms.sourcegitcommit: 945a0f4bda02e3b4eb9a665379c2af9bd5285a53
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/18/2019
ms.locfileid: "58907517"
---
### <a name="msa-and-aad-authentication-registration"></a>MSA y registro de la autenticación de AAD

Registro de autenticación de cuenta de Microsoft (MSA) o Azure Active Directory (AAD) es necesario para todas las características del SDK que incluya las notificaciones, excepto para el uso compartido de Nearby API. 

Si aún no tiene una MSA y desea usar uno, registrar en [account.microsoft.com](https://account.microsoft.com/account).

A continuación, si utilizas MSA como la autenticación y el marco de identidad para los usuarios, debe registrar la aplicación con Microsoft, siga las instrucciones de la [Portal de registro de aplicación](https://apps.dev.microsoft.com/) (si no tiene un Microsoft cuenta de desarrollador, debe crear una primera). Debería recibir una cadena de identificador de cliente de la aplicación; Asegúrese de recordar la ubicación o guardar esto. Más adelante se usará durante la incorporación de notificaciones de gráfico. Tenga en cuenta que una aplicación mediante la autenticación de MSA debe estar registrada como una aplicación de SDK de Live, como se muestra a continuación.
![Portal de registro de aplicación](../../notifications/media/msa_app_registration/app_registration_portal.png)

Si está escribiendo una aplicación que usa AAD como cuenta profesional o educativa autenticación y cuentas marco de identidad, debe registrar la aplicación a través de [bibliotecas de autenticación de Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) con el fin de obtener el identificador de cliente, como se muestra a continuación. 
 ![Portal de registro de AAD](../../notifications/media/aad_registration_portal/aad_registration_portal.png) al crear un nuevo registro de aplicación, hay algunos permisos necesarios para poder usar las notificaciones de Graph y otras capacidades de plataforma de dispositivo conectado. Consulte a continuación. 
![AAD Portal: configuración – requiere permisos de registro de](../../notifications/media/aad_registration_portal/aad_registration_portal_permissions.png)
* Agregar inicio de sesión de permiso de usuario que se muestra a continuación.
![Permisos necesarios: perfil de usuario AAD](../../notifications/media/aad_registration_portal/permissions_1_user.png)
* Agregar permisos de servicio de comandos para obtener información de dispositivo, que se muestra a continuación.
![Permisos necesarios: los dispositivos](../../notifications/media/aad_registration_portal/permissions_2_devices.png)
* Agregue el permiso de Graph notificaciones en actividad fuente Service API, se muestra a continuación.
![Permisos necesarios: los dispositivos](../../notifications/media/aad_registration_portal/permissions_3_graph_notifications.png)
* Al final, si está escribiendo aplicaciones multiplataforma incluida una aplicación de UWP que se ejecutan en Windows, asegúrese de agregar permiso de servicio de notificación de Windows, que se muestra a continuación. 
![Permisos necesarios: WNS](../../notifications/media/aad_registration_portal/permissions_4_wns_push.png)
