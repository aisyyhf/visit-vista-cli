# VisitVista

VisitVista is a Go-based CLI (Command Line Interface) application for managing tourist attraction ("tempat wisata") data. It allows users to add, edit, delete, view, and search tourist attraction data interactively through the terminal.

## Features

1. **Add Tourist Attraction** — Add a new tourist attraction record (name, location, cost, distance, rating, description).
2. **Edit Tourist Attraction** — Edit a specific attribute of an attraction by ID (name, location, cost, description, distance, or rating).
3. **Delete Tourist Attraction** — Delete an attraction by ID. IDs of the remaining data are automatically re-sequenced.
4. **View Tourist Attractions**
   - View the full list of attractions in a table format.
   - View the full description of a specific attraction by ID.
   - View the list sorted by **Distance**, **Cost**, or **Rating** (ascending/descending).
5. **Search Tourist Attractions** — Search by:
   - Name
   - Location
   - Cost range (5 categories)
   - Distance range (5 categories)
   - Rating range (4 categories)
6. **Exit** — End the program.

## Data Structure

Each tourist attraction is stored using the following struct:

```go
type TempatWisata struct {
    ID        int
    Nama      string
    Lokasi    string
    Biaya     int
    Deskripsi string
    Jarak     float64
    Rating    float64
}
```

Data is stored in a fixed-size static array with a maximum capacity of **100 records** (`NMAX = 100`), with no file persistence — all data is kept in memory only and is lost every time the program is closed.

## Requirements

- [Go](https://go.dev/dl/) version 1.16 or later installed on your system.

## How to Run

1. Save the code to a file, e.g. `main.go`.
2. Open a terminal in the directory containing the file.
3. Run one of the following commands:

   **Run directly without building:**
   ```bash
   go run main.go
   ```

   **Or build an executable first:**
   ```bash
   go build -o visitvista main.go
   ./visitvista
   ```

## Usage

Once running, the main menu will appear:

```
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

Select the menu number you need, then follow the on-screen input prompts. (Note: menu labels and prompts are in Indonesian, since that is the program's original language.)

### Example: Adding a New Record

```
Pilih Opsi: 1
Masukkan nama tempat wisata: Pantai Kuta
Masukkan lokasi tempat wisata: Bali
Masukkan biaya tempat wisata: 50000
Masukkan jarak tempat wisata (Dalam KM): 12.5
Masukkan rating tempat wisata (dalam skala 1.0 - 5.0): 4.5
Masukkan deskripsi tempat wisata: Pantai indah dengan sunset terbaik
Tempat wisata berhasil ditambahkan.
```

## Notes / Limitations

- Maximum data capacity is **100 tourist attractions**, since the program uses a static array instead of a dynamic slice.
- Data is **not persisted** (no file/database storage), so it will be lost when the program closes.
- Rating must be within the range of **1.0 – 5.0**; invalid input will be rejected and the add operation will be cancelled.
- Search by name/location uses **exact matching** (case-sensitive, must match exactly) and only reads a single word (uses `fmt.Scan`, so it does not support input containing spaces).
- After a record is deleted, the IDs of all remaining data are re-sequenced in order (1, 2, 3, ...).

## License

Free to use and modify for learning purposes or further development.
