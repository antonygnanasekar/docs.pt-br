---
title: "Manipular valores nulos em expressões de consulta"
description: "Como manipular valores nulos em expressões de consulta."
keywords: .NET, .NET Core, C#
author: BillWagner
manager: wpickett
ms.author: wiwagn
ms.date: 12/1/2016
ms.topic: article
ms.prod: .net-core
ms.technology: .net-core-technologies
ms.devlang: dotnet
ms.assetid: ac63ae8b-724d-4251-9334-528f4e884ae7
ms.translationtype: HT
ms.sourcegitcommit: 306c608dc7f97594ef6f72ae0f5aaba596c936e1
ms.openlocfilehash: f4f189504c57c9c01268b10bc96ad3c9af49ddbd
ms.contentlocale: pt-br
ms.lasthandoff: 07/28/2017

---
# <a name="handle-null-values-in-query-expressions"></a>Manipular valores nulos em expressões de consulta

Este exemplo mostra como tratar os possíveis valores nulos em coleções de origem. Uma coleção de objetos, tal como uma <xref:System.Collections.Generic.IEnumerable%601>, pode conter elementos cujo valor é [null](../language-reference/keywords/null.md). Se uma coleção de origem for nula ou contiver um elemento cujo valor for null e sua consulta não lidar com valores null, uma <xref:System.NullReferenceException> será gerada ao executar a consulta.  
  
## <a name="example"></a>Exemplo

 Você pode escrever o código defensivamente para evitar uma exceção de referência nula conforme mostrado no exemplo a seguir:  
  
 [!code-cs[csProgGuideLINQ#82](../../../samples/snippets/csharp/concepts/linq/how-to-handle-null-values-in-query-expressions_1.cs)]  
  
 No exemplo anterior, a cláusula `where` filtra todos os elementos nulos na sequência de categorias. Essa técnica é independente da verificação de nulos na cláusula join. A expressão condicional com null nesse exemplo funciona porque `Products.CategoryID` é do tipo `int?` que é uma abreviação para `Nullable<int>`.  
  
## <a name="example"></a>Exemplo

 Em uma cláusula join, se apenas uma das chaves de comparação for um tipo de valor que permite valor nulo, você pode converter a outra para um tipo que permite valor nulo na expressão de consulta. No exemplo a seguir, suponha que `EmployeeID` é uma coluna que contém os valores do tipo `int?`:  
  
 [!code-cs[csProgGuideLINQ#83](../../../samples/snippets/csharp/concepts/linq/how-to-handle-null-values-in-query-expressions_2.cs)]  
  
## <a name="see-also"></a>Consulte também  
 <xref:System.Nullable%601>   
 [Expressões de consulta LINQ](index.md)   
 [Tipos que permitem valor nulo](../programming-guide/nullable-types/index.md)

