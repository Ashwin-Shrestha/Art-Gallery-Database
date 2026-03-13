# Art Gallery Database 🎨

A relational database system for managing an art gallery, built using Oracle SQL as a BSc university project.

## Overview

This project implements a fully normalised relational database for an art gallery management system. It covers the data modelling, schema design, and SQL implementation needed to manage artists, artworks, exhibitions, and sales within a gallery context.

## Features

- Relational schema covering core gallery entities
- Normalised table design (avoiding data redundancy)
- SQL queries for data retrieval and reporting
- Oracle database dump (`.dmp`) for full import

## Tech Stack

![Oracle SQL](https://img.shields.io/badge/Oracle-F80000?style=flat&logo=oracle&logoColor=white)

- **Database**: Oracle SQL
- **Format**: Oracle Data Pump export (`.dmp`)

## Database Schema

The system models the following core entities:

| Table | Description |
|---|---|
| Artists | Artist profiles and biographical info |
| Artworks | Individual pieces with medium, year, price |
| Exhibitions | Gallery shows and their dates |
| Sales | Transaction records linking buyers and artworks |
| Customers | Buyer contact and purchase history |

## How to Import

### Prerequisites
- Oracle Database (or Oracle XE for local use)
- Oracle Data Pump (`impdp`) utility

### Import the dump

```sql
-- Using Oracle Data Pump
impdp your_username/your_password \
  DIRECTORY=your_directory \
  DUMPFILE="20049390 Ashwin Shrestha.dmp" \
  LOGFILE=import.log
```

> Alternatively, open the `.dmp` file using **Oracle SQL Developer** via the import wizard.

## Academic Context

- **Degree**: BSc (Hons) Computing — Islington College (London Metropolitan University)
- **Type**: Individual coursework project
- **Focus**: Relational database design, normalisation, SQL

---

*Part of [Ashwin Shrestha's](https://github.com/Ashwin-Shrestha) academic portfolio.*
