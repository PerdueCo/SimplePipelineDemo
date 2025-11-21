# SimplePipelineDemo  
A clean, beginner-friendly demonstration of how an ASP.NET Core Web API request travels through the **middleware pipeline** — from the moment a GET request arrives until JSON is returned.

This project includes:
- ✔ Simple `/api/products/{id}` endpoint  
- ✔ Custom service layer (`IProductService`)  
- ✔ The full ASP.NET Core request pipeline  
- ✔ Docker support (Dockerfile included)  
- ✔ GitHub Actions CI workflow  
- ✔ Diagram explaining the request flow  

---

## 📌 Project Purpose
Use this project to demonstrate your understanding of:
- How the ASP.NET Core middleware pipeline works  
- Routing, controllers, and model binding  
- Dependency injection  
- Service layers  
- JSON serialization  
- Dockerized Web APIs  
- GitHub Actions CI pipelines  

---

## 📁 Project Structure
SimplePipelineDemo/
├── Controllers/
│ └── ProductsController.cs
├── Services/
│ ├── IProductService.cs
│ └── ProductService.cs
├── Models/
│ └── Product.cs
├── Program.cs
├── Dockerfile
├── README.md
└── .github/workflows/ci.yml
---
SimplePipelineDemo/
├── Controllers/
│ └── ProductsController.cs
├── Services/
│ ├── IProductService.cs
│ └── ProductService.cs
├── Models/
│ └── Product.cs
├── Program.cs
├── Dockerfile
├── README.md
└── .github/workflows/ci.yml
---
