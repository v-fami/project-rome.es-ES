---
title: MCDConnectedDevicesNotificationRegistrationStatus
description: Valores que se usa para comunicar el estado de registro en la nube.
keywords: Microsoft, windows, iOS, iPhone, objectiveC, conectado los dispositivos, proyecto Roma
ms.openlocfilehash: c7d770c73479afb949a4917b5457b12e23b78698
ms.sourcegitcommit: 945a0f4bda02e3b4eb9a665379c2af9bd5285a53
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/18/2019
ms.locfileid: "59801367"
---
# <a name="class-mcdconnecteddevicesnotificationregistrationstatus"></a>Clase `MCDConnectedDevicesNotificationRegistrationStatus` 

```
typedef NS_ENUM(NSInteger, MCDConnectedDevicesNotificationRegistrationStatus)
```  
Enumeración que indica el estado de la operación de registro.
Los Estados de error indican condiciones transitorias, donde el desarrollador puede querer vuelva a intentar el registro.

## <a name="fields"></a>Campos

| Nombre                              |   Valor     | Descripción |
|:----------------------------------|:------|:-------------------------------|
| MCDConnectedDevicesNotificationRegistrationStatusSuccess | 0 | Operación se completó correctamente.
| MCDConnectedDevicesNotificationRegistrationStatusErrorNoNetwork | 1 | Red no estaba disponible. |
| MCDConnectedDevicesNotificationRegistrationStatusErrorWebFailure | 2 | Error en un servicio web. |
| MCDConnectedDevicesNotificationRegistrationStatusErrorNoTokenRequestSubscriber | 3 | No hay ningún suscriptor de la solicitud de token respondió. |
| MCDConnectedDevicesNotificationRegistrationStatusErrorTokenRequestFailed | 4 | Error en la solicitud de token. |
| MCDConnectedDevicesNotificationRegistrationStatusErrorAccountNotFound | 5 | No se encontró la cuenta para registrar la información de. |
| MCDConnectedDevicesNotificationRegistrationStatusErrorUnknown | 6 | Operación encontró un error desconocido. |