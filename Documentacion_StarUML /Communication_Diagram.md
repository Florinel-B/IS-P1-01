Copy
Working with Diagrams
Communication Diagram
Create Communication Diagram
To create a Communication Diagram:
Select first an element where a new Communication Diagram to be contained as a child.
Select 
Model | Add Diagram | Communication Diagram
 in Menu Bar or select 
Add Diagram | Communication Diagram
 in Context Menu.
See also
UML Communication Diagram
 - For more information about UML Communication Diagram.
You can show or hide sequence numbers of messages. To show or hide sequence numbers of message:
Check or Uncheck 
showSequenceNumber
 property of 
Sequence Diagram
 or 
Communication Diagram
.
Lifeline
To create a Lifeline:
Select 
Lifeline
 in 
Toolbox
.
Drag on the diagram as the size of Lifeline.
To create a Lifeline from a Classifier (Class, Interface, etc.) by Drag-and-Drop:
Drag a Classifier from 
Explorer
.
Drop on the diagram.
You can use 
QuickEdit
 for Lifeline by double-click or press 
Enter
 on a selected Lifeline.
Lifeline Expression
 : Edit lifeline expression.
Syntax of Lifeline Expression
Copy
lifeline ::= [ '<<' stereotype `>>` ] [ visibility ] name [ '[' selector ']' ] [ ':' type ]


stereotype ::= (identifier)


visibility ::= '+' | '#' | '-' | '~'


name ::= (identifier)


selector ::= (string)


type ::= (identifier)
Visibility
 : Change visibility property.
Add Note
 : Add a linked note.
Select Type
 : Select a type of the lifeline.
Create Type
 : Create a Class as a type of the lifeline.
Add Connected Lifeline
 : Add a lifeline with a connector.
Add Create Message with Lifeline
 : Add a create message with a lifeline.
Add Self Connector
 : Add a self connector.
Add Forward Message
 : Add a forward message with a connected lifeline.
Add Reverse Message
 : Add a reverse message with a connected lifeline.
Connector
To create an Connector (or Self Connector):
Select 
Connector
 (or 
Self Connector
) in 
Toolbox
.
Drag from a Lifeline and drop on another Lifeline. (Just click on a Lifeline if you want to create a Self Connector.)
You can use 
QuickEdit
 for Connector by double-click or press 
Enter
 on a selected Connector.
Name Expression
 : Edit name expression.
Syntax of Name Expression
Copy
expression ::= [ '<<' stereotype `>>` ] [ visibility ] name


stereotype ::= (identifier)


visibility ::= '+' | '#' | '-' | '~'


name ::= (identifier)
Visibility
 : Change visibility property.
Navigability
 : Change navigability property.
Add Forward Message
 : Add a forward message on the connector.
Add Reverse Message
 : Add a reverse message on the connector.
Message
To create a Forward Message:
Select 
Forward Message
 in 
Toolbox
.
Click on a Connector.
To create a Reverse Message:
Select 
Reverse Message
 in 
Toolbox
.
Click on a Connector.
You can use custom sequence numbers instead of auto-generated integer sequence numbers.
Enter sequence number for each Message's 
sequenceNumber
 property.
Change 
sequenceNumbering
 property of 
Sequence Diagram
 or 
Communication Diagram
 to 
custom
.
You can use 
QuickEdit
 for Message (See 
Message
).
Previous
Sequence Diagram
Next
Statechart Diagram
Last updated 
6 years ago