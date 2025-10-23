Copy
Working with Diagrams
Class Diagram
Create Class Diagram
To create a Class Diagram:
First select an element where a new Class Diagram to be contained as a child.
Select 
Model | Add Diagram | Class Diagram
 in the Menu Bar or select 
Add Diagram | Class Diagram
 in Context Menu.
See also
UML Class Diagram
 - For more information about UML Class Diagram.
Model Element
Model Element is an abstract element of all UML model elements.
You can use 
QuickEdit
 for Model Element by double-click or press 
Enter
 on a selected model element.
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
Add Note
 : Add a linked note.
Classifier
Classifier is an abstract element of:
Class
Interface
Signal
DataType
PrimitiveType
Enumeration
Component
Artifact
You can use 
QuickEdit
 for Classifier by double-click or press 
Enter
 on a selected classifier.
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
Add Note
 : Add a linked note.
Add Attribute
 (
Ctrl+Enter
) : Add an attribute.
Add Operation
 (
Ctrl+Shift+Enter
) : Add an operation.
Add Reception
 : Add a reception.
Class
To create a Class:
Select 
Class
 in 
Toolbox
.
Drag on the diagram as the size of Class.
To create a Class (model element only) by Menu:
Select an Element where a new Class to be contained.
Select 
Model | Add | Class
 in Menu Bar or 
Add | Class
 in Context Menu.
You can use 
QuickEdit
 for Class by double-click or press 
Enter
 on a selected Class.
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
Add Note
 : Add a linked note.
Add Attribute
 (
Ctrl+Enter
) : Add an attribute.
Add Operation
 (
Ctrl+Shift+Enter
) : Add an operation.
Add Template Parameter
 : Add a template parameter.
Add Reception
 : Add a reception.
Add Sub-Class
 : Add a sub-class.
Add Super-Class
 : Add a super class.
Add Provided Interface
 : Add a provided interface.
Add Required Interface
 : Add a required interface.
Add Associated Class
 : Add an associated class.
Add Aggregated Class
 : Add an aggregated class.
Add Composited Class
 : Add a composited class.
Add Port
 : Add a port.
Add Part
 : Add a part.
To suppress Attributes, see 
Suppress Attributes
.
To suppress Operations, see 
Suppress Operations
.
To suppress Receptions, see 
Suppress Receptions
.
To show or hide Operation Signatures, see 
Show Operation Signature
.
Attribute
To add an Attribute:
Select a Classifier.
Select 
Model | Add | Attribute
 in Menu Bar or 
Add | Attribute
 in Context Menu.
You can use 
QuickEdit
 for Attribute by double-click or press 
Enter
 on a selected Attribute.
Attribute Expression
 : Edit Attribute expression.
Syntax of Attribute Expression
Copy
attribute ::= [ '<<' stereotype `>>` ] [ visibility ] name [':' type ] [ '[' multiplicity ']' ] [ '=' defaut-value ]


stereotype ::= (identifier)


visibility ::= '+' | '#' | '-' | '~'


name ::= (identifier)


type ::= (identifier)


multiplicity ::= multiplicity-bound [ '..' multiplicity-bound ]


multiplicity-bound ::= (number) | '*'


default-value ::= (string)
Visibility
 : Change visibility property.
Add
 (
Ctrl+Enter
) : Add one more attribute in the below.
Delete
 (
Ctrl+Delete
) : Delete the attribute
Move Up
 (
Ctrl+Up
) : Move the attribute up.
Move Down
 (
Ctrl+Down
) : Move the attribute down.
Operation
To add an Operation:
Select a Classifier.
Select 
Model | Add | Operation
 in Menu Bar or 
Add | Operation
 in Context Menu.
You can use 
QuickEdit
 for Operation by double-click or press 
Enter
 on a selected Operation.
Operation Expression
 : Edit Operation expression.
Syntax of Operation Expression
Copy
operation ::= [ '<<' stereotype `>>` ] [ visibility ] name [ '(' parameter-list ')' ] [ ':' return-type ]


stereotype ::= (identifier)


visibility ::= '+' | '#' | '-' | '~'


name ::= (identifier)


parameter-list ::= parameter [ ',' parameter ]*


parameter ::= (identifier)


return-type ::= (identifier)
Visibility
 : Change visibility property.
Add
 (
Ctrl+Enter
) : Add one more operation in the below.
Delete
 (
Ctrl+Delete
) : Delete the operation
Move Up
 (
Ctrl+Up
) : Move the operation up.
Move Down
 (
Ctrl+Down
) : Move the operation down.
To add a Parameter, see 
Parameter
.
To show or hide Operation Signatures, see 
Show Operation Signature
.
Parameter
To add a Parameter:
Select an Operation.
Select 
Model | Add | Parameter
 in Menu Bar or 
