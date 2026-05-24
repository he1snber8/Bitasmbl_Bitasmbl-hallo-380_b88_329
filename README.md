# Bitasmbl Project

<p align="center">
  <img src="https://img.shields.io/badge/.NET-8.0-blue" />
  <img src="https://img.shields.io/badge/status-generated-success" />
</p>

## Quick Start

```bash
git clone {{RepoUrl}}
cd {{RepoName}}
dotnet restore
dotnet run
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
