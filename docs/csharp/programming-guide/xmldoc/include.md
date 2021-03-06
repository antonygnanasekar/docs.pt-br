---
title: "&lt;include&gt; (Guia de Programação em C#)"
ms.date: 2015-07-20
ms.prod: .net
ms.technology:
- devlang-csharp
ms.topic: article
f1_keywords:
- include
- <include>
dev_langs:
- CSharp
helpviewer_keywords:
- <include> C# XML tag
- include C# XML tag
ms.assetid: a8a70302-6196-4643-bd09-ef33f411f18f
caps.latest.revision: 19
author: BillWagner
ms.author: wiwagn
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
ms.sourcegitcommit: df0438dd742db802bb0f935d840006236d5d9bf9
ms.openlocfilehash: 0cabcc25c4e35027c600e4af2bccfad7f9db1514
ms.contentlocale: pt-br
ms.lasthandoff: 08/29/2017

---
# <a name="ltincludegt-c-programming-guide"></a>&lt;include&gt; (Guia de Programação em C#)
## <a name="syntax"></a>Sintaxe  
  
```xml  
<include file='filename' path='tagpath[@name="id"]' />  
```  
  
#### <a name="parameters"></a>Parâmetros  
 `filename`  
 O nome do arquivo XML que contém a documentação. O nome do arquivo pode ser qualificado com um caminho. Coloque `filename` entre aspas simples (' ').  
  
 `tagpath`  
 O caminho das marcas em `filename` que leva à marca `name`. Coloque o caminho entre aspas simples (' ').  
  
 `name`  
 O especificador de nome na marca que precede os comentários; `name` terá um `id`.  
  
 `id`  
 A ID da marca que precede os comentários. Coloque a ID entre aspas duplas (" ").  
  
## <a name="remarks"></a>Comentários  
 A marca \<include> permite consultar comentários em outro arquivo que descrevem os tipos e membros em seu código-fonte. Essa é uma alternativa para inserir comentários de documentação diretamente em seu arquivo de código-fonte. Colocando a documentação em um arquivo separado, é possível aplicar o controle do código-fonte à documentação separadamente do código-fonte. Uma pessoa pode fazer o check-out do arquivo de código-fonte e outra pessoa pode fazer o check-out do arquivo de documentação.  
  
 A marca \<include> usa a sintaxe XML XPath. Consulte a documentação do XPath para obter maneiras de personalizar o uso de \<include>.  
  
## <a name="example"></a>Exemplo  
 Este é um exemplo de vários arquivos. O primeiro arquivo, que usa \<include>, é listado abaixo:  
  
 [!code-cs[csProgGuideDocComments#5](../../../csharp/programming-guide/xmldoc/codesnippet/CSharp/include_1.cs)]  
  
 O segundo arquivo, xml_include_tag.doc, contém os comentários de documentação a seguir:  
  
```xml  
<MyDocs>  
  
<MyMembers name="test">  
<summary>  
The summary for this type.  
</summary>  
</MyMembers>  
  
<MyMembers name="test2">  
<summary>  
The summary for this other type.  
</summary>  
</MyMembers>  
  
</MyDocs>  
```  
  
## <a name="program-output"></a>Saída do Programa  
 A seguinte saída é gerada quando você compila as classes Test e Test2 com a seguinte linha de comando: `/doc:DocFileName.xml.` No Visual Studio, especifique a opção de comentários de documentos XML no painel Compilar do Designer de Projeto. Quando o compilador C# encontrar a marca \<include>, ele pesquisará os comentários da documentação em xml_include_tag.doc, em vez de no arquivo de origem atual. O compilador, então, gera DocFileName.xml e esse é o arquivo consumido pelas ferramentas de documentação como [Sandcastle](https://github.com/EWSoftware/SHFB) para gerar a documentação final.  
  
```xml  
<?xml version="1.0"?>   
<doc>   
    <assembly>   
        <name>xml_include_tag</name>   
    </assembly>   
    <members>   
        <member name="T:Test">   
            <summary>   
The summary for this type.   
</summary>   
        </member>   
        <member name="T:Test2">   
            <summary>   
The summary for this other type.   
</summary>   
        </member>   
    </members>   
</doc>   
```  
  
## <a name="see-also"></a>Consulte também  
 [Guia de Programação em C#](../../../csharp/programming-guide/index.md)   
 [Marcas recomendadas para comentários de documentação](../../../csharp/programming-guide/xmldoc/recommended-tags-for-documentation-comments.md)

