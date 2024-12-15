# XPath Expressions from 10/16

1. Hamlet's title under the title statement
``/TEI/teiHeader/fileDesc/titleStmt/title``

2. Head element within div element
``/TEI/text/body/div/head``

3. Looking for lines within an "Act"
``/TEI/text/body/div/div//l``

4. Want to know how many scenes per act
``/TEI/text/body/div/count(div)``
Exclamation means switching to funtion: !
``/TEI/text/body/div!count(div)``

5. 
``/TEI/text/body/div/div =>count()
``/TEI/text/body/div ! count(.)``

``/TEI/text/body/div ! count(.//sp)``

``max(/TEI/text/body/div ! count(.//sp))``
``/TEI/text/body/dov ! count(.//sp) => max``

``/TEI/text/body/div [count(.//sp)=257]/head``

``/TEI/text/body/div [count(.//sp) => max()]/head