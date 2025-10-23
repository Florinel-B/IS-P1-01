Copy
User Guide
CLI (Command Line Interface)
StarUML can be used as CLI (Command Line Interface) in terminal. With the CLI feature, you can generate various artifacts including source codes, documents (markdown, HTML, etc.), diagram images without launching StarUML GUI. Therefore, you can use CLI in your build script to automate   artifacts generation based on your software model.
Creating Alias
MacOS
It is useful to make an alias for StarUML application in terminal as below:
Copy
$ alias staruml='/Applications/StarUML.app/Contents/MacOS/StarUML'
Windows
You can create an alias for StarUML application in PowerShell as below:
Copy
PS> Set-Alias -Name staruml -Value 'C:\Program Files\StarUML\StarUML.exe'
Linux
In Linux, you don't need to create alias. If you installed StarUML successfully, you can run with 
staruml
 in Terminal without additional configuration.
Commands
You can use four commands in CLI mode. If you omit the supported commands, StarUML will be launched as GUI mode.
You can see what kind of commands are supported by typing with help (
--help
) option.
Copy
$
 
staruml
 
--help


$
 
staruml
 
ejs
 
--help
    
# help for ejs command


$
 
staruml
 
image
 
--help
  
# help for image command


$
 
staruml
 
html
 
--help
   
# help for html command


$
 
staruml
 
pdf
 
--help
    
# help for pdf command


$
 
staruml
 
exec
 
--help
   
# help for exec command
ejs
The 
ejs
 command allow to generate textual artifacts from a user's software model file (.mdj). You can write your own templates with 
EJS (Embedded JavaScript templating)
. You can find simple examples for EJS at 
https://github.com/staruml/staruml-cli-examples
.
You can generate textual artifacts with the below CLI command:
Copy
$ staruml ejs <file> <options>
<file>
 : A model file (.mdj) to load
option 
-t
, 
--template
 : A template file (.ejs) to apply
option 
-o
, 
--output
 : output file name (default: 
output.txt
)
option 
-s
, 
--select
 : query to select elements (default: 
@Project
)
Here is an example to generate a HTML file.
Copy
$ staruml ejs myproject.mdj \


  -t class-list.ejs \


  -o class-list.html
You can generate multiple files with the select option as below:
Copy
$ staruml ejs myproject.mdj \


  -t java-class.ejs \


  -s @UMLClass \


  -o "out/<%=filenamify(element.name)%>.java"
This command selects all classes (UMLClass type) in 
myproject.mdj
 and then apply the 
java-class.ejs
 template for each class and save it as a 
.java
 file with the name of the class. You can get more information about the query expression to select elements at the 
retrieving elements by query
 section.
Note that you can also use EJS template syntax in the output option. Sometimes the element name cannot be used as a filename (including special characters like 
/
, 
!
, 
#
, 
?
, etc.). You can use 
filename()
 function to convert a string to a legal filename string in output option like 
-o "out/<%=filenamify(element.name)%>.java"
.
In EJS template string (in .ejs files or in output option), you can use below variables:
app
 : The application object. (See 
Application Context
)
element
 : The element retrieved by the select option.
filenamify
 : A function convert a string to a legal filename string. (See 
https://github.com/sindresorhus/filenamify
)
image
The 
image
 command allows you can generate image files for diagrams:
Copy
$ staruml image <file> <options>
<file>
 : A model file (.mdj) to load
option 
-f
, 
--format
 : image file format. One of 
png
, 
jpeg
, or 
svg
. (default: 
png
)
option 
-o
, 
--output
 : output file name.
option 
-s
, 
--select
 : query to select diagrams (default: 
@Diagram
)
Here is an example to export all diagrams as PNG images in 
out
 folder:
Copy
$ staruml image myproject.mdj \


  -f png \


  -o "out/<%=filenamify(element.name)%>.png"
html
The 
html
 command allows you can generate HTML docs for the model file:
Copy
$ staruml html <file> <options>
<file>
 : A model file (.mdj) to load
option 
-o
, 
--output
 : output path. (default: 
./html-docs
)
Here is an example to generate HTML docs:
Copy
$ staruml html myproject.mdj
pdf
The pdf command allows you can generate PDF document for diagrams:
Copy
$ staruml pdf <file> <options>
<file>
 : A model file (.mdj) to load
option 
-o
, 
--output
 : output file name. (default: 
output.pdf
)
option 
-s
, 
--select
 : query to select diagrams (default: 
@Diagram
)
option 
-z
, 
--size
 : page size. One of 4A0, 2A0, A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, B0, B1, B2, B3, B4, B5, B6, B7, B8, B9, B10, C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, RA0, RA1, RA2, RA3, RA4, SRA0, SRA1, SRA2, SRA3, SRA4, Executive, Folio, Legal, Letter, Tabloid (default: 
A4
).
option 
-l
, 
--layout
 : page layout. 
landscape
 or 
portrait
. (default: 
landscape
)
option 
-n
, 
--showname
 : Show diagram name on page top. 
yes
 or 
no
. (default: 
yes
)
Here is an example to generate PDF document (A3-sized portrait) including all diagrams:
Copy
$ staruml pdf myproject.mdj \


  -o doc.pdf \


  -z A3 \


  -l portrait
exec
The exec command allows you can execute a command:
Copy
$ staruml exec <file> <options>
<file>
 : A model file (.mdj) to load before executing a command
option 
-c
, 
--command
 : command id. (e.g. 
application:main-log
)
option 
-a
, 
--arg
 : argument for the command
Here is an example to execute a command:
Copy
$ staruml exec myproject.mdj \


  --command application:main-log \


  --arg hello
Previous
User Interface
Next
Validation Rules
Last updated 
3 years ago