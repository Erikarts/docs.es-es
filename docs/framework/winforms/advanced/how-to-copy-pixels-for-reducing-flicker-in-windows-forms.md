---
title: Procedimiento Copiar píxeles para reducir el parpadeo en formularios de Windows
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- bitblt
- graphics [Windows Forms], copying
- flicker [Windows Forms], reducing in Windows Forms
- graphics [Windows Forms], reducing flicker
- pixels [Windows Forms], copying
- flicker
- bit-block transfer
ms.assetid: 33b76910-13a3-4521-be98-5c097341ae3b
ms.openlocfilehash: cdcb64588f91ece02f1e7f446d4020d68262c93d
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/23/2019
ms.locfileid: "54559455"
---
# <a name="how-to-copy-pixels-for-reducing-flicker-in-windows-forms"></a>Procedimiento Copiar píxeles para reducir el parpadeo en formularios de Windows
Al animar un gráfico sencillo, los usuarios a veces pueden encontrarse parpadeos u otros efectos visuales no deseados. Una forma de limitar este problema es usar un proceso "bitblt" en el gráfico. BitBlt es la "bloque de bits transferencia" de los datos de color de un rectángulo de píxeles de origen a un rectángulo de destino de píxeles.  
  
 Con Windows Forms, bitblt se realiza utilizando la <xref:System.Drawing.Graphics.CopyFromScreen%2A> método de la <xref:System.Drawing.Graphics> clase. En los parámetros del método, especifique el origen y destino (como puntos), el objeto graphics que se usa para dibujar la nueva forma y el tamaño del área que se va a copiar.  
  
 En el ejemplo siguiente, se dibuja una forma en el formulario en su <xref:System.Windows.Forms.Control.Paint> controlador de eventos. A continuación, la <xref:System.Drawing.Graphics.CopyFromScreen%2A> método se usa para duplicar la forma.  
  
> [!NOTE]
>  Configuración del formulario <xref:System.Windows.Forms.Control.DoubleBuffered%2A> propiedad `true` hará que el código basado en gráficos en el <xref:System.Windows.Forms.Control.Paint> evento sea de doble búfer. Aunque no tendrá ningún aumento del rendimiento apreciable cuando se usa el código siguiente, es algo a tener en cuenta cuando se trabaja con código más complejo de manipulación de gráficos.  
  
## <a name="example"></a>Ejemplo  
  
```vb  
Private Sub Form1_Paint(ByVal sender As Object, ByVal e As _  
    System.Windows.Forms.PaintEventArgs) Handles MyBase.Paint  
    ' Draw a circle with a bar on top.  
        e.Graphics.FillEllipse(Brushes.DarkBlue, New Rectangle _  
             (10, 10, 60, 60))  
        e.Graphics.FillRectangle(Brushes.Khaki, New Rectangle _  
             (20, 30, 60, 10))  
    ' Copy the graphic to a new location.  
        e.Graphics.CopyFromScreen(New Point(10, 10), New Point _  
             (100, 100), New Size(70, 70))  
End Sub  
```  
  
```csharp  
private void Form1_Paint(System.Object sender,  
    System.Windows.Forms.PaintEventArgs e)  
        {  
        e.Graphics.FillEllipse(Brushes.DarkBlue, new  
            Rectangle(10,10,60,60));  
        e.Graphics.FillRectangle(Brushes.Khaki, new  
            Rectangle(20,30,60,10));  
        e.Graphics.CopyFromScreen(new Point(10, 10), new Point(100, 100),   
            new Size(70, 70));  
}  
```  
  
## <a name="compiling-the-code"></a>Compilar el código  
 El código anterior se ejecuta en el formulario <xref:System.Windows.Forms.Control.Paint> controlador de eventos para que conservar los gráficos cuando se vuelve a dibujar el formulario. Por lo tanto, no llame a métodos relacionados con gráficos el <xref:System.Windows.Forms.Form.Load> controlador de eventos, porque no se volverá a dibujar el contenido dibujado si el formulario cambia de tamaño u ocultado por otro formulario.  
  
## <a name="see-also"></a>Vea también
- <xref:System.Drawing.CopyPixelOperation>
- <xref:System.Drawing.Graphics.FillRectangle%2A?displayProperty=nameWithType>
- <xref:System.Windows.Forms.Control.OnPaint%2A?displayProperty=nameWithType>
- [Gráficos y dibujos en Windows Forms](../../../../docs/framework/winforms/advanced/graphics-and-drawing-in-windows-forms.md)
- [Utilizar lápiz para dibujar líneas y formas](../../../../docs/framework/winforms/advanced/using-a-pen-to-draw-lines-and-shapes.md)
