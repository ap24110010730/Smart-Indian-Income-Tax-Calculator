# Smart Indian Income Tax Calculator

## Project Overview

The **Smart Indian Income Tax Calculator** is a Java Swing-based desktop application developed to simplify income tax calculation and taxpayer record management.

The application calculates estimated tax liability under both the Old and New Tax Regimes, compares the results, and recommends the regime with the lower estimated tax payable. It uses MySQL for storing taxpayer information and calculation history.

## Key Features

- **Tax Calculation:** Calculates estimated income tax under Old and New Tax Regimes.
- **Tax Regime Comparison:** Compares tax payable under both regimes and recommends the lower-tax option.
- **Taxpayer Management:** Supports Create, Read, Update and Delete (CRUD) operations.
- **Income and Deduction Details:** Accepts salary, house property, business income, capital gains, other income and deduction inputs.
- **Calculation History:** Stores and retrieves previous tax calculations.
- **PDF Report Generation:** Generates downloadable tax calculation summaries.
- **CSV Export:** Exports tax comparison information in CSV format.
- **Input Validation:** Checks user inputs to reduce invalid entries.
- **Dashboard:** Displays taxpayer statistics, completed calculations and financial summaries.

## Technologies Used

| Technology | Purpose |
|---|---|
| Java | Application development |
| Java Swing | Graphical user interface |
| MySQL | Database management |
| JDBC | Database connectivity |
| Apache Maven | Project build and dependency management |
| FlatLaf | Modern Swing interface styling |
| OpenPDF | PDF report generation |
| JUnit 5 | Unit testing |

## Project Structure

```text
Smart Indian Income Tax Calculator/
│
├── database/
│   └── schema.sql
│
├── reports/
│
├── src/
│   ├── main/
│   │   └── java/com/smarttax/
│   │       ├── config/
│   │       ├── dao/
│   │       ├── model/
│   │       ├── service/
│   │       ├── ui/
│   │       ├── util/
│   │       └── Main.java
│   │
│   └── test/
│
├── .mvn/
├── .env.example
├── .gitignore
├── mvnw
├── mvnw.cmd
├── pom.xml
└── README.md
```

## Requirements

- Java Development Kit (JDK)
- MySQL Server
- Visual Studio Code or another Java IDE
- Maven (the project includes Maven Wrapper)

## Database Setup

1. Install and start MySQL Server.
2. Open MySQL Workbench or the MySQL command line.
3. Execute the SQL script available at `database/schema.sql`.
4. Create the database connection using your local MySQL credentials.
5. Configure the database username and password using the environment variables expected by `DatabaseConnection.java`.

**Security Note:** Do not upload actual database passwords or private credentials to GitHub.

## How to Run the Project

Open PowerShell in the project directory.

### Step 1: Compile the project

```powershell
.\mvnw.cmd clean compile
```

### Step 2: Run the application

```powershell
.\mvnw.cmd exec:java
```

The Smart Indian Income Tax Calculator desktop application will launch.

## Testing

The project includes JUnit 5 test cases for testing tax calculation functionality.

Run the tests using:

```powershell
.\mvnw.cmd test
```

## Project Team

| S. No. | Team Member |
|---|---|
| 1 | Uddaraju Pavan Varma |
| 2 | Kodipalli Venu Madhav |
| 3 | Kosaraju Sai Subash Raja |
| 4 | Medarametla Khushwanth |
| 5 | Madhyanapu Shreyank Gautam |

All five members contributed to the development, implementation, testing, integration and documentation of the project.

## Project Deliverables

- Java source code and database schema.
- Project documentation and final report.
- Project presentation.
- Application demonstration video.

## Limitations

The application provides estimated tax calculations for academic demonstration purposes. Certain special tax treatments, including capital gains tax rates and surcharge calculations for higher incomes, may not be fully supported. Users should verify actual tax liability with official Income Tax Department guidance or a qualified tax professional.

## Disclaimer

This project is developed for educational purposes. The calculated tax amounts are estimates and should not be considered professional tax or financial advice.

---

**Project:** Smart Indian Income Tax Calculator  
**Platform:** Java Swing Desktop Application  
**Database:** MySQL  
**Academic Year:** 2026–2027
