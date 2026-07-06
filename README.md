# VisitVista CLI

VisitVista CLI is a simple command-line application built with Go for managing tourism destination data. It allows users to add, edit, delete, view, search, and sort tourism destination records through an interactive terminal menu.

This project was developed as an introductory programming project to practice fundamental programming concepts, especially data structuring, CRUD operations, searching, sorting, and terminal-based user interaction.

---

## ✨ Key Features

* **Add Destination Data:** Add new tourism destinations with details such as name, location, entrance fee, distance, rating, and description.
* **Edit Destination Data:** Update existing destination information based on its ID.
* **Delete Destination Data:** Remove tourism destination records from the list.
* **View Destination List:** Display all stored tourism destination data.
* **View Destination Description:** Show detailed descriptions of selected destinations.
* **Search Destinations:** Search tourism destinations by name, location, entrance fee range, distance range, or rating range.
* **Sort Destinations:** Sort tourism destinations by distance, entrance fee, or rating.
* **Interactive CLI Menu:** Navigate the application through a simple numbered terminal menu.

---

## 🛠️ Tech Stack

* **Programming Language:** Go
* **Interface:** Command-Line Interface
* **Data Storage:** In-memory storage using array and struct
* **Core Concepts:** CRUD, searching, sorting, loops, conditionals, functions, and structured data

---

## 📁 Project Structure

```txt
visit-vista-cli/
└── visitVista.go
```

The project is currently contained in a single Go file because it was created as a basic command-line application for learning purposes.

---

## 🚀 Getting Started

### Prerequisites

Make sure Go is installed on your machine.

Check your Go installation by running:

```bash
go version
```

### Installation

1. Clone the repository:

```bash
git clone https://github.com/Ahmadnhy/visit-vista-cli.git
```

2. Navigate to the project directory:

```bash
cd visit-vista-cli
```

3. Run the application:

```bash
go run visitVista.go
```

---

## 💻 Usage

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

Users can select a menu option by entering the corresponding number.

---

## 🧾 Data Fields

Each tourism destination contains the following data:

| Field     | Description                                 |
| --------- | ------------------------------------------- |
| ID        | Unique identifier for each destination      |
| Nama      | Name of the tourism destination             |
| Lokasi    | Location of the destination                 |
| Biaya     | Estimated entrance fee                      |
| Deskripsi | Short description of the destination        |
| Jarak     | Distance of the destination in kilometers   |
| Rating    | Destination rating on a scale of 1.0 to 5.0 |

---

## 🎯 Learning Objectives

Through this project, I practiced:

* Creating and using structs in Go
* Managing data with arrays
* Building reusable functions
* Handling user input from the terminal
* Implementing basic CRUD operations
* Searching data based on specific criteria
* Sorting data in ascending or descending order
* Structuring a simple terminal-based application

---

## ⚠️ Current Limitations

This project is still a beginner-level command-line application and has several limitations:

* Data is stored temporarily in memory and will reset when the program stops.
* The application does not use a database or file-based storage.
* Some input handling is still basic.
* Search functionality is case-sensitive.
* The project does not include automated testing yet.

---

## 🔮 Future Improvements

Possible improvements for future development include:

* Adding persistent data storage using files or a database
* Improving input validation
* Refactoring the code into smaller modules
* Adding case-insensitive search
* Adding unit tests for search and sorting functions
* Creating a web-based version of the application

---

## 📌 Project Status

This project is completed as a basic command-line application for learning and portfolio documentation purposes.

---

## 📄 License

This project is intended for educational and portfolio purposes.

---

Developed by Aisy Fadlillah (@aisyfadlillah)
