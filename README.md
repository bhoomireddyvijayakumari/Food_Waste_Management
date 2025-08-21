# Food_Waste_Management

# Project Overview

This project implements a comprehensive Local Food Wastage Management System that connects food providers with receivers to reduce food waste. The system includes database management, analytics, and a user-friendly web interface.

# Implementation Steps

1. Environment Setup and Database Configuration

- Mounted Google Drive for data storage and access

- Installed and configured MySQL server with proper authentication

- Established database connection with Python using mysql-connector

- Created a dedicated database (foodwaste_db) for the project
  
2. Database Schema Design

- Designed four main tables with proper relationships:

providers: Stores information about food donors (restaurants/individuals)

receivers: Contains details of NGOs/individuals receiving food

food_listings: Main table tracking available food items with status management

claims: Records transactions between providers and receivers

- Implemented foreign key constraints and cascading updates for data integrity

- Used ENUM types for status fields to ensure data consistency

3. Data Loading and Processing

- Loaded four CSV files containing sample data for all entities

- Implemented data normalization functions to handle column naming inconsistencies

- Created robust date parsing functions to handle various date formats

- Built specialized loading functions for each table with duplicate handling

- Ensured proper data type conversion and error handling during import

4. Analytical Query Development

Designed and executed 15 comprehensive SQL queries for business intelligence:

- Geographic analysis of providers and receivers

- Quantity and type-based food analysis

- Claim status and efficiency metrics

- Temporal analysis of expiration patterns

- Provider and receiver performance metrics

- Generated automated reports for key insights including:

- Wastage by food type and city

- Soon-to-expire items (7-day window)

- Supply-demand analysis by location

- Monthly trends of expired vs completed claims

5. Streamlit Application Development

- Built a multi-tab web application with comprehensive functionality:

- Browse & Contact Tab: Filterable food listing display with direct contact options

- CRUD Operations Tab: Full create, read, update, delete functionality for all entities

- Analytics Tab: Display of all 15 analytical queries with export capabilities

- Data Insights Tab: Visualizations of key trends using Plotly charts

- Implemented smart contact linking (email, phone, WhatsApp) based on contact data

- Added comprehensive form validation and user feedback mechanisms

- Designed responsive layout with sidebar filters for enhanced user experience

6. Deployment Preparation

- Configured ngrok tunneling for public access to the Streamlit application

- Set up proper error handling and warning suppression

- Ensured cross-platform compatibility and dependency management


# Technical Achievements

- Successfully integrated MySQL database with Python and Streamlit

- Implemented a complete CRUD system with relational integrity

- Developed comprehensive analytical capabilities with both tabular and visual outputs

- Created a production-ready web application with professional UI/UX

- Established automated reporting system for ongoing monitoring

The project demonstrates a full-stack solution to food waste management, combining database management, analytics, and web application development into a cohesive system that can effectively connect food donors with recipients while providing valuable insights for optimization.
