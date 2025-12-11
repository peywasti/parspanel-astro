# AGENTS.md

## Commands
- **Build**: `npm run build` - Builds the Astro project for production
- **Dev**: `npm run dev` - Starts development server
- **Preview**: `npm run preview` - Previews the built project
- **Lint**: No linting configured - consider adding ESLint
- **Test**: No testing framework configured - consider adding Vitest or Jest
- **Single test**: Not available - add testing framework first

## Code Style Guidelines

### Imports
- Use ES6 imports with named exports preferred
- Group imports: external libraries first, then internal modules
- Use absolute imports for internal modules when possible

### Formatting
- Use 2 spaces for indentation (Astro/TypeScript default)
- Max line length: 100 characters
- Use semicolons

### Types
- Use TypeScript strict mode (enabled via astro/tsconfigs/strict)
- Prefer explicit types over `any`
- Use interfaces for object shapes, types for unions/primitives

### Naming Conventions
- **Files**: kebab-case for Astro pages/components (e.g., `my-page.astro`)
- **Components**: PascalCase (e.g., `MyComponent`)
- **Variables/Functions**: camelCase
- **Types/Interfaces**: PascalCase
- **Constants**: UPPER_SNAKE_CASE

### Error Handling
- Use try/catch for async operations
- Prefer throwing Error objects with descriptive messages
- Handle errors at appropriate levels (component/page level)

### Styling
- Use Tailwind CSS for all styling
- Prefer utility classes over custom CSS
- Use dark mode variants (dark:) for theme support
- Import global styles in page frontmatter

### Astro Specific
- Use `.astro` for page components
- Prefer frontmatter script over inline scripts
- Avoid scoped styles - use Tailwind utilities instead