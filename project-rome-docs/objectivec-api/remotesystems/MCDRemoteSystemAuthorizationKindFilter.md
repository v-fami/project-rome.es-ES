---
title: MCDRemoteSystemAuthorizationKindFilter
description: Una clase utilizada para filtrar según el tipo de autorización de sistemas remotos.
keywords: Microsoft, windows, iOS, iPhone, objectiveC, conectado los dispositivos, proyecto Roma
ms.openlocfilehash: da68c7a0eacd2018332d5e2fe5c8e3c906f473f8
ms.sourcegitcommit: 945a0f4bda02e3b4eb9a665379c2af9bd5285a53
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/18/2019
ms.locfileid: "59801257"
---
# <a name="class-mcdremotesystemauthorizationkindfilter"></a>Clase `MCDRemoteSystemAuthorizationKindFilter` 

```
@interface MCDRemoteSystemAuthorizationKindFilter : NSObject<MCDRemoteSystemFilter>
```  

Una clase utilizada para filtrar según el tipo de autorización de sistemas remotos.

## <a name="properties"></a>Propiedades

### <a name="kind"></a>Tipo
`@property(nonatomic, readonly) MCDRemoteSystemAuthorizationKind kind;`

El tipo de autorización para filtrar.

## <a name="constructors"></a>Constructores

### <a name="filterwithkind"></a>filterWithKind
`+ (nullable instancetype)filterWithKind:(MCDRemoteSystemAuthorizationKind)authorizationKind;`

Una nueva instancia de esta clase MCDRemoteSystemAuthorizationKind a filtrar.

#### <a name="parameters"></a>Parámetros 
* `authorizationKind` 

El tipo de autorización para filtrar.

#### <a name="returns"></a>Devuelve
Devuelve un objeto MCDRemoteSystemAuthorizationKindFilter con el filtro de autorización proporcionado.

### <a name="initwithkind"></a>initWithKind
`- (nullable instancetype)initWithKind:(MCDRemoteSystemAuthorizationKind)authorizationKind;`

Una nueva instancia de esta clase con MCDRemoteSystemAuthorizationKind.

#### <a name="parameters"></a>Parámetros 
* `authorizationKind` 

El tipo de autorización para filtrar.

#### <a name="returns"></a>Devuelve
Devuelve un objeto MCDRemoteSystemAuthorizationKindFilter inicializado con el authorizationKind.