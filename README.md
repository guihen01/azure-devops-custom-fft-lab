# Azure DevOps CI/CD Pipeline for a Custom C# FFT NuGet Package

This project demonstrates a complete Azure DevOps CI/CD pipeline for a .NET 8 C# console application using a custom FFT NuGet package published on NuGet.org.

The application uses the custom package `FFTlib` to perform FFT / DFT / DSP signal processing operations.

---

## Technologies

- C#
- .NET 8
- Azure DevOps
- YAML Pipelines
- GitHub
- NuGet
- FFTlib

---

## Features

- Custom FFT NuGet package consumption
- Automated Azure DevOps pipeline
- GitHub integration
- Build automation
- Artifact publishing
- Signal processing application

---

## Pipeline Workflow

```text
GitHub
   ↓
Azure DevOps Pipeline
   ↓
dotnet restore
   ↓
Download FFTlib from NuGet
   ↓
dotnet build
   ↓
dotnet publish
   ↓
Published Artifact
```

---

## Project Structure

```text
azure-devops-custom-fft-lab/
│
├── src/
│   └── CustomFFTConsoleApp/
│
├── azure-pipelines.yml
└── README.md
```

---

## Run Locally

```bash
dotnet build
dotnet run --project src/CustomFFTConsoleApp
```

---

## NuGet Package

FFTlib package:

https://www.nuget.org/packages/FFTlib/

---

## GitHub Repository

Math-FFT-Lib repository:

https://github.com/guihen01/Math-FFT-Lib

---

## Azure DevOps Pipeline

The pipeline automatically:

- restores NuGet packages
- builds the application
- publishes build artifacts

---

## Future Improvements

- Docker support
- Azure Container Registry (ACR)
- Azure Container Apps deployment
- Terraform integration
