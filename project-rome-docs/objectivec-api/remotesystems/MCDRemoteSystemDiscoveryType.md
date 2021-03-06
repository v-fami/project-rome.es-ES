---
title: MCDRemoteSystemDiscoveryType
description: Contiene valores que describen los sistemas remotos cómo pueden detectarse.
keywords: Microsoft, windows, iOS, iPhone, objectiveC, conectado los dispositivos, proyecto Roma
ms.openlocfilehash: dc94b92311cb666fd2ffd3949b3d4d66a49e6e5b
ms.sourcegitcommit: 945a0f4bda02e3b4eb9a665379c2af9bd5285a53
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/18/2019
ms.locfileid: "59800507"
---
# <a name="enum-mcdremotesystemdiscoverytype"></a>Enum `MCDRemoteSystemDiscoveryType` 

```
typedef NS_ENUM(NSInteger, MCDRemoteSystemDiscoveryType)
```  

Contiene valores que describen los sistemas remotos cómo pueden detectarse. 

## <a name="fields"></a>Campos

| Name                              | Valor | Descripción                    |
|:----------------------------------|:------|:-------------------------------|
| MCDRemoteSystemDiscoveryTypeAny   | 0     | Los sistemas remotos son reconocibles a través de cualquier conexión.  |
| MCDRemoteSystemDiscoveryTypeProximal | 1     | Los sistemas remotos solo son reconocibles a través de una conexión articulaciones próximas, como una variable local
red o la conexión Bluetooth. |
| MCDRemoteSystemDiscoveryTypeCloud | 2     | Los sistemas remotos solo son reconocibles a través de la conexión en la nube. |
| MCDRemoteSystemDiscoveryTypeSpatiallyProximal | 3     | Los sistemas remotos son reconocibles a través de una conexión articulaciones próximas y se esperan que sean
espacialmente cerca del dispositivo de cliente (en el intervalo de Bluetooth, por ejemplo).  |

