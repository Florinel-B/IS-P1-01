Copy
User Guide
AI integration via MCP
StarUML supports integration with various AI services (such as Claude Desktop, Cursor, etc.) through the MCP server. The StarUML MCP Server is open-sourced in the GitHub repository. Installation and usage instructions are described in detail in the repository.
StarUML MCP Server
https://github.com/staruml/staruml-mcp-server
Configure API Server
The MCP Server communicates with StarUML's API Server using the HTTP protocol. You can disable the API Server or change the communication port.
If you want to configure API server, you can edit 
settings.json
 at the user configuration path:
/Users/<user>/Library/Application Support/StarUML
 for Mac OS.
C:\Users\<user>\AppData\Roaming\StarUML
 for Windows.
~/.config/StarUML
 for Linux.
To control whether the API Server runs, modify the 
apiServer
 field. To change the API Server port number, edit the 
apiServerPort
 field as below. Default port number is 
58321
.
Copy
{


  ...


  "apiServer": true,


  "apiServerPort": 58321


}
Previous
Mermaid Support
Next
Class Diagram
Last updated 
3 months ago