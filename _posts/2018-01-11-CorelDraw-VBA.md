---
categories: cdr
---
```vb
Public Sub TextTranslate()
    ActiveDocument.BeginCommandGroup "Text Translate"
    For Each shp In ActivePage.Shapes
        shp.Text.Story.Text = "hello, world"
    Next shp
    ActiveDocument.EndCommandGroup
End Sub
```

> In CorelDRAW 11, text is manipulated as a TextRange. Text ranges can be accessed via any of the following properties of Shape.Text:

> Frames collection - each TextFrame ’s default member is a TextRange
which is the text within the frame

> Story - this is a TextRange containing all the text in all of the frames linked to the current Shape on all pages in the document

See [VBA Programming Guide for CorelDRAW 11](http://apps.corel.com/partners_developers/csp/resources/dvba_pg.pdf)
