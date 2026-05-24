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

<details>
<summary>Available commands</summary>

```bash
dotnet build
dotnet test
dotnet watch run
```

</details>
