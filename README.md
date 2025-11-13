
# NestJS Basic Commands a Developer Should Know

Here's a structured command reference for NestJS development (Windows/Linux/macOS compatible):

## **Installation & Project Setup**
```bash
# Install NestJS CLI globally
npm install -g @nestjs/cli

# Create new NestJS project (interactive setup)
nest new project-name

# Start development server (from project root)
npm run start:dev
```

## **Database & Prisma Setup**
```bash
# Install Prisma as dev dependency
npm install -D prisma

# Initialize Prisma (creates prisma/schema.prisma)
npx prisma init

# Install Prisma Client
npm install @prisma/client

# Generate Prisma Client after schema changes
npx prisma generate

# Run database migrations
npx prisma migrate dev --name migration_name

# Open Prisma Studio (database GUI)
npx prisma studio
```

## **Authentication Packages**
```bash
# Install bcrypt for password hashing
npm install bcrypt
npm install -D @types/bcrypt

# Install JSON Web Tokens (corrected spelling)
npm install jsonwebtoken
npm install -D @types/jsonwebtoken

# OR install NestJS JWT module (recommended)
npm install @nestjs/jwt
```

## **Development Commands**
```bash
# Start in watch mode (auto-reload)
npm run start:dev

# Start in debug mode
npm run start:debug

# Build for production
npm run build

# Start production build
npm run start:prod

# Lint code
npm run lint

# Format code
npm run format
```

## **CRUD Generation**
```bash
# Generate module, service, and controller
nest generate resource users

# Generate individual components
nest generate module users
nest generate controller users
nest generate service users
```

## **Testing**
```bash
# Run unit tests
npm run test

# Run e2e tests
npm run test:e2e

# Run tests in watch mode
npm run test:watch

# Generate coverage report
npm run test:cov
```

## **Package Management**
```bash
# Install dependency
npm install package-name

# Install dev dependency
npm install -D package-name

# Uninstall package
npm uninstall package-name
```

---

### **Key Corrections & Best Practices**
- ✅ Fixed `npm -D prisma` → `npm install -D prisma`
- ✅ Fixed `npm prisma init` → `npx prisma init`
- ✅ Fixed typo: `jsonwebtocken` → `jsonwebtoken`
- ✅ Use `npx` for CLI tools like Prisma
- ✅ Use `@nestjs/jwt` instead of manual JWT implementation when possible

**Pro Tip**: Run `nest --help` to see all available CLI commands!
