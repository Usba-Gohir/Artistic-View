# ArtisticView: Art Gallery Database Management System

ArtisticView is a comprehensive database management system for art galleries and convention centers, designed to support the organization, retrieval, and management of various gallery-related data. This project centralizes data related to artwork, artists, events, employees, and attendees, making it an essential tool for art galleries and community centers.

## Project Overview

ArtisticView enables efficient management of an art gallery's inventory, events, ticket sales, and purchases by organizing data into key tables and establishing relationships between them. It is optimized for ease of use and scalability, providing functionalities that allow users to add, update, and delete records while ensuring data integrity through normalization up to 3NF/BCNF standards.

## Features

1. **Artwork Management**: Add, update, or remove artwork details, track artwork sales, and manage artist information.
2. **Event Scheduling**: Organize and track art exhibitions, workshops, and other gallery events. Event capacity and ticket pricing can also be managed efficiently.
3. **Sales and Ticketing**: Manage ticket sales and purchases, keeping a detailed record of visitors, ticket numbers, and purchase dates.
4. **Customer and Collector Profiles**: Maintain customer profiles and collector details, enabling efficient record-keeping of purchases and preferences.
5. **Views and Queries**: The database includes pre-defined views and sample queries for retrieving high-value artworks, upcoming events, artist portfolios, and much more.

## Database Schema

### Key Entities and Relationships

- **Artist**: Stores artist profiles, including name, birth date, and nationality.
- **Artwork**: Contains information about each artwork, including title, creation year, medium, dimensions, genre, and price.
- **Event**: Manages events and exhibitions, specifying genres, dates, ticket prices, and visitor capacity.
- **Ticket Sales**: Records ticket purchases with customer details, linked to specific events.
- **Artwork Purchase**: Tracks artwork sales with details on buyer information, bid amount, and purchase date.

### Relationships

- **Artist-Artwork**: Links artists to their respective artworks.
- **Artwork-Event**: Associates artworks with the events in which they are displayed.
- **Event-Ticket**: Connects events to ticket sales, maintaining visitor attendance records.

## Normalization

All tables in this database are normalized to 3NF/BCNF to ensure data integrity and eliminate redundancy:
- **3NF**: All non-key attributes are functionally dependent on the primary key.
- **BCNF**: Each table is decomposed to remove partial and transitive dependencies where necessary.

## SQL Scripts

The project includes the following SQL scripts:

- **Table Creation**: Scripts to create tables for `Artist`, `Artwork`, `Event`, `Ticket Sales`, and other relevant entities.
- **Data Insertion**: Scripts for populating tables with sample data.
- **Sample Queries**: Includes queries to retrieve information such as top-priced artworks, events per genre, average ticket prices, etc.
- **Views**: Pre-defined views to simplify data retrieval, including `ExpensiveArtworks`, `UpcomingEventDates`, and `ArtistTotalValue`.

## Requirements

- A relational database management system (e.g., MySQL, PostgreSQL, or Oracle)
- Basic knowledge of SQL for executing and modifying queries

## Authors

- Usba Gohir
- Yusra Farooqi
