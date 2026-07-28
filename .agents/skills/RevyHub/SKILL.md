```markdown
# RevyHub Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the core development patterns and conventions used in the RevyHub TypeScript codebase. You'll learn how to structure files, write imports and exports, follow commit message conventions, and implement and test features in a consistent, maintainable way.

## Coding Conventions

### File Naming
- **PascalCase** is used for all file names.
  - Example: `UserProfile.ts`, `AuthService.ts`

### Import Style
- **Alias imports** are preferred.
  - Example:
    ```typescript
    import UserService from '@services/UserService';
    ```

### Export Style
- **Default exports** are used for modules.
  - Example:
    ```typescript
    export default UserProfile;
    ```

### Commit Messages
- **Conventional Commits** with the `feat` prefix are used.
  - Example:
    ```
    feat: add user authentication to login page
    ```

## Workflows

### Feature Development
**Trigger:** When adding a new feature  
**Command:** `/feature-development`

1. Create a new file using PascalCase (e.g., `NewFeature.ts`).
2. Implement the feature logic.
3. Use alias imports for dependencies.
    ```typescript
    import Helper from '@utils/Helper';
    ```
4. Export the main component or function as default.
    ```typescript
    export default NewFeature;
    ```
5. Write a test file named `NewFeature.test.ts`.
6. Commit changes using a conventional commit message:
    ```
    feat: add new feature for [description]
    ```

### Testing
**Trigger:** When writing or running tests  
**Command:** `/run-tests`

1. Create test files with the pattern `*.test.ts` (e.g., `UserProfile.test.ts`).
2. Write tests for your feature or module.
3. Run tests using your preferred test runner (framework is unspecified; check project documentation or use a standard TypeScript-compatible runner).

## Testing Patterns

- **Test File Naming:** Use the pattern `*.test.ts` for test files.
  - Example: `AuthService.test.ts`
- **Test Framework:** Not explicitly specified; use a standard TypeScript test framework (e.g., Jest, Mocha) if not otherwise instructed.
- **Test Structure:** Place tests alongside or near the modules they test.

## Commands

| Command              | Purpose                                      |
|----------------------|----------------------------------------------|
| /feature-development | Guide for adding a new feature               |
| /run-tests           | Steps for writing and running tests          |
```
