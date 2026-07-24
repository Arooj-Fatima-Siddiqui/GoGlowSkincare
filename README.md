

# GoGlow - Premium Natural Skincare Brand 🌿✨

**GoGlow** is a web-based skincare application developed as part of a **Visual Programming** course project. The system provides personalized, skin-type-based, and budget-friendly skincare solutions to customers with convenience and simplicity.

---

## 📌 Project Details

* **Project Title:** Skin Care Brand


* **Subject:** Visual Programming


* **Institute:** Air University Multan


* **Semester:** 3rd (BScs-A)


* **Instructor:** Faisal Idrees


* **Submission Date:** December 25, 2025


## ❓ Problem Statement & Motivation

Most mass-market skincare products are not one-size-fits-all, leading to skin issues and wasted money when consumers purchase unsuitable formulations. **GoGlow** solves this problem by offering customized, affordable skincare recommendations tailored directly to the user’s specific skin type and budget.

---

## 🌟 Key Features

* 🛍️ **Interactive Product Showcase:** Browse products with high-quality images and short instructional videos.


* 🛒 **Dynamic Shopping Cart:** Add/remove items, adjust quantities, and calculate sub-totals instantly.


* 👤 **Customer Auto-Fill:** Remembers returning customers to speed up future checkouts.


* 📦 **Real-Time Stock Management:** Automatically disables "Out of Stock" items to prevent invalid orders.


* 🚚 **Order Processing:** Checkout form validation with immediate confirmation and estimated delivery dates.


* ✉️ **Contact & Support:** Easy-to-use communication channels directly with store operators.

## 🛠️ Tech Stack & Architecture

* **Architecture:** ASP.NET Core MVC (Model-View-Controller)


* **Backend:** C# / ASP.NET Core


* **Frontend:** HTML, CSS, Bootstrap 5, JavaScript, jQuery


* **Database:** SQL Server


* **ORM:** Entity Framework Core


* **Security & Session Management:** Server-side validation, Anti-Forgery Tokens, and HTTP-only session cookies.


## 🗄️ Database Models Overview

The backend uses Entity Framework Core with primary models:

### 1. `Product` Model

```csharp
public class Product 
{
    public int Id { get; set; }
    public string Name { get; set; }
    public string Description { get; set; }
    public decimal Price { get; set; }
    public string ImageUrl { get; set; }
    public string Category { get; set; }
    public int StockQuantity { get; set; }
}

```

### 2. `CartItem` Model

```csharp
public class CartItem 
{
    public int Id { get; set; }
    public Product Product { get; set; }
    public int Quantity { get; set; }
}

```

### 3. `CartViewModel` Structure

Calculates real-time order totals, fixed shipping charges, and estimates standard 3-day deliveries.

---

## 🚀 Getting Started

### Prerequisites

* [.NET SDK (6.0 or higher)](https://dotnet.microsoft.com/download)
* [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
* Visual Studio 2022 or VS Code

### Installation & Run Instructions

1. **Clone the repository:**
```bash
git clone https://github.com/243512/GoGlowSkincare.git
cd GoGlowSkincare

```

2. **Configure Database Connection:**
Update your database connection string inside `appsettings.json`.
3. **Apply Database Migrations:**
```bash
dotnet ef database update

4. **Run the Application:**
```bash
dotnet run


## 🔮 Future Enhancements

* 🤖 AI-based skin type analysis engine


* 💬 Live consultation chat with skin care specialists


* 💳 Integrated online payment gateways


* 📊 Comprehensive Admin Dashboard for order/inventory tracking


* 📱 Native Mobile Application