Add | Parameter
 in Context Menu.
Template Parameter
To add a Template Parameter:
Select an Element.
Select 
Model | Add | Template Parameter
 in Menu Bar or 
Add | Template Parameter
 in Context Menu.
You can use 
QuickEdit
 for Template Parameter by double-click or press 
Enter
 on a selected Template Parameter.
Template Parameter Expression
 : Edit Template Parameter expression.
Syntax of Template Parameter Expression
Copy
template-parameter ::= [ '<<' stereotype `>>` ] [ visibility ] name [':' type ] [ '=' defaut-value ]


stereotype ::= (identifier)


visibility ::= '+' | '#' | '-' | '~'


name ::= (identifier)


type ::= (identifier)


default-value ::= (string)
Visibility
 : Change visibility property.
Add
 (
Ctrl+Enter
) : Add one more template parameter in the below.
Delete
 (
Ctrl+Delete
) : Delete the template parameter.
Move Up
 (
Ctrl+Up
) : Move the template parameter up.
Move Down
 (
Ctrl+Down
) : Move the template parameter down.
Template Parameter Substitution
To add a Template Parameter Substituion:
Select a Template Binding element.
Select 
Model | Add | Template Parameter Substitution
 in Menu Bar or 
Add | Template Parameter Substitution
 in Context Menu.
Each 
Template Parameter Substitution
 should have 
formal
 property assigned to a 
Template Parameter
 of the template element and 
actual
 property assigned to the actual value for the template parameter.
Interface
To create an Interface:
Select 
Interface
 in 
Toolbox
.
Drag on the diagram as the size of Interface.
To create an Interface (model element only) by Menu:
Select an Element where a new Interface to be contained.
Select 
Model | Add | Interface
 in Menu Bar or 
Add | Interface
 in Context Menu.
You can use 
QuickEdit
 for Interface by double-click or press 
Enter
 on a selected Interface.
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
Add Note
 : Add a linked note.
Add Attribute
 (
Ctrl+Enter
) : Add an attribute.
Add Operation
 (
Ctrl+Shift+Enter
) : Add an operation.
Add Reception
 : Add a reception.
Add Sub-Interface
 : Add a sub-interface.
Add Super-Interface
 : Add a super interface.
Add Realizing Class
 : Add an realizing class.
To show an Interface as Lollipop notation, Interface should be realized (See 
Interface Realization
) and then change Stereotype Display to Icon or Icon with Label (See 
Stereotype Display
).
To show an Interface as Socket notation, Interface should have dependants (See 
Dependency
) and then change Stereotype Display to Icon or Icon with Label (See 
Stereotype Display
).
To suppress Attributes, see 
Suppress Attributes
.
To suppress Operations, see 
Suppress Operations
.
To suppress Receptions, see 
Suppress Receptions
.
To show or hide Operation Signatures, see 
Show Operation Signature
.
Signal
To create a Signal:
Select 
Signal
 in 
Toolbox
.
Drag on the diagram as the size of Signal.
To create a Signal (model element only) by Menu:
Select an Element where a new Signal to be contained.
Select 
Model | Add | Signal
 in Menu Bar or 
Add | Signal
 in Context Menu.
You can use 
QuickEdit
 for Classifier (See 
Classifier
).
DataType
To create a DataType:
Select 
DataType
 in 
Toolbox
.
Drag on the diagram as the size of DataType.
To create a DataType (model element only) by Menu:
Select an Element where a new DataType to be contained.
Select 
Model | Add | DataType
 in Menu Bar or 
Add | DataType
 in Context Menu.
You can use 
QuickEdit
 for Classifier (See 
Classifier
).
PrimitiveType
To create a PrimitiveType:
Select 
PrimitiveType
 in 
Toolbox
.
Drag on the diagram as the size of PrimitiveType.
To create a PrimitiveType (model element only) by Menu:
Select an Element where a new PrimitiveType to be contained.
Select 
Model | Add | PrimitiveType
 in Menu Bar or 
Add | PrimitiveType
 in Context Menu.
You can use 
QuickEdit
 for Classifier (See 
Classifier
).
Enumeration
To create an Enumeration:
Select 
Enumeration
 in 
Toolbox
.
Drag on the diagram as the size of Enumeration.
To create an Enumeration (model element only) by Menu:
Select an Element where a new Enumeration to be contained.
Select 
Model | Add | Enumeration
 in Menu Bar or 
