# VisitVista CLI

VisitVista CLI is a simple command-line application built with Go for managing tourism destination data. The application allows users to add, edit, delete, view, search, and sort tourism destination records through an interactive terminal menu.

This project was created as an introductory programming project to practice basic data management logic, structured programming, and fundamental Go concepts.

## Project Overview

VisitVista CLI provides a basic tourism destination management system that runs directly in the terminal. Users can manage destination information such as name, location, entrance fee, distance, rating, and description.

The application stores data temporarily in memory using arrays and structs, without database integration. This makes the project suitable for understanding core programming concepts before moving into more advanced topics such as persistent storage, APIs, or web-based applications.

## Problem / Context

Tourism destination data often needs to be organized based on several criteria, such as location, entrance fee, distance, and rating. This project simulates a simple system that helps users manage and filter destination records through a command-line interface.

The main purpose of this project is to demonstrate basic CRUD operations, searching, sorting, input handling, and data structuring in Go.

## Features

* Add new tourism destination data
* Edit existing destination information
* Delete destination data by ID
* View all destination records
* View detailed destination descriptions
* Search destinations by:

  * Name
  * Location
  * Entrance fee range
  * Distance range
  * Rating range
* Sort destinations by:

  * Distance
  * Entrance fee
  * Rating
* Interactive terminal-based menu

## Tech Stack

* Go
* Command-Line Interface
* In-memory data storage using array and struct

## Installation and Setup

### Prerequisites

Make sure Go is installed on your machine.

You can check your Go installation by running:

```bash
go version
```

### Clone the Repository

```bash
git clone https://github.com/your-username/visit-vista-cli.git
```

### Navigate to the Project Directory

```bash
cd visit-vista-cli
```

### Run the Application

```bash
go run visitVista.go
```

## Usage

After running the application, the main menu will appear in the terminal.

```txt
----------------------------------------------------------------
                           VisitVista
----------------------------------------------------------------
1. Tambah Tempat Wisata
2. Edit Tempat Wisata
3. Hapus Tempat Wisata
4. Lihat Tempat Wisata
5. Cari Tempat Wisata
6. Keluar
----------------------------------------------------------------
Pilih Opsi:
```

Users can select a menu option by entering the corresponding number.

## Data Structure

Each tourism destination is represented using a struct with the following fields:

| Field     | Description                                 |
| --------- | ------------------------------------------- |
| ID        | Unique identifier for each destination      |
| Nama      | Name of the tourism destination             |
| Lokasi    | Location of the destination                 |
| Biaya     | Estimated entrance fee                      |
| Deskripsi | Short description of the destination        |
| Jarak     | Distance of the destination in kilometers   |
| Rating    | Destination rating on a scale of 1.0 to 5.0 |

## Folder Structure

```txt
visit-vista-cli/
└── visitVista.go
```

## Screenshots

Screenshots can be added to help users understand how the application works without running it first.

Recommended screenshots:

```txt
docs/screenshots/main-menu.png
docs/screenshots/add-destination.png
docs/screenshots/destination-list.png
docs/screenshots/search-result.png
```

Example README format after adding screenshots:

```md
### Main Menu

![Main Menu](docs/screenshots/main-menu.png)

### Destination List

![Destination List](docs/screenshots/destination-list.png)
```

## Demo Account

This project does not require a demo account because it is a command-line application without authentication.

## My Role

I developed this project as a basic Go programming exercise. My work included designing the command-line menu, creating the tourism destination data structure, implementing CRUD operations, and adding search and sorting features for destination records.

## Learning Objectives

Through this project, I practiced:

* Using structs and arrays in Go
* Creating reusable functions
* Handling user input from the terminal
* Implementing basic CRUD operations
* Searching data based on specific criteria
* Sorting data in ascending and descending order
* Structuring a simple terminal-based application

## Current Limitations

This project is still a beginner-level command-line application and has several limitations:

* Data is stored temporarily in memory and will reset when the program stops
* The application does not use a database or file storage
* Some input handling is still basic
* Search functionality is case-sensitive
* The project does not include automated testing yet

## Future Improvements

Possible improvements for future development include:

* Adding persistent data storage using files or a database
* Improving input validation
* Refactoring the code into smaller modules
* Adding case-insensitive search
* Adding unit tests for search and sorting functions
* Creating a web-based version of the application

## Project Status

This project is completed as a basic command-line application for learning and portfolio documentation purposes.

## License

This project is intended for educational and portfolio purposes.
