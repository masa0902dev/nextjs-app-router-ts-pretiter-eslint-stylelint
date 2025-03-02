# NextJS App Router Starter with TypeScript, Prettier, ESLint, and Stylelint

This is a boilerplate for starting a Next.js project with the App Router feature enabled.  
The project is preconfigured with TypeScript, Prettier, ESLint, and Stylelint to provide a foundation for building NextJS project.

## formatter, linter

Prettier: Automated code formatting.  
ESLint: Linting for ts, tsx files.  
Stylelint: Linting for css,scss,module.scss files.  

## Installation

Clone this repository:

```bash
git clone https://github.com/masa0902dev/nextjs-app-router-ts-pretiter-eslint-stylelint.git
cd nextjs-app-router-ts-pretiter-eslint-stylelint

npm install
```

### create environment without `git clone`
1. npx create-next-app@latest
2. copy and paste package.json, config files (prettier,eslint,stylelint,.vscode)
3. npm install (or, npm ci)

## npm Scripts

This project includes the following npm scripts:

1. **dev**: Starts the development server using Next.js with TurboPack on port 3001.

   ```bash
   echo 'this is test repo, using port 3001' && next dev --turbopack -p 3001
   ```

2. **build**: Checks the code formatting with Prettier, lints the styles with Stylelint, and builds the Next.js application.

   ```bash
   prettier --check . && stylelint --allow-empty-input "**/*.{css,scss}" && next build
   ```

3. **start**: Starts the production server for the Next.js application.

   ```bash
   next start
   ```

4. **format**: Formats the code using Prettier and echoes a completion message.

   ```bash
   prettier --write . && echo '\nPrettier Finished'
   ```

5. **lint:es**: Lints the JavaScript/TypeScript code using ESLint and automatically fixes issues.

   ```bash
   next lint --fix && echo '\nESLint Finished'
   ```

6. **lint:style**: Lints the styles using Stylelint and automatically fixes issues.

   ```bash
   stylelint --fix --allow-empty-input "**/*.{css,scss}" && echo 'StyleLint Finished'
   ```

7. **check**: Runs the format, ESLint, and Stylelint checks in sequence.

   ```bash
   npm run format && npm run lint:es && npm run lint:style
   ```

8. **build:local**: Similar to the build command, but formats the code before building.
   ```bash
   prettier --write . && stylelint --allow-empty-input "**/*.{css,scss}" && next build
   ```

