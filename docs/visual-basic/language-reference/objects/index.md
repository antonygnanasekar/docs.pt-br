---
title: Objetos (Visual Basic)
ms.date: 2015-07-20
ms.prod: .net
ms.suite: 
ms.technology:
- devlang-visual-basic
ms.topic: article
dev_langs:
- VB
helpviewer_keywords:
- objects [Visual Basic]
ms.assetid: 651c73e4-dca8-402b-9c6b-e3902b3a3f4b
caps.latest.revision: 22
author: dotnet-bot
ms.author: dotnetcontent
translation.priority.ht:
- cs-cz
- de-de
- es-es
- fr-fr
- it-it
- ja-jp
- ko-kr
- pl-pl
- pt-br
- ru-ru
- tr-tr
- zh-cn
- zh-tw
ms.translationtype: HT
ms.sourcegitcommit: 306c608dc7f97594ef6f72ae0f5aaba596c936e1
ms.openlocfilehash: 98503c5764690d6dea90bf46a229e9ee2fd81df7
ms.contentlocale: pt-br
ms.lasthandoff: 07/28/2017

---
# <a name="objects-visual-basic"></a>Objetos (Visual Basic)
Este tópico fornece links para outros tópicos que documentam os objetos de tempo de execução do Visual Basic e que contêm tabelas dos procedimentos, das propriedades e dos eventos dos seus membros.  
  
## <a name="visual-basic-run-time-objects"></a>Objetos em tempo de execução do Visual Basic  
  
