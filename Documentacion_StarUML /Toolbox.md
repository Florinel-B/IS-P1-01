Copy
Developing Extensions
Toolbox
If you want to add your tool items in 
Toolbox
, you need to define a toolbox JSON in your extension. The toolbox JSON files should be placed in 
toolbox/
 folder in your extension.
Copy
my-extension/


└─ toolbox/


   └─ toolbox.json
Tool Group
The toolbox JSON defines an array of Tool Group definitions as below:
Copy
[


  {


    
"label"
:
 
"Tool Group 1"
,


    
"id"
:
 
"tool-group-1"
,


    
"diagram-types"
:
 [ 
"UMLClassDiagram"
 ]
,


    
"items"
:
 [


      {


        
"label"
:
 
"Tool Item 1"
,


        
"id"
:
 
"tool-item-1"
,


        
"icon"
:
 
"icon-UMLClass"
,


        
"rubberband"
:
 
"rect"
,


        
"command"
:
 
"my:add-element"
,


        
"command-arg"
:
 {


          
"id"
:
 
"UMLClass"
,


          
"stereotype"
:
 
"my-stereotype"


        }


      }
,


      ...


    ]


  }
,


  ...


]
label
 : The tool group title shown in the Toolbox.
id
 : Unique identifier.
diagram-types
 : A list of diagram types. The tool group will be shown only when one of the diagram-types is active. (e.g. 
"UMLClassDiagram"
, 
"UMLUseCaseDiagram"
, ...)
items
 : A list of tool item definitions.
Tool Item
A tool item represents an element that users can create on a diagram.
label
 : The tool item title shown in the Toolbox
id
 : Unique identifier of the tool item.
icon
 : Icon CSS class name. You can specify already defined icon names (e.g. 
"icon-UMLClass"
, 
"icon-UMLPackage"
, ...) or your own CSS class name in stylesheets of your extension.
rubberband
 : A type of rubberband. One of 
"rect"
(for sizable node-type elements),  
"line"
(for edge-type elements), 
"point"
(for fixed-size node-type elements).
command
 : A command name to be executed.
command-arg
 : An argument object will be passed to the command.
Command
A command used for tool item should create an element on a diagram. We strongly recommend to use 
app.factory.createModelAndView()
 function to create an element. See the 
section
 for more detail.
Toolbox will pass 
options
 object to the command. The passed 
options
 parameter contains:
diagram
 : The active diagram.
id
 : The identifier of tool item.
x1
, 
y1
, 
x2
, 
y2
 : The user dragged area on the diagram.
... : 
command-arg
 are combined.
main.js
Copy
function handleAddElement (options) {


  options = Object.assign(options, {


    'model-init': {


      'stereotype': options.stereotype


    },


    'view-init': {


      'stereotypeDisplay': 'icon',


      'suppressAttributes': true,


      'suppressOperations': true


    }


  })


  return app.factory.createModelAndView(options)


}




app.commands.register('my:add-element', handleAddElement)
Previous
Keymaps
Next
Accessing Elements
Last updated 
3 years ago