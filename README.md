# Quickstart for Bitasmbl project (React)

## 1) Install Bitasmbl-CLI package

```bash
npm i bitasmbl-cli
```

## 2) Run bitasmbl command to set up the project

```bash
bitasmbl pull --repoUrl https://github.com/he1snber8/Bitasmbl-hallo-380_b88_329 --appId 329 --repoId 123
```

## 3) Enter into the main directory and start coding!

```bash
cd project-repo-123
```

## Customize requirements in a way you like

Bitasmbl organizes development into requirements (tasks). Each requirement describes a specific feature or implementation goal and can optionally define suggested file locations through a `paths` array.

The `paths` property acts as a mapping guideline, helping contributors understand where related code should live inside the project structure.

You can customize 'paths' mappings to fit your preferred architecture through `bitasmbl.json` file.

```json
{
  "requirement": "Implement authentication flow",
  "paths": ["**/src/features/auth/**", "**/src/components/auth/**"]
}
```

Examples:

- `src/features/auth/` → feature/business logic
- `src/components/auth/` → reusable UI components
- Multiple paths can be assigned to a single requirement
- Paths are recommendations and help maintain consistency across contributors

## Requirements

### 🛒 Implement cart management UI

Create React cart UI to add, remove, and update items with real-time price calculations.

## Requirement Evaluation

Bitasmbl includes a requirement evaluation workflow that lets contributors select a task and submit work for validation.

Run:

```bash
bitasmbl evaluate
```

Example output:

```console
? Available Requirements:

❯ [1] Define portfolio layout              [3]
  [2] Build showcase components            [3]
  [3] Implement navigation routing         [3]
  [4] Add content configuration            [2]
  [5] Style and interaction design         [3]
```

`[x]` on the right represents the number of submission attempts remaining for a requirement.

- Each requirement starts with **3 submissions**
- A successful evaluation completes the requirement
- Failed evaluations decrease remaining attempts
- When attempts reach `0`, no further submissions are allowed

## Example Component

```tsx
export default function App() {
  return <h1>Hello from Bitasmbl</h1>;
}
```

<details>
<summary>Available commands</summary>

```bash
dotnet build
dotnet test
dotnet watch run
```

</details>
