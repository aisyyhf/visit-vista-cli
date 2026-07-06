# VisitVista CLI

VisitVista CLI is a command-line application built with Go for managing tourism destination data. The application allows users to add, edit, delete, view, search, and sort tourism destination records through an interactive terminal menu.

This project was developed to practice fundamental programming concepts in Go, including structured data, CRUD operations, searching, sorting, function decomposition, and terminal-based user interaction.

---

## Key Features

* Add new tourism destination data with name, location, entrance fee, distance, rating, and description.
* Edit existing destination information based on its ID.
* Delete tourism destination records from the list.
* View all stored tourism destinations in a formatted table.
* View detailed descriptions of selected destinations.
* Search destinations by name, location, entrance fee range, distance range, or rating range.
* Sort destinations by distance, entrance fee, or rating in ascending or descending order.
* Navigate the application through an interactive numbered CLI menu.

---

## Tech Stack

* Programming Language: Go
* Interface: Command-Line Interface
* Data Storage: In-memory storage using arrays and structs
* Core Concepts: CRUD, searching, sorting, loops, conditionals, functions, and structured data

---

## Project Structure

```txt
visit-vista-cli/
├── README.md
└── visitVista.go
```

The project is currently contained in a single Go source file because it focuses on fundamental command-line application logic and basic data management implementation.

---

## Getting Started

### Prerequisites

Make sure Go is installed on your machine.

Check your Go installation by running:

```bash
go version
```

### Installation

Clone the repository:

```bash
git clone https://github.com/aisyyhf/visit-vista-cli.git
```

Navigate to the project directory:

```bash
cd visit-vista-cli
```

Run the application:

```bash
go run visitVista.go
```

---

## Usage

After running the application, the main menu will appear in the terminal:

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

Users can select a menu option by entering the corresponding number. Each option will guide the user through the required input, such as destination name, location, entrance fee, distance, rating, or description.

---

## Data Fields

Each tourism destination contains the following data:

| Field     | Description                               |
| --------- | ----------------------------------------- |
| ID        | Unique identifier for each destination    |
| Nama      | Name of the tourism destination           |
| Lokasi    | Location of the destination               |
| Biaya     | Estimated entrance fee                    |
| Deskripsi | Short description of the destination      |
| Jarak     | Distance of the destination in kilometers |
| Rating    | Destination rating on a scale of 1.0–5.0  |

---

## Implementation Notes

This project applies several basic programming concepts:

* Structs are used to represent tourism destination data.
* Arrays are used as temporary in-memory storage.
* Linear search is used to find destination data by ID.
* Sorting is implemented manually using nested loops.
* Each main operation is separated into different functions to keep the program easier to read and maintain.

---

## Current Limitations

This project focuses on fundamental programming concepts and currently has several limitations:

* Data is stored temporarily in memory and will reset when the program stops.
* The application does not use a database or file-based storage.
* Some input handling and validation can still be improved.
* Search by name and location is still case-sensitive and requires exact input.
* The project does not include automated testing yet.

---

## Future Improvements

Possible improvements for future development include:

* Add persistent data storage using files or a database.
* Improve input validation for numeric and text input.
* Refactor the code into smaller modules.
* Add case-insensitive and partial keyword search.
* Add unit tests for search and sorting functions.
* Create a web-based version of the application.

---

## Project Status

This project is intended for learning and portfolio documentation purposes.

---

Developed by Aisy Fadlillah (@aisyyhf)