|||  
|---|---|  
|<xref:Microsoft.VisualBasic.Collection>|Fornece uma maneira conveniente para ver um grupo relacionado de itens como um único objeto.|  
|<xref:Microsoft.VisualBasic.Information.Err%2A>|Contém informações sobre erros de tempo de execução.|  
|O objeto `My.Application` consiste nas seguintes classes:<br /><br /> <xref:Microsoft.VisualBasic.ApplicationServices.ApplicationBase> fornece membros disponíveis em todos os projetos.<br /><br /> <xref:Microsoft.VisualBasic.ApplicationServices.WindowsFormsApplicationBase> fornece membros disponíveis nos aplicativos do Windows Forms.<br /><br /> <xref:Microsoft.VisualBasic.ApplicationServices.ConsoleApplicationBase> fornece membros disponíveis nos aplicativos de console.|Fornece dados associados apenas ao aplicativo ou à DLL atual. Nenhuma informação em nível de sistema pode ser alterada com `My.Application`.<br /><br /> Alguns membros estão disponíveis apenas para aplicativos do Windows Forms ou de console.|  
|`My.Application.Info` (<xref:Microsoft.VisualBasic.ApplicationServices.ApplicationBase.Info%2A>)|Fornece propriedades para obter informações sobre o aplicativo, como o número de versão, a descrição, os assemblies carregados e assim por diante.|  
|`My.Application.Log` (<xref:Microsoft.VisualBasic.ApplicationServices.ApplicationBase.Log%2A>)|Fornece uma propriedade e métodos para gravar informações de evento e de exceção para os ouvintes de log do aplicativo.|  
|`My.Computer` (<xref:Microsoft.VisualBasic.Devices.Computer>)|Fornece propriedades para manipular componentes do computador, como o áudio, o relógio, o teclado, o sistema de arquivos e assim por diante.|  
|`My.Computer.Audio` (<xref:Microsoft.VisualBasic.Devices.Audio>)|Fornece métodos para reproduzir sons.|  
|`My.Computer.Clipboard` (<xref:Microsoft.VisualBasic.Devices.Computer.Clipboard%2A>)|Fornece métodos para manipular a Área de Transferência.|  
|`My.Computer.Clock` (<xref:Microsoft.VisualBasic.Devices.Clock>)|Fornece propriedades para acessar a hora local atual e o Tempo Universal Coordenado (equivalente ao Horário do Meridiano de Greenwich) no relógio do sistema.|  
|`My.Computer.FileSystem` (<xref:Microsoft.VisualBasic.FileIO.FileSystem>)|Fornece propriedades e métodos para trabalhar com unidades, arquivos e diretórios.|  
|`My.Computer.FileSystem.SpecialDirectories` (<xref:Microsoft.VisualBasic.FileIO.SpecialDirectories>)|Fornece propriedades para acessar diretórios comumente referenciados.|  
|`My.Computer.Info` (<xref:Microsoft.VisualBasic.Devices.ComputerInfo>)|Fornece propriedades para obter informações sobre memória, assemblies carregados, nome e sistema operacional do computador.|  
|`My.Computer.Keyboard` (<xref:Microsoft.VisualBasic.Devices.Keyboard>)|Fornece propriedades para acessar o estado atual do teclado, como quais teclas estão pressionadas no momento e fornece um método para enviar pressionamentos de teclas para a janela ativa.|  
|`My.Computer.Mouse` (<xref:Microsoft.VisualBasic.Devices.Mouse>)|Fornece propriedades para obter informações sobre o formato e a configuração do mouse instalado no computador local.|  
|`My.Computer.Network` (<xref:Microsoft.VisualBasic.Devices.Network>)|Fornece uma propriedade, um evento e métodos para interagir com a rede à qual o computador está conectado.|  
|`My.Computer.Ports` (<xref:Microsoft.VisualBasic.Devices.Ports>)|Fornece uma propriedade e um método para acessar portas seriais do computador.|  
|`My.Computer.Registry` (<xref:Microsoft.VisualBasic.MyServices.RegistryProxy>)|Fornece propriedades e métodos para manipular o Registro.|  
|[Objeto My.Forms](../../../visual-basic/language-reference/objects/my-forms-object.md)|Fornece propriedades para acessar uma instância de cada Formulário do Windows declarado no projeto atual.|  
|`My.Log` (<xref:Microsoft.VisualBasic.Logging.AspLog>)|Fornece uma propriedade e métodos para gravar informações de evento e de exceção para os ouvintes de log dos aplicativos Web.|  
|[Objeto My.Request](../../../visual-basic/language-reference/objects/my-request-object.md)|Obtém o objeto <xref:System.Web.HttpRequest> para a página solicitada. O objeto `My.Request` contém informações sobre a solicitação HTTP atual.<br /><br /> O objeto `My.Request` está disponível apenas para aplicativos do [!INCLUDE[vstecasp](~/includes/vstecasp-md.md)].|  
|[Objeto My.Resources](../../../visual-basic/language-reference/objects/my-resources-object.md)|Fornece propriedades e classes para acessar recursos de um aplicativo.|  
|[Objeto My.Response](../../../visual-basic/language-reference/objects/my-response-object.md)|Obtém o objeto <xref:System.Web.HttpResponse> associado à <xref:System.Web.UI.Page>. Esse objeto permite que você envie dados de resposta HTTP para um cliente e contém informações sobre essa resposta.<br /><br /> O objeto `My.Response` está disponível apenas para aplicativos do [!INCLUDE[vstecasp](~/includes/vstecasp-md.md)].|  
|[Objeto My.Settings](../../../visual-basic/language-reference/objects/my-settings-object.md)|Fornece propriedades e métodos para acessar as configurações de um aplicativo.|  
|`My.User` (<xref:Microsoft.VisualBasic.ApplicationServices.User>)|Fornece acesso às informações sobre o usuário atual.|  
|[Objeto My.WebServices](../../../visual-basic/language-reference/objects/my-webservices-object.md)|Fornece propriedades para criar e acessar uma única instância de cada serviço Web referenciado pelo projeto atual.|  
|<xref:Microsoft.VisualBasic.FileIO.TextFieldParser>|Fornece métodos e propriedades para analisar arquivos de texto estruturado.|  
  
## <a name="see-also"></a>Consulte também  
 [Referência da linguagem Visual Basic](../../../visual-basic/language-reference/index.md)   
 [Visual Basic](../../../visual-basic/index.md)

