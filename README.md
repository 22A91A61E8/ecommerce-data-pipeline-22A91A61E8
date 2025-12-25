# E-Commerce Data Pipeline Project

**Student:** Divya Eeli  
**Roll Number:** 22A91A61E8  
**Submission Date:** December 27, 2025

## 📋 Project Overview

End-to-End ETL Pipeline for E-Commerce Analytics Platform - A production-ready data engineering solution demonstrating:
- Three-tier database architecture (staging, production, warehouse)
- Automated ETL/ELT workflows
- Data quality assurance and monitoring
- Business Intelligence dashboards
- Docker containerization and CI/CD

## 🏗️ Architecture

### Database Design
- **Staging Schema**: Raw data ingestion with minimal constraints
- **Production Schema**: Normalized (3NF) with full constraints and indexes
- **Warehouse Schema**: Star schema with SCD Type 2 for dimensional modeling

### Tech Stack
- **Data Generation**: Python (Faker library)
- **Database**: PostgreSQL 14
- **ETL**: Python (Pandas, SQLAlchemy)
- **Orchestration**: Apache Airflow / Cron
- **BI Tool**: Tableau Public / Power BI Desktop
- **Containerization**: Docker & Docker Compose
- **CI/CD**: GitHub Actions
- **Testing**: Pytest (>80% coverage)

## 📊 Data Specifications

- **Customers**: 1,000 records
- **Products**: 500 records
- **Transactions**: 10,000 records
- **Transaction Items**: 15,000-25,000 records
- **Referential Integrity**: 100% (zero orphan records)

## 🚀 Quick Start

### Prerequisites
```bash
Python 3.8+
PostgreSQL 12+
Docker & Docker Compose
Git
```

### Installation

1. Clone the repository
```bash
git clone https://github.com/22A91A61E8/ecommerce-data-pipeline-22A91A61E8.git
cd ecommerce-data-pipeline-22A91A61E8
```

2. Set up environment
```bash
cp .env.example .env
# Edit .env with your database credentials
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Run with Docker (Recommended)
```bash
docker-compose up -d
```

5. Or run locally
```bash
bash setup.sh
python scripts/main.py
```

## 📁 Project Structure

```
ecommerce-data-pipeline/
├── data/
│   ├── raw/                 # Generated CSV files
│   ├── staging/             # Intermediate processed data
│   └── processed/           # Final clean data & reports
├── scripts/
│   ├── data_generation/     # Data generation scripts
│   ├── ingestion/           # Data ingestion to staging
│   ├── transformation/      # ETL transformations
│   └── quality_checks/      # Data quality validation
├── sql/
│   ├── ddl/                 # Schema creation scripts
│   ├── dml/                 # Data manipulation
│   └── queries/             # Analytical queries
├── dashboards/              # BI dashboards & screenshots
├── docker/                  # Docker configuration
├── tests/                   # Unit & integration tests
├── docs/                    # Documentation
├── config/                  # Configuration files
├── .github/workflows/       # CI/CD pipelines
└── logs/                    # Application logs
```

## 🔄 Pipeline Workflow

1. **Data Generation**: Generate realistic e-commerce data
2. **Staging Load**: Bulk load raw data to staging schema
3. **Data Quality**: Validate completeness, uniqueness, consistency
4. **Transformation**: Cleanse and apply business rules
5. **Production Load**: Load to normalized production schema
6. **Warehouse Load**: Build dimensional model with SCD Type 2
7. **Analytics**: Create aggregates and run analytical queries
8. **Dashboard**: Visualize insights in BI tool

## 🎯 Key Features

- ✅ 100% referential integrity
- ✅ Idempotent pipeline execution
- ✅ Comprehensive data quality framework
- ✅ SCD Type 2 implementation
- ✅ Automated testing (>80% coverage)
- ✅ Docker containerization
- ✅ CI/CD pipeline
- ✅ Detailed documentation

## 📈 Dashboard

[Link to Tableau Public Dashboard / Power BI Screenshots]

- **Page 1**: Executive KPIs & Sales Overview
- **Page 2**: Product Performance Analysis
- **Page 3**: Customer Segmentation
- **Page 4**: Geographic Distribution

## 🧪 Testing

Run tests with coverage:
```bash
pytest --cov=scripts --cov-report=html
```

## 📝 Documentation

- [Architecture Documentation](docs/architecture.md)
- [Dashboard Guide](docs/dashboard_guide.md)
- [API Documentation](docs/api_documentation.md)
- [SUBMISSION.md](SUBMISSION.md)

## 🔐 Configuration

Key configuration in `config/config.yaml`:
- Database connection parameters
- Data generation settings
- Pipeline batch sizes
- Logging levels

## 📊 Project Statistics

- **Lines of Code**: TBD
- **Test Coverage**: >80%
- **Data Records Processed**: 30,000+
- **Execution Time**: ~5 minutes

## 🤝 Contributing

This is a student project for academic evaluation.

## 📄 License

MIT License

## 📧 Contact

Divya Eeli - 22A91A61E8

---
**Note**: This project is part of the Global Placement Program - Data Engineering Track
