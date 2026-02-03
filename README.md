# Strapi Local Setup

A local development setup for the Strapi headless CMS, cloned from the official repository.

## 📋 Project Overview

[Strapi](https://strapi.io) is the leading open-source headless CMS. It's 100% JavaScript/TypeScript, fully customizable, and developer-first.

This repository contains:
- The complete Strapi monorepo cloned from [strapi/strapi](https://github.com/strapi/strapi)
- Configuration for local development
- Sample content types (created via Admin Panel)

---

## 🚀 Getting Started

### Prerequisites

- **Node.js**: v20.x or v22.x (Required by Strapi 5.x)
- **Yarn**: v4.x (package manager)
- **Git**: For version control

### Installation Steps

1. **Clone this repository**
   ```bash
   git clone https://github.com/Vishalldwivedi/strapi-local-setup.git
   cd strapi-local-setup
   ```

2. **Navigate to the Strapi folder**
   ```bash
   cd strapi
   ```

3. **Install dependencies**
   ```bash
   yarn install
   ```

4. **Build the project**
   ```bash
   yarn build
   ```

5. **Start the development server**
   ```bash
   cd examples/getstarted
   yarn develop
   ```

6. **Access the Admin Panel**
   - Open your browser and navigate to: `http://localhost:1337/admin`
   - On first run, create your admin account

---

## 📁 Project Folder Structure

```
strapi-local-setup/
├── strapi/                      # Main Strapi monorepo
│   ├── packages/               # Core packages
│   │   ├── core/              # Core Strapi functionality
│   │   ├── admin-test-utils/  # Admin testing utilities  
│   │   ├── cli/               # Command-line interface
│   │   ├── generators/        # Code generators
│   │   ├── plugins/           # Official plugins
│   │   ├── providers/         # Email, upload providers
│   │   └── utils/             # Utility libraries
│   │
│   ├── examples/              # Example projects
│   │   ├── getstarted/        # ⭐ Main example we use
│   │   ├── complex/           # Complex example
│   │   ├── kitchensink/       # All features example
│   │   └── plugins/           # Plugin examples
│   │
│   ├── docs/                  # Documentation
│   ├── tests/                 # Test suites
│   ├── templates/             # Project templates
│   └── scripts/               # Build scripts
│
└── README.md                   # This file
```

### Key Directories Explained

| Directory | Description |
|-----------|-------------|
| `packages/core` | Core Strapi packages (admin, content-manager, database, etc.) |
| `packages/plugins` | Official plugins (GraphQL, i18n, users-permissions, etc.) |
| `packages/providers` | Upload/email providers (AWS S3, Cloudinary, SendGrid, etc.) |
| `examples/getstarted` | Quickstart example with all basic features configured |

---

## 🎨 Using the Admin Panel

### First-Time Setup

1. Navigate to `http://localhost:1337/admin`
2. Create your admin account:
   - First name, Last name
   - Email address
   - Password (min 8 characters)
3. Click "Let's start"

### Creating a Content Type

1. In the left sidebar, click **Content-Type Builder**
2. Click **Create new collection type**
3. Enter a display name (e.g., "Article")
4. Add fields:
   - `title` - Text (Short text)
   - `content` - Rich text
   - `publishedAt` - Date
5. Click **Save**
6. Wait for the server to restart

### Adding Content

1. Go to **Content Manager** in the sidebar
2. Select your new content type
3. Click **Create new entry**
4. Fill in the fields and **Publish**

---

## 🔧 Available Scripts

From the monorepo root (`strapi/`):

| Script | Description |
|--------|-------------|
| `yarn install` | Install all dependencies |
| `yarn build` | Build all packages |
| `yarn clean` | Clean build artifacts |
| `yarn lint` | Run linter |
| `yarn test:unit` | Run unit tests |

From the example project (`strapi/examples/getstarted/`):

| Script | Description |
|--------|-------------|
| `yarn develop` | Start in development mode (with hot reload) |
| `yarn start` | Start in production mode |
| `yarn build` | Build admin panel |

---

## 📊 Strapi Features

- ✅ **Content Types Builder** - Create custom data structures
- ✅ **Media Library** - Upload and manage files
- ✅ **Internationalization (i18n)** - Multi-language support
- ✅ **Role-Based Access Control** - User permissions
- ✅ **REST & GraphQL APIs** - Flexible data access
- ✅ **Plugin System** - Extend functionality

---

## Proof:
![Strapi Admin Panel](./image.png)

---

## 📚 Resources

- [Strapi Documentation](https://docs.strapi.io)
- [Strapi GitHub Repository](https://github.com/strapi/strapi)
- [Strapi Discord Community](https://discord.strapi.io)

---

## 👤 Author

**Vishal dwivedi**  
GitHub: https://github.com/Vishalldwivedi

---

## 📝 License

This project uses Strapi which is licensed under the [MIT License](https://github.com/strapi/strapi/blob/main/LICENSE).
