# Product Experimentation Analytics Pipeline

## What This Project Does

This pipeline automates how product experiment data gets 
cleaned, structured, and prepared for analysis. Instead 
of manually cleaning raw event data every time a new 
experiment runs, this pipeline handles it automatically 
using dbt and BigQuery — so analysts can focus on 
insights, not data wrangling.

## The Problem It Solves

Product teams run A/B tests to decide what features to 
ship. But raw experiment event data from warehouses is 
messy — duplicate records, inconsistent formats, missing 
values. Without a reliable data pipeline, experiment 
results can't be trusted. This project builds that 
reliable foundation.

## Tech Stack

- Google BigQuery — cloud data warehouse for storing 
  and querying experiment data
- dbt Cloud — transforms raw data into clean, 
  analysis-ready models
- SQL — business logic, aggregations, data cleaning
- GitHub — version control with branch-based 
  development workflow

## Project Structure

analyses/     → ad-hoc SQL queries for experiment insights  
macros/       → reusable dbt SQL functions  
models/       → core staging and transformation models  
seeds/        → static reference data  
snapshots/    → slowly changing dimension tracking  
tests/        → automated data quality checks  

## What I Built

**Milestone 1 — Environment Setup**  
Connected dbt Cloud to Google BigQuery and configured 
the project structure with separate development and 
production environments.

**Milestone 2 — Staging Models**  
Built SQL models that take raw product experiment 
event data and clean it — removing duplicates, 
standardizing formats, and applying business logic 
for downstream analysis.

**Milestone 3 — Automated Testing**  
Added dbt tests to automatically check data quality 
before any model goes to production. This ensures 
experiment data is always reliable when analysts 
query it.

## Key Skills Demonstrated

- Building modular, reusable SQL transformation models
- Writing automated data quality tests
- Managing a Git workflow with branches and 
  pull requests
- Working with modern data stack tools used in 
  production at real companies

## Why This Matters for Product Analytics

Clean, reliable experiment data is the foundation 
of every product decision. This pipeline is the 
layer that makes A/B test analysis trustworthy — 
without it, teams are making product decisions 
on bad data.

## Status

Active portfolio project. Currently expanding 
models to include automated statistical significance 
calculations for experiment results.
