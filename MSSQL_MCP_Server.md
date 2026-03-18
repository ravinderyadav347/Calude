### MSSQL MCP Server
A local Model Context Protocol (MCP) server that connects Claude Desktop to your MS SQL Server instance.

##📋 Prerequisites

-Node.js v18 or higher
-Claude Desktop installed
-Access to your MS SQL Server instance

Here's your complete local MCP Server for MS SQL. Here's how to set it up:
## Step 1 — Create the project folder
mkdir mssql-mcp-server
cd mssql-mcp-server

Copy both index.js and package.json into that folder.

## Step 2 — Install dependencies
npm install

## Step 3 — Test it runs
node index.js

You should see: MSSQL MCP Server running on stdio

## Step 4 — Register with Claude Desktop
Open your Claude Desktop config file:

Windows: %APPDATA%\Claude\claude_desktop_config.json
Mac: ~/Library/Application Support/Claude/claude_desktop_config.json

Paste in the config from the third file, replacing the path with your actual folder path. Then restart Claude Desktop.


Available MCP Tools once connected:

ToolWhat it doesqueryRun SELECT queries, returns JSON rowsexecuteRun INSERT / UPDATE / DELETE / DDLlist_tablesList all tables in CXSA1CashAndCarry_QA66describe_tableShow columns & types for any tablelist_stored_proceduresList all stored procedures