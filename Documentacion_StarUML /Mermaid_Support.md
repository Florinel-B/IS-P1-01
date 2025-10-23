Copy
User Guide
Mermaid Support
Generate Diagram by Mermaid
Mermaid
 is a diagramming tool that renders Markdown-inspired text definitions into visual diagrams. It is a powerful way to create and visualize various types of diagrams, including flowcharts, sequence diagrams, class diagrams, and more, directly from text.
To  generate diagrams by Mermaid:
Select 
Tools > Generate Diagram by Mermaid
 menu.
Enter mermaid code and click 
Generate
 button.
Select a package where the generated diagram and elements to be contained.
Supported Mermaid Diagrams
StarUML support the following Mermaid diagrams:
Class Diagram
Sequence Diagram
State Diagram
Flowchart
Entity Relationship Diagram
Requirement Diagram
Mindmap
Please refer to the 
official documentation
 for the specific Mermaid syntax.
There may be differences in style, layout, etc. between the diagram generated in StarUML using Mermaid syntax and the actual rendering of Mermaid.
Class Diagram
You can create a class diagram with Mermaid. Keep in mind that the class diagram syntax in Mermaid is different from the UML specification. For example, an attribute is written as 
age: int
 in UML, but as 
int age
 in Mermaid. For more details, refer to the official Mermaid documentation.
Here is an example code for class diagram.
Copy
classDiagram


    note "From Duck till Zebra"


    Animal <|-- Duck


    note for Duck "can fly\ncan swim\ncan dive\ncan help in debugging"


    Animal <|-- Fish


    Animal <|-- Zebra


    Animal : +int age


    Animal : +String gender


    Animal: +isMammal()


    Animal: +mate()


    class Duck{


        +String beakColor


        +swim()


        +quack()


    }


    class Fish{


        -int sizeInFeet


        -canEat()


    }


    class Zebra{


        +bool is_wild


        +run()


    }
Mermaid for StarUML do not support followings in class diagram:
Namespaces
Styling and classes
Markdown formatting
Links
Interactions
Sequence Diagram
A sequence diagram illustrates how objects interact in a particular scenario of a use case. It shows the sequence of messages exchanged between the objects to perform a specific function. Here is an example code for sequence diagram.
Copy
sequenceDiagram


    Alice->>Bob: Hello Bob, how are you ?


    Bob->>Alice: Fine, thank you. And you?


    create participant Carl


    Alice->>Carl: Hi Carl!


    create actor D as Donald


    Carl->>D: Hi!


    destroy Carl


    Alice-xCarl: We are too many


    Bob->>Alice: I agree
Message types that do not exist in the UML specification are not supported.
Lines without arrowheads
Lines with a cross at the end
Lines with bidirectional arrowheads
Dotted lines with arrowheads treated as 
asyncSignal
 type. 
In StarUML, activation cannot be controlled on a per-message basis. Therefore, if even a single message has an activation, the activation is shown throughout the entire diagram.
Mermaid for StarUML do not support followings in sequence diagram:
Group/Box
Background color
Styles and classes
Actor menu
State Diagram
A state diagram is a graphical representation of a system that shows its states, transitions, and events. Each state depicts a unique situation in the system, while transitions indicate how the system moves from one state to another based on events or conditions. Here is an example code for state diagram.
Copy
stateDiagram-v2


    [*] --> Still


    Still --> [*]




    Still --> Moving


    Moving --> Still


    Moving --> Crash


    Crash --> [*]
Mermaid for StarUML do not support followings in state diagram:
Composite state
Concurrency
Styles and classes
Markdown formatting
Flowchart
A flowchart is a visual representation of a process, system, or algorithm. It uses symbols like arrows, rectangles, ovals, and diamonds to depict the flow of steps, decisions, and information, allowing for easy understanding and communication of complex processes. Here is an example code for flowchart.
Copy
flowchart TD


    A[Start] --> B{Is it?}


    B -->|Yes| C[OK]


    C --> D[Rethink]


    D --> B


    B ---->|No| E[End]    
Mermaid for StarUML do not support followings in flowchart:
Some node shapes (asymmetric, parallelogram alt, trapezoid, and double circle)
Expanded node shapes and special shapes
Link types and arrow types except solid arrows (means flow)
Animation, interaction, style, classes and icons
Markdown formatting
Subgraph
Entity Relationship Diagram
An Entity Relationship Diagram (ERD) is a graphical representation of entities and their relationships in a database. It is a critical tool in database design that helps visualize how data is structured and how different entities interact within the system. Here is an example code for entity relationship diagram.
Copy
erDiagram


    CUSTOMER ||--o{ ORDER : places


    CUSTOMER {


        string name


        string custNumber


        string sector


    }


    ORDER ||--|{ LINE-ITEM : contains


    ORDER {


        int orderNumber


        string deliveryAddress


    }


    LINE-ITEM {


        string productCode


        int quantity


        float pricePerUnit


    }
Mermaid for StarUML do not support followings in entity relationship diagram:
Markdown formatting
Styling and classes
Requirement Diagram
A requirement diagram is a visual representation used to capture, categorize, and manage requirements in a system or project. Primarily used in systems engineering and software engineering, it helps stakeholders understand requirement relationships and hierarchies. Here is an example code for requirement diagram.
Copy
requirementDiagram


    requirement test_req {


        id: 1


        text: the test text.


        risk: high


        verifymethod: test


    }


    


    element test_entity {


        type: simulation


    }


    


    test_entity - satisfies -> test_req
Mermaid for StarUML do not support followings in requirement diagram:
Markdown formatting
Styles and classes
Mindmap
A mindmap is a visual tool used for organizing information hierarchically. It starts with a central idea and branches out into related subtopics, helping to generate, organize, and visualize ideas or concepts. Mindmaps are useful for brainstorming and planning as they encourage a free flow of ideas. Here is an example code for mindmap.
Copy
mindmap


  root((mindmap))


    Origins


      Long history


      Popularisation


        British popular psychology author Tony Buzan


    Research


      On effectiveness and features


      On Automatic creation


        Uses


            Creative techniques


            Strategic planning


            Argument mapping


    Tools


      Pen and paper


      Mermaid
Mermaid for StarUML do not support followings in mindmap:
Node shapes
Icon and classes
Markdown formatting
Previous
Customization
Next
AI integration via MCP
Last updated 
5 months ago