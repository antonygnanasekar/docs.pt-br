---
title: Requisitos do sistema do .NET Framework
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology:
- dotnet-clr
ms.tgt_pltfrm: 
ms.topic: article
helpviewer_keywords:
- software requirements
- .NET Framework, system requirements
- system requirements
- operating systems supported
- hardware requirements
ms.assetid: 298275e2-da1d-4618-9f74-6a3567832350
caps.latest.revision: 95
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.translationtype: HT
ms.sourcegitcommit: 21c6a1485f3d0c38bde065d6ecc7b07d5e424c1d
ms.openlocfilehash: 18875105836ee4be0a3d3fb61a83ef6cd29b8c58
ms.contentlocale: pt-br
ms.lasthandoff: 08/05/2017

---

# <a name="net-framework-system-requirements"></a>Requisitos do sistema do .NET Framework

As tabelas nesse tópico fornecem o hardware, o sistema operacional e os requisitos de software para o .NET Framework 4.5 e lançamentos pontuais (4.5.1 e 4.5.2), e o [!INCLUDE[net_v46](../../../includes/net-v46-md.md)] e seus lançamentos pontuais (4.6.1 e 4.6.2) e o .NET Framework 4.7. Os ambientes de desenvolvimento que permitem desenvolver aplicativos para o .NET Framework têm um conjunto de requisitos separado.

Para obter informações sobre download e links, consulte [Instalar o .NET Framework para desenvolvedores](../../../docs/framework/install/guide-for-developers.md).

