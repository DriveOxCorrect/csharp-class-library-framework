# Csharp Class Library Framework

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:6A11CB,100:2575FC&height=220&section=header&text=Csharp%20Class%20Library%20Framework&fontSize=55&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Build%20Robust%20Reusable%20And%20Scalable%20Dotnet%20Libraries&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-5.0.0-2575FC?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-95.2K-6A11CB?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-00E676?style=for-the-badge&logo=opensourceinitiative&logoColor=white)
![Platform](https://img.shields.io/badge/platform-dotnet%208%20%7C%20netstandard-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)

</div>

---

## 🏗️ The Foundation Of Modern .NET Architecture

Every great .NET application—whether it's a high-frequency trading platform, an enterprise ERP, or a mobile game—is built on a solid foundation of reusable class libraries. However, designing a library that is easy to maintain, test, version, and distribute is an art form. **Csharp Class Library Framework** is a production-ready, opinionated template designed to eliminate the boilerplate and enforce best practices from day one.

This repository is not just a starting point; it is a complete architectural blueprint. It provides a structured solution template with pre-configured projects for the core library, unit tests, integration tests, benchmarks, and NuGet packaging. It enforces strict coding standards, dependency injection, and clean architecture principles, ensuring your code remains maintainable as it scales.

Whether you are a solo developer publishing open-source utilities or part of an enterprise team building internal SDKs, this framework saves you weeks of setup time. It includes continuous integration pipelines for GitHub Actions, automated semantic versioning, and a beautiful documentation site generated via DocFX.

<img width="491" height="431" alt="1616320355636" src="https://github.com/user-attachments/assets/11262109-c870-4e10-8f84-57a53b2e198b" />


---

## 🧱 The Anatomy Of A Perfect Library

We have structured the solution to follow the **Onion Architecture**, ensuring your business logic is isolated from external dependencies. Here is how the projects are organized:

### 1. The Core Domain (`MyLibrary.Core`)
This is the heart of your library. It contains the interfaces, domain models, and business logic. It has **zero external dependencies**, making it incredibly fast to test and easy to port. It defines the contracts that the rest of the application will implement.

### 2. The Infrastructure Layer (`MyLibrary.Infrastructure`)
This project contains the concrete implementations of the interfaces defined in the Core. For example, if your Core defines an `IEmailService`, the Infrastructure project contains the `SmtpEmailService`. This separation allows you to swap out implementations without touching the core logic.

### 3. The Testing Suite (`MyLibrary.Tests`)
We provide a comprehensive testing setup using **xUnit** and **Moq**. It includes unit tests for the core logic, integration tests for the infrastructure, and mutation tests using **Stryker.NET** to ensure your tests are actually catching bugs.

### 4. The Benchmark Suite (`MyLibrary.Benchmarks`)
Performance matters. This project uses **BenchmarkDotNet** to measure the execution time and memory allocation of your critical methods. It generates beautiful, statistically rigorous reports so you can prove your library is fast.

### 5. The NuGet Package (`MyLibrary.Package`)
We provide a pre-configured `.csproj` file with all the metadata required for NuGet publishing. It includes a custom icon, README embedding, and SourceLink support, ensuring your package looks professional on NuGet.org.

---

<div align="center">

### 🔗 Ready to build your library?

[![Get Framework](https://img.shields.io/badge/🏗️_GET_FRAMEWORK-6A11CB?style=for-the-badge&logoColor=white)](https://share.google/OuPRpELcn3qUs4ZN1)

</div>

---

## ⚙️ Automated DevOps Pipeline

We believe that deployment should be as simple as pushing code. The framework includes a fully configured GitHub Actions workflow.

| Stage | Description |
| :--- | :--- |
| **Build** | Restores dependencies and builds the solution in Release mode |
| **Test** | Runs all unit and integration tests with code coverage reporting |
| **Benchmark** | Runs performance benchmarks and detects regressions |
| **Package** | Automatically versions and packages the library as a `.nupkg` |
| **Publish** | Pushes the package to NuGet.org when a new tag is created |

---

## 🧠 Under The Hood: Why Source Generators?

This framework includes support for **C# Source Generators**. Source Generators are a compiler feature that allows you to inspect your code and generate additional C# files on the fly.

We use this to automatically generate boilerplate code. For example, if you decorate a class with `[AutoImplement]`, the source generator automatically creates the `INotifyPropertyChanged` implementation for all your properties. This eliminates hundreds of lines of tedious code while maintaining full compile-time safety. We also provide a template for creating your own source generators, allowing you to automate your own repetitive patterns.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-2575FC?style=for-the-badge&logoColor=white)](https://share.google/OuPRpELcn3qUs4ZN1)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![xUnit](https://img.shields.io/badge/xUnit-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![NuGet](https://img.shields.io/badge/NuGet-004880?style=flat-square&logo=nuget&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## 🤝 Community & Contributing

We believe that great libraries are built by communities, not individuals. If you have suggestions for improving the architecture, found a bug in the pipeline, or want to add support for a new testing framework, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-generator`).
3. **Commit** your changes (`git commit -m 'Add new source generator'`).
4. **Push** to the branch (`git push origin feature/new-generator`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your libraries, ask for help with NuGet publishing, and discuss the latest trends in .NET development.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@csharp-library.dev.

---

<div align="center">

### ⭐ If this framework accelerates your development, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-00E676?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username/csharp-class-library-framework)

---

### 🚀 Start building your library today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-512BD4?style=for-the-badge&logoColor=white)](https://share.google/OuPRpELcn3qUs4ZN1)

<sub>Crafted with precision and ❤️ by the Csharp Class Library Framework community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:2575FC,100:6A11CB&height=120&section=footer)

</div>
