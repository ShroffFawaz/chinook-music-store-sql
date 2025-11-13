🚀 Project Overview

The Chinook dataset simulates a digital music store with tables for customers, artists, albums, tracks, invoices, and playlists.
The goal of this project is to extract business insights and demonstrate strong SQL querying ability.

This project includes:
⦁	Revenue analysis
⦁	Customer behavior and segmentation
⦁	Artist performance
⦁	Genre popularity
⦁	Monthly trends
⦁	Year-over-year (YoY) metrics
⦁	Playlist and track insights

All queries are written in SQL Server, but the logic is fully compatible with PostgreSQL (standard SQL features: JOINs, GROUP BY, window functions).

🔧 Tech Stack

⦁	SQL Server
⦁	Chinook Database
⦁	PostgreSQL-compatible query logic
⦁	Window functions, CTEs, subqueries, joins

📂 Folder Details
📁 schema/

Contains the structure of the Chinook database.

tables.sql

1.	Table definitions for:
⦁	Customers
⦁	Invoices
⦁	InvoiceLine
⦁	Tracks
⦁	Albums
⦁	Artists
⦁	Genres
⦁	Playlists

1.	Primary/Foreign keys
2.	Table relationships

indexes.sql

Indexes created for faster analytical queries, such as:
⦁	Index on Invoice.InvoiceDate
⦁	Index on Track.GenreId
⦁	Composite index on Customer.Country, Customer.CustomerId

These improve reporting performance significantly.

📁 data/
seed.sql

Sample dataset extracted from the Chinook schema to quickly run the queries.
Useful for recruiters or team leads who want to test and reproduce output.

migrations/

Contains any schema changes or updates created during development.
Example:
⦁	Renaming columns
⦁	Adding new indexes
⦁	Fixing data types

📁 queries/

This is the core of the project.
reports.sql

Contains all 10+ analytical queries, including:
1.	Top-Selling Genre by Revenue
2.	Top 5 Customers by Total Spend
3.	Monthly Revenue Trend
4.	Top Artists by Tracks Sold
5.	Revenue by Country (Excluding USA)
6.	Albums with Most Tracks
7.	Customer Purchase Segmentation
8.	Year-over-Year (YoY) Revenue Growth
9.	Unique Genres per Playlist
10.	Longest Tracks per Genre

Queries use:

⦁	INNER & LEFT JOIN
⦁	Aggregation (SUM, COUNT, MIN, MAX)
⦁	CASE statements
⦁	GROUP BY and HAVING
⦁	ORDER BY
⦁	Window functions (LAG, OVER)
⦁	CTEs (WHERE needed)

common.sql

Helpful utility queries for:
⦁	exploring tables
⦁	checking metadata
⦁	debugging relationships
⦁	quick SELECT queries

🧩 Project Summary
Title: Chinook Music Store Analytics – SQL Project

Problem:
The Chinook dataset stores music-store data across several related tables. Extracting revenue insights, customer patterns, and artist/genre performance requires complex SQL logic.

Solution:
I wrote analytical SQL queries involving joins, aggregations, window functions, and segmentation logic. These queries generate business insights such as monthly revenue trends, genre popularity, customer value, and playlist diversity.

Impact:
This project demonstrates strong SQL competency, the ability to analyze relational data end-to-end, and readiness to work with PostgreSQL-based analytics pipelines.
