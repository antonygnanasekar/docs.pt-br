---
title: "in (modificador genérico) (Referência de C#)"
ms.date: 2015-07-20
ms.prod: .net
ms.technology:
- devlang-csharp
ms.topic: article
dev_langs:
- CSharp
helpviewer_keywords:
- contravariance, in keyword [C#]
- in keyword [C#]
ms.assetid: 3a778c36-8aed-4ebe-aa8b-39f4057215b1
caps.latest.revision: 17
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
ms.sourcegitcommit: 775e4512a5ff31c7059961f6332c6bdc0dc5247a
ms.openlocfilehash: 663fa75a7e214ed97efb45dda2c9ac298559653d
ms.contentlocale: pt-br
ms.lasthandoff: 08/11/2017

---
# <a name="in-generic-modifier-c-reference"></a>in (modificador genérico) (Referência de C#)
Para parâmetros de tipo genérico, a palavra-chave `in` especifica que o parâmetro de tipo é contravariante. Você pode usar a palavra-chave `in` em delegados e interfaces genéricas.  
  
 A contravariância permite que você use um tipo menos derivado do que aquele especificado pelo parâmetro genérico. Isso permite a conversão implícita de classes que implementam interfaces variantes e a conversão implícita de tipos delegados. A covariância e a contravariância em parâmetros de tipo genérico têm suporte para tipos de referência, mas não para tipos de valor.  
  
 Um tipo pode ser declarado contravariante em uma interface genérica ou delegado se ele for usado apenas como um tipo de argumentos de método e não como um tipo de retorno do método. Os parâmetros `Ref` e `out` não podem ser variantes.  
  
 Uma interface que tem um parâmetro de tipo contravariante permite que os seus métodos aceitem argumentos de tipos menos derivados que aqueles especificados pelo parâmetro de tipo de interface. Por exemplo, como no .NET Framework 4, na interface <xref:System.Collections.Generic.IComparer%601>, o tipo T é contravariante, você poderá atribuir um objeto do tipo `IComparer(Of Person)` a um objeto do tipo `IComparer(Of Employee)`, sem usar qualquer método de conversão especial se o `Employee` herdar o `Person`.  
  
 Um delegado contravariante pode ser atribuído a outro delegado do mesmo tipo, mas com um parâmetro de tipo genérico menos derivado.  
  
 Para obter mais informações, consulte [Covariância e contravariância](../../programming-guide/concepts/covariance-contravariance/index.md).  
  
## <a name="example"></a>Exemplo  
 O exemplo a seguir mostra como declarar, estender e implementar uma interface genérica contravariante. Ele também mostra como você pode usar a conversão implícita para classes que implementam essa interface.  
  
 [!code-cs[csVarianceKeywords#1](../../../csharp/language-reference/keywords/codesnippet/CSharp/in-generic-modifier_1.cs)]  
  
## <a name="example"></a>Exemplo  
 O exemplo a seguir mostra como declarar, instanciar e invocar um delegado genérico contravariante. Ele também mostra como você pode converter implicitamente um tipo delegado.  
  
 [!code-cs[csVarianceKeywords#2](../../../csharp/language-reference/keywords/codesnippet/CSharp/in-generic-modifier_2.cs)]  
  
## <a name="c-language-specification"></a>Especificação da Linguagem C#  
 [!INCLUDE[CSharplangspec](~/includes/csharplangspec-md.md)]  
  
## <a name="see-also"></a>Consulte também  
 [out](../../../csharp/language-reference/keywords/out-generic-modifier.md)   
 [Covariância e contravariância](../../programming-guide/concepts/covariance-contravariance/index.md)   
 [Modificadores](../../../csharp/language-reference/keywords/modifiers.md)

