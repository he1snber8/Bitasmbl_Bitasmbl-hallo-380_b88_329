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

## Environment

Create an `appsettings.Development.json` file:

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Database=bitasmbl;User Id=sa;Password=Your_password123;"
  }
}
```

## Project Structure

```txt
{{RepoName}}/
├── src/
├── tests/
├── README.md
└── .gitignore
```

## Quick Start

```bash
npm install
npm run dev
```

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