Add | Enumeration
 in Context Menu.
You can use 
QuickEdit
 for Enumeration by double-click or press 
Enter
 on a selected Enumeration.
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
Add Note
 : Add a linked note.
Add Literal
 (
Ctrl+Enter
) : Add an enumeration literal.
Add Operation
 (
Ctrl+Shift+Enter
) : Add an operation.
To suppress Literals, see see 
Suppress Literals
.
Enumeration Literal
To add an Enumeration Literal:
Select a Classifier.
Select 
Model | Add | Enumeration Literal
 in Menu Bar or 
Add | Enumeration Literal
 in Context Menu.
You can use 
QuickEdit
 for Enumeration Literal by double-click or press 
Enter
 on a selected Enumeration Literal.
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
Add
 (
Ctrl+Enter
) : Add one more literal in the below.
Delete
 (
Ctrl+Delete
) : Delete the literal
Move Up
 (
Ctrl+Up
) : Move the literal up.
Move Down
 (
Ctrl+Down
) : Move the literal down.
Relationship
Relationship is an abstract element representing a relationship between UML elements.
Subclasses of Relationship are:
Generalization
Association
Aggregation
Composition
Dependency
Interface Realization
Component Realization
Include
Exclude
You can use 
QuickEdit
 by double-click or press 
Enter
 on a selected relationship.
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
Add Note
 : Add a linked note.
Generalization
To create a Generalization:
Select 
Generalization
 in 
Toolbox
.
Drag from an element (to be special) and drop on another element (to be general).
You can use 
QuickEdit
 for Relationship (See 
Relationship
).
Association
To create an Association (or Directed Association):
Select 
Association
 (or 
Directed Association
) in 
Toolbox
.
Drag from an element and drop on another element.
You can use 
QuickEdit
 for Relationship (See 
Relationship
).
You can also use 
QuickEdit
 for Association End by double-click at the end side of an Association.
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
Aggregation Kind
 : Change aggregationKind property.
Multiplicity
 : Change multiplicity property.
Add Qualifier
 : Add a qualifier (attribute) to the AssociationEnd.
Aggregation
To create an Aggregation:
Select 
Aggregation
 in 
Toolbox
.
Drag from an element (to be a part) and drop on another element (to be whole).
You can use 
QuickEdit
 for Relationship (See 
Relationship
).
You can also use 
QuickEdit
 for AssociationEnd by double-click at the end side of an Association (See 
Association
).
Note
Aggregation is an association whose 
aggregation
 propery is 
shared
.
Composition
To create a Composition:
Select 
Composition
 in 
Toolbox
.
Drag from an element (to be a part) and drop on another element (to be whole).
You can use 
QuickEdit
 for Relationship (See 
Relationship
).
You can also use 
QuickEdit
 for AssociationEnd by double-click at the end side of an Association (See 
Association
).
Note
Composition is an association whose 
aggregation
 propery is 
composite
.
Dependency
To create an Dependency:
Select 
Dependency
 in 
Toolbox
.
Drag from an element (client) and drop on another element (supplier).
You can use 
QuickEdit
 for Relationship (See 
Relationship
).
Interface Realization
To create an Interface Realization:
Select 
Interface Realization
 in 
Toolbox
.
Drag from an element (realizing) and drop on an interface (to be realized).
You can use 
QuickEdit
 for Relationship (See 
Relationship
).
Association Class
To create an Association Class by linking two Classifiers:
Select 
Association Class
 in 
Toolbox
.
Drag from an element and drop on another element.
An Association and a Class connected to the association will be created.
To create an Association Class by linking Association and Class:
Select 
Association Class
 in 
Toolbox
.
Drag from an Association (or Class) and drop on a Class (or Association).
The Class will be connected to the Association.
Template Binding
To create a Template Binding:
Select 
Template Binding
 in 
Toolbox
.
Drag from a bound element and drop on a template element.
If required, create 
Template Parameter Substitution
.
You can use 
QuickEdit
 for Template Binding by double-click or press 
Enter
.
Visibility
 : Change visibility property.
Add Note
 : Add a linked note.
Add Template Parameter
 : Add a template parameter substitution.
Frame
To create a Frame view of a particular model element:
Select 
Frame
 in 
Toolbox
.
Drag on the diagram as the size of Frame.
Select a model element which the Frame represents in 
Element Picker Dialog
Previous
Keyboard Shortcuts
Next
Package Diagram
Last updated 
6 years ago