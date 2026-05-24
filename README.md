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

<pre>
? Available Requirements:

❯ [<span style="color:#9333ea">1</span>] <span style="color:#9333ea"> Define portfolio layout </span>            [3]
  [2] Build showcase components            [3]
  [3] Implement navigation routing         [3]
  [4] Add content configuration            [2]
  [5] Style and interaction design         [3]
</pre>

`[x]` on the right represents the number of submission attempts remaining for a requirement.

- Each requirement starts with **3 submissions**
- A successful evaluation completes the requirement
- Failed evaluations decrease remaining attempts
- When attempts reach `0`, no further submissions are allowed

## Example evaluation result

```tsx
/*
|--------------------------------------------------------------------------
| BITASMBL EVALUATION
|--------------------------------------------------------------------------
| SCORE: 5/100
| STATUS: FAIL ✕
|
| INSIGHT:
| Missing semantic structure and responsive layout.
|  
|  SUGGESTIONS:
| - rename mainpage → MainPage (React component convention)
| 
| frontend/src/pages/MainPage.tsx
|--------------------------------------------------------------------------
*/

export default function mainpage() {
  return (
    <main className="max-w-4xl mx-auto p-4 md:grid md:gap-8">
      <nav className="flex justify-between items-center py-6">
        <Logo />

        <ul className="flex gap-4">
          <li>
            <a href="#work">My Work</a>
          </li>
        </ul>
      </nav>

      <section id="hero" className="min-h-[60vh] flex items-center">
        <h1 className="text-4xl font-bold">Hello world!</h1>
      </section>

      <footer className="mt-auto py-8 border-t text-sm opacity-60">
        <p>{new Date().getFullYear()} Evaluated by Bitasmbl</p>
      </footer>
    </main>
  );
}
```

## Learn More

For complete command references, workflow explanations, and additional documentation, visit:

👉 [Bitasmbl Documentation](https://bitasmbl.com/docs)
