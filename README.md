# Deep Directory Tree MCP 🌳

[![Smithery Tool Calls](https://smithery.ai/badge/deep-directory-tree-mcp)](https://smithery.ai/server/deep-directory-tree-mcp)
[![NPM Version](https://img.shields.io/npm/v/%40andredezzy%2Fdeep-directory-tree-mcp.svg)](https://npmjs.org/package/@andredezzy/deep-directory-tree-mcp)
[![NPM Downloads](https://img.shields.io/npm/dm/%40andredezzy%2Fdeep-directory-tree-mcp)](https://npmjs.org/package/@andredezzy/deep-directory-tree-mcp)

A powerful Model Context Protocol (MCP) implementation for visualizing and analyzing directory structures. Why? Now you can let AI assistants understand and navigate your project structure efficiently, enabling smarter code navigation and project organization insights.

Built with:

- [Anthropic MCP](https://docs.anthropic.com/claude/docs/mcp-getting-started)
- [Cursor](https://cursor.sh)

## Features

- Deep directory tree visualization
- Configurable depth-based tree generation
- Smart pattern-based file/directory exclusion
- Clean and readable tree output format
- Real-time directory structure updates
- Targeted directory analysis

**DEMO:**

![Cursor + Deep Directory Tree MCP Demo](./cursor-demo.mp4)

## Quick Start

### Prerequisites

- [Node.js](https://nodejs.org) (v18 or higher)

### Smithery Installation

The easiest way to get started is using [Smithery](https://smithery.ai/server/deep-directory-tree-mcp):

```bash
npx -y @smithery/cli install @andredezzy/deep-directory-tree-mcp --client cursor
```

### Manual Installation

#### Cursor IDE Setup

1. Open Cursor Settings → MCP → Add new MCP server
2. Configure with these settings:

   ```json
   {
     "deep-directory-tree": {
       "command": "npx",
       "args": ["-y", "@andredezzy/deep-directory-tree-mcp"]
     }
   }
   ```

#### Claude Desktop Setup

Add the following to your MCP configuration:

```json
{
  "mcpServers": {
    "deep-directory-tree": {
      "command": "npx",
      "args": ["-y", "@andredezzy/deep-directory-tree-mcp"]
    }
  }
}
```

## Usage

Common commands for AI assistants:

- "Show me the directory structure"
- "Visualize project tree up to depth 4"
- "Show files excluding test directories"

## Development

### Prerequisites

- [Bun Runtime](https://bun.sh) (required)

```bash
# Clone the repository
git clone https://github.com/andredezzy/deep-directory-tree-mcp.git
cd deep-directory-tree-mcp

# Install dependencies
bun install

# Build the project
bun run build
```

### Development Manual Installation

#### Cursor IDE Setup

1. Open Cursor Settings → MCP → Add new MCP server
2. Configure with these settings:

   ```json
   {
     "deep-directory-tree": {
       "command": "node",
       "args": ["ABSOLUTE_PATH_TO_MCP_SERVER/bin/deep-directory-tree.js"]
     }
   }
   ```

#### Claude Desktop Setup

Add the following to your MCP configuration:

```json
{
  "mcpServers": {
    "deep-directory-tree": {
      "command": "node",
      "args": ["ABSOLUTE_PATH_TO_MCP_SERVER/bin/deep-directory-tree.js"]
    }
  }
}
```

## Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Support

Need help? Try these resources:

- [Open an issue](https://github.com/andredezzy/deep-directory-tree-mcp/issues)
- [FAQ Wiki](https://github.com/andredezzy/deep-directory-tree-mcp/wiki/FAQ)
- [Documentation](https://github.com/andredezzy/deep-directory-tree-mcp/wiki)

## License

MIT License - see [LICENSE](LICENSE) file for details.