Para saber mais sobre o ciclo de vida de suporte de versões do .NET Framework, veja [Ciclo de vida do Suporte da Microsoft](https://support.microsoft.com/en-us/lifecycle/search?sort=PN&alpha=Microsoft%20.NET%20Framework&Filter=FilterNO).

## <a name="hardware-requirements"></a>Requisitos de hardware

|                          |        |
| ------------------------ | ------ |
| **Processador**            | 1 GHz  |
| **RAM**                  | 512 MB |
| **Espaço em disco (mínimo)** |        |
| 32 bits                   | 4,5 GB |
| 64 bits                   | 4,5 GB |

## <a name="installation-requirements"></a>Requisitos de instalação

A instalação do .NET Framework exige privilégios de administrador. Se você não tiver direitos de administrador no computador no qual deseja instalar o .NET Framework, entre em contato com o administrador da rede.

## <a name="supported-client-operating-systems"></a>Sistemas operacionais cliente compatíveis

| Sistema operacional | Edições com suporte | Pré-instalado com o sistema operacional | Instalado separadamente |
| ---------------- | ------------------ | ------------------------ | ---------------------- |
| Atualização do Windows 10 para Criadores | 32 bits e 64 bits | .NET Framework 4.7 | | 
| Atualização de Aniversário do Windows 10 | 32 bits e 64 bits | [!INCLUDE[net_v462](../../../includes/net-v462-md.md)]|.NET Framework 4.7 |
| Atualização de novembro do Windows 10 | 32 bits e 64 bits | [!INCLUDE[net_v461](../../../includes/net-v461-md.md)] | |
| Windows 10 | 32 bits e 64 bits | [!INCLUDE[net_v46](../../../includes/net-v46-md.md)] | [!INCLUDE[net_v461](../../../includes/net-v461-md.md)] |
| [!INCLUDE[win81](../../../includes/win81-md.md)] | 32 bits, 64 bits e ARM | [!INCLUDE[net_v451](../../../includes/net-v451-md.md)] | [!INCLUDE[net_v452](../../../includes/net-v452-md.md)]<br /><br /> [!INCLUDE[net_v46](../../../includes/net-v46-md.md)]<br /><br /> [!INCLUDE[net_v461](../../../includes/net-v461-md.md)]<br /><br /> [!INCLUDE[net_v462](../../../includes/net-v462-md.md)]<br /><br />.NET Framework 4.7 |
| [!INCLUDE[win8](../../../includes/win8-md.md)] | 32 bits, 64 bits e ARM | [!INCLUDE[net_v45](../../../includes/net-v45-md.md)] | [!INCLUDE[net_v451](../../../includes/net-v451-md.md)]<br /><br /> [!INCLUDE[net_v452](../../../includes/net-v452-md.md)]<br /><br /> [!INCLUDE[net_v46](../../../includes/net-v46-md.md)]<br /><br /> [!INCLUDE[net_v461](../../../includes/net-v461-md.md)] |
| Windows 7 SP1|32 bits e 64 bits | -- | .NET Framework 4<br /><br /> [!INCLUDE[net_v45](../../../includes/net-v45-md.md)]<br /><br /> [!INCLUDE[net_v451](../../../includes/net-v451-md.md)]<br /><br /> [!INCLUDE[net_v452](../../../includes/net-v452-md.md)]<br /><br /> [!INCLUDE[net_v46](../../../includes/net-v46-md.md)]<br /><br /> [!INCLUDE[net_v461](../../../includes/net-v461-md.md)]<br /><br /> [!INCLUDE[net_v462](../../../includes/net-v462-md.md)]<br /><br />.NET Framework 4.7 |
| Windows Vista SP2|32 bits e 64 bits | -- | .NET Framework 4<br /><br /> [!INCLUDE[net_v45](../../../includes/net-v45-md.md)]<br /><br /> [!INCLUDE[net_v451](../../../includes/net-v451-md.md)]<br /><br /> [!INCLUDE[net_v452](../../../includes/net-v452-md.md)]<br /><br /> [!INCLUDE[net_v46](../../../includes/net-v46-md.md)] |
| Windows XP |32 bits e 64 bits | -- | .NET Framework 4 |

 **Observações:**

- Em sistemas com Windows 7, o .NET Framework exige o Windows 7 SP1. Se você estiver no Windows 7 e ainda não tiver instalado o Service Pack 1, precisará fazer isso antes de instalar o .NET Framework.

- O [!INCLUDE[net_v45](../../../includes/net-v45-md.md)] é compatível no Windows PE (Ambiente de Pré-Instalação do Windows). Nem todos os recursos são compatíveis com o Windows PE.

- O .NET Framework 4 também oferece suporte à plataforma IA64.

- Para todas as plataformas, recomendamos que você atualize para o Service Pack mais recente do Windows e instale as atualizações críticas disponíveis no [site Windows Update](http://go.microsoft.com/fwlink/?LinkId=168461) para garantir a melhor compatibilidade e segurança.

- Em sistemas operacionais 64 bits, o .NET Framework dá suporte ao WOW64 (processamento de 32 bits em um computador de 64 bits) e ao processamento de 64 bits nativo.

## <a name="supported-server-operating-systems"></a>Sistemas operacionais de servidor compatíveis

| Sistema operacional | Edições com suporte | Pré-instalado com o sistema operacional | Instalado separadamente |
| ---------------- | ------------------ | ------------------------ | ---------------------- |
| Windows Server 2016 | 64 bits | [!INCLUDE[net_v462](../../../includes/net-v462-md.md)] | .NET Framework 4.7 |
| [!INCLUDE[winblue_server_2](../../../includes/winblue-server-2-md.md)] | 64 bits | [!INCLUDE[net_v451](../../../includes/net-v451-md.md)] | [!INCLUDE[net_v452](../../../includes/net-v452-md.md)]<br /><br /> [!INCLUDE[net_v46](../../../includes/net-v46-md.md)]<br /><br /> [!INCLUDE[net_v461](../../../includes/net-v461-md.md)]<br /><br /> [!INCLUDE[net_v462](../../../includes/net-v462-md.md)]<br /><br />.NET Framework 4.7 |
| [!INCLUDE[winserver8](../../../includes/winserver8-md.md)] (edição de 64 bits) | 64 bits| [!INCLUDE[net_v45](../../../includes/net-v45-md.md)] | [!INCLUDE[net_v451](../../../includes/net-v451-md.md)]<br /><br /> [!INCLUDE[net_v452](../../../includes/net-v452-md.md)]<br /><br /> [!INCLUDE[net_v46](../../../includes/net-v46-md.md)]<br /><br /> [!INCLUDE[net_v461](../../../includes/net-v461-md.md)]<br /><br /> [!INCLUDE[net_v462](../../../includes/net-v462-md.md)]<br /><br />.NET Framework 4.7 |
| Windows Server 2008 R2 SP1|64 bits | -- | .NET Framework 4<br /><br /> [!INCLUDE[net_v45](../../../includes/net-v45-md.md)]<br /><br /> [!INCLUDE[net_v451](../../../includes/net-v451-md.md)]<br /><br /> [!INCLUDE[net_v452](../../../includes/net-v452-md.md)]<br /><br /> [!INCLUDE[net_v46](../../../includes/net-v46-md.md)]<br /><br /> [!INCLUDE[net_v461](../../../includes/net-v461-md.md)]<br /><br /> [!INCLUDE[net_v462](../../../includes/net-v462-md.md)]<br /><br />.NET Framework 4.7 |
| Windows Server 2008 SP2|32 bits e 64 bits | -- | .NET Framework 4<br /><br /> [!INCLUDE[net_v45](../../../includes/net-v45-md.md)]<br /><br /> [!INCLUDE[net_v451](../../../includes/net-v451-md.md)]<br /><br /> [!INCLUDE[net_v452](../../../includes/net-v452-md.md)]<br /><br /> [!INCLUDE[net_v46](../../../includes/net-v46-md.md)] |

 **Observações:**

- [!INCLUDE[winserver8](../../../includes/winserver8-md.md)] inclui o [!INCLUDE[net_v45](../../../includes/net-v45-md.md)], para que você não precise instalá-lo separadamente. Da mesma forma, [!INCLUDE[winblue_server_2](../../../includes/winblue-server-2-md.md)] inclui o [!INCLUDE[net_v451](../../../includes/net-v451-md.md)].

- O .NET Framework tem suporte na Função Núcleo do Servidor com Windows Server 2008 R2 SP1 ou posterior, mas não tem suporte no Windows Server 2008 R2 for Itanium-Based Systems.

- Windows Server 2008 SP2, o .NET Framework não tem suporte na Função Server Core.

- Para todas as plataformas, recomendamos que você atualize para o Service Pack e as atualizações críticas disponíveis mais recentes do Windows no [site Windows Update](http://go.microsoft.com/fwlink/?LinkId=168461) para garantir a melhor compatibilidade e segurança. A instalação do Windows Service Pack mais recente pode ser necessária em alguns sistemas operacionais.

- Em sistemas operacionais 64 bits, o .NET Framework dá suporte ao WOW64 (processamento de 32 bits em um computador de 64 bits) e ao processamento de 64 bits nativo.

## <a name="see-also"></a>Consulte também

[Guia de instalação](../../../docs/framework/install/index.md)   
[Introdução](../../../docs/framework/get-started/index.md)   
[Solução de problemas de instalações e desinstalações bloqueadas do .NET Framework](../../../docs/framework/install/troubleshoot-blocked-installations-and-uninstallations.md)

