# ApiAju Documentation

Official documentation for ApiAju - A public API providing calendar, holidays, and business days information for Aracaju-SE, Brazil.

## 🌐 Live Documentation

Visit the documentation at: [https://docs.api.aju.br](https://docs.api.aju.br) (or your deployed URL)

## 📖 About ApiAju

ApiAju is a free, public REST API designed to provide comprehensive calendar information for Aracaju, the capital city of Sergipe state in Brazil. The API includes:

- 🎉 **Holiday Information**: National, state (Sergipe), and municipal (Aracaju) holidays
- 📊 **Business Days Calculator**: Calculate working days between dates
- 🎯 **Holiday Verification**: Check if any specific date is a holiday
- 📅 **End Date Calculation**: Calculate dates based on business days

## 🚀 Quick Links

- **API Endpoint**: [https://api.aju.br](https://api.aju.br)
- **Source Code**: [github.com/wolney-fo/apiaju](https://github.com/wolney-fo/apiaju)
- **OpenAPI Spec**: [openapi.yml](./openapi.yml)

## 📚 Documentation Structure

This documentation is built with [Mintlify](https://mintlify.com) and includes:

- **Getting Started**: Introduction and quickstart guide
- **Guides**: Use cases, error handling, and best practices
- **API Reference**: Complete endpoint documentation with interactive examples
- **OpenAPI Integration**: Auto-generated API documentation from OpenAPI specification

## 🛠️ Local Development

### Prerequisites

- Node.js version 19 or higher
- npm or yarn

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/wolney-fo/apiaju-docs.git
   cd apiaju-docs
   ```

2. Install the Mintlify CLI:
   ```bash
   npm i -g mintlify
   ```

3. Start the development server:
   ```bash
   mintlify dev
   ```

4. Open your browser at [http://localhost:3000](http://localhost:3000)

### Making Changes

The documentation updates automatically as you edit files. All documentation pages are written in MDX format.

## 📁 Project Structure

```
apiaju-docs/
├── api-reference/          # API endpoint documentation
│   ├── endpoint/          # Individual endpoint pages
│   └── introduction.mdx   # API reference overview
├── images/                # Images and assets
├── logo/                  # Logo files (light/dark mode)
├── index.mdx             # Homepage
├── quickstart.mdx        # Quick start guide
├── use-cases.mdx         # Use cases and examples
├── error-handling.mdx    # Error handling guide
├── best-practices.mdx    # Best practices guide
├── openapi.yml           # OpenAPI specification
├── docs.json             # Mintlify configuration
└── README.md            # This file
```

## 🔧 Configuration

The main configuration is in `docs.json`:

- **Theme**: Maple theme with custom colors (#FF6900)
- **Navigation**: Organized into Getting Started, Guides, and API Reference sections
- **OpenAPI Integration**: Automatically generates endpoint pages from `openapi.yml`
- **Features**: GitHub integration, contextual options, feedback system

## 📝 Writing Documentation

### Adding New Pages

1. Create a new `.mdx` file in the appropriate directory
2. Add frontmatter with title and description:
   ```yaml
   ---
   title: "Page Title"
   description: "Page description"
   ---
   ```
3. Add the page to `docs.json` navigation

### Mintlify Components

The documentation uses Mintlify's MDX components:

- `<Card>`, `<CardGroup>` - For cards and card groups
- `<Accordion>`, `<AccordionGroup>` - For collapsible content
- `<Tabs>`, `<Tab>` - For tabbed content
- `<CodeGroup>` - For multi-language code examples
- `<Steps>`, `<Step>` - For step-by-step guides
- `<Note>`, `<Tip>`, `<Warning>`, `<Info>` - For callouts

### OpenAPI Endpoints

Endpoint pages are automatically generated from `openapi.yml`. To add a new endpoint:

1. Add the endpoint to `openapi.yml`
2. Create a new `.mdx` file in `api-reference/endpoint/`
3. Add the OpenAPI reference:
   ```yaml
   ---
   title: 'Endpoint Name'
   openapi: 'GET /path/to/endpoint'
   ---
   ```

## 🚀 Deployment

### Mintlify Cloud

1. Push changes to your GitHub repository
2. Connect your repository to [Mintlify Dashboard](https://dashboard.mintlify.com)
3. Mintlify will automatically deploy your changes

### Custom Deployment

You can also deploy to any static hosting service (Vercel, Netlify, etc.):

1. Build the documentation:
   ```bash
   mintlify build
   ```
2. Deploy the `_site` directory

## 🐛 Troubleshooting

### CLI Issues

If you encounter issues with the Mintlify CLI:

```bash
# Update to the latest version
npm update -g mintlify

# Check version
mintlify --version
```

### Broken Links

Check for broken links:

```bash
mintlify broken-links
```

### Port Conflicts

Use a different port if 3000 is already in use:

```bash
mintlify dev --port 3333
```

## 🤝 Contributing

Contributions to improve the documentation are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improve-docs`)
3. Make your changes
4. Commit your changes (`git commit -m 'Improve documentation for X'`)
5. Push to the branch (`git push origin feature/improve-docs`)
6. Open a Pull Request

## 📄 License

This documentation is open source and available under the [MIT License](./LICENSE).

## 🔗 Related Projects

- **ApiAju API**: [github.com/wolney-fo/apiaju](https://github.com/wolney-fo/apiaju)
- **Mintlify**: [mintlify.com](https://mintlify.com)

## 📧 Contact

- **GitHub Issues**: [Report issues or request features](https://github.com/wolney-fo/apiaju/issues)
- **API Status**: [Check API health](https://api.aju.br/api/v1/health)

---

Made with ❤️ for Aracaju-SE, Brazil
