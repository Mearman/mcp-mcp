# MCP-MCP Server

[![npm version](https://img.shields.io/npm/v/mcp-mcp.svg)](https://www.npmjs.com/package/mcp-mcp)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

## Build Status
[![CI Build](https://github.com/Mearman/mcp-mcp/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Mearman/mcp-mcp/actions/workflows/ci.yml)
[![Tests](https://img.shields.io/badge/tests-passing-brightgreen)](https://github.com/Mearman/mcp-mcp/actions/workflows/ci.yml)

## Release Status
[![Release](https://github.com/Mearman/mcp-mcp/actions/workflows/semantic-release.yml/badge.svg)](https://github.com/Mearman/mcp-mcp/actions/workflows/semantic-release.yml)

A Model Context Protocol (MCP) server for MCP-related operations and utilities.

**Built with**: [MCP TypeScript Template](https://github.com/Mearman/mcp-template)

## Features

- 🚀 **TypeScript with ES Modules** - Modern JavaScript with full type safety
- 🧪 **Comprehensive Testing** - Vitest with coverage reporting
- 🔧 **Code Quality** - Biome for linting and formatting
- 📦 **Automated Publishing** - Semantic versioning and NPM publishing
- 🛠️ **Development Tools** - Hot reload, watch mode, and CLI support

## Available Tools

### `example_tool`
A basic example tool that demonstrates MCP tool implementation patterns.

**Parameters:**
- `message` (string, required): A message to process
- `count` (number, optional, default: 1): Number of times to repeat the message

**Example:**
```json
{
  "message": "Hello, MCP!",
  "count": 3
}
```

**Response:**
```
1: Hello, MCP!
2: Hello, MCP!
3: Hello, MCP!
```

## Installation

### Using NPM
```bash
npm install -g mcp-mcp
```

### Using Yarn
```bash
yarn global add mcp-mcp
```

### From Source
```bash
git clone https://github.com/Mearman/mcp-mcp.git
cd mcp-mcp
yarn install
yarn build
```

## Usage

### As MCP Server

Add to your MCP client configuration:

```json
{
  "mcpServers": {
    "mcp-mcp": {
      "command": "mcp-mcp",
      "args": []
    }
  }
}
```

### Development

```bash
# Start development server with hot reload
yarn dev

# Run tests
yarn test

# Run tests in watch mode
yarn test:watch

# Build the project
yarn build

# Run linting
yarn lint

# Auto-fix linting issues
yarn lint:fix
```

## Development Status

This server is currently in **development** and serves as a foundation for MCP-related utilities. Future versions may include:

- MCP server discovery and management tools
- Protocol validation utilities
- Server health checking and monitoring
- MCP specification compliance testing

## Configuration

Currently no additional configuration is required. The server runs with default settings suitable for most MCP environments.

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'feat: add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## License

This project is licensed under the [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.

## Related Projects

- [MCP TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk)
- [MCP Specification](https://spec.modelcontextprotocol.io/)
- [MCP Template](https://github.com/Mearman/mcp-template)