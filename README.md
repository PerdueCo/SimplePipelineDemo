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

```
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
```

---

# 🚀 1. Create the Project (Visual Studio 2022)

1. Open **Visual Studio 2022**  
2. Click **Create a new project**  
3. Search: **API** → select **ASP.NET Core Web API** → Next  
4. Configure:
   - **Project name:** `SimplePipelineDemo`
   - **Framework:** `.NET 8.0`
   - **Use Controllers:** ✔ Enabled  
   - **OpenAPI/Swagger:** ✔ Enabled  
5. Click **Create**

---

# 📂 2. Create Folders & Files

### Create folders
In **Solution Explorer**:

- Right-click the project → **Add → New Folder** → `Models`
- Add another folder → `Services`

### Remove sample template file (optional)
- Delete `WeatherForecastController.cs`

### Create the files below:

- `Models/Product.cs`
- `Services/IProductService.cs`
- `Services/ProductService.cs`
- `Controllers/ProductsController.cs`

---

# 🧩 3. Paste the Code (Complete Source Files)

## 📌 **Models/Product.cs**
```csharp
public class Product
{
    public int Id { get; set; }
    public string Name { get; set; } = string.Empty;
}
