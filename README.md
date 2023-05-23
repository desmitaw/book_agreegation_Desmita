# book_agreegation_Desmita
class Book:
    def __init__(self, title, author, price):
        self.title = title
        self.author = author
        self.price = price

class Bookstore:
    def __init__(self, name):
        self.name = name
        self.books = []

    def add_book(self, book):
        self.books.append(book)

    def display_books(self):
        print(f"Daftar buku di {self.name}:")
        for book in self.books:
            print(f"Judul: {book.title}")
            print(f"Penulis: {book.author}")
            print(f"Harga: {book.price}")
            print("----------------------")


# Membuat objek Bookstore
bookstore = Bookstore("Toko Buku Griya")

# Membuat objek Book
book1 = Book("Machine Learning", "Dios Kurniawan", 76500)
book2 = Book("Otodidak Python", "Jubile Entreprise",88000)
book3 = Book("Dasar Pemrograman", "Wenty A", 69700)

# Menambahkan objek Book ke dalam objek Bookstore
bookstore.add_book(book1)
bookstore.add_book(book2)
bookstore.add_book(book3)

# Menampilkan daftar buku yang tersedia di toko
bookstore.display_books()


Penjelasan
Kelas Book memiliki atribut title, author, dan price, yang mewakili judul buku, penulis buku, dan harga buku secara berturut-turut. Metode __init__ digunakan untuk menginisialisasi atribut-atribut tersebut saat objek Book dibuat.

Kelas Bookstore memiliki atribut name yang merepresentasikan nama toko buku, dan atribut books yang merupakan daftar buku yang ada di toko tersebut. Metode __init__ digunakan untuk menginisialisasi atribut-atribut tersebut. Metode add_book digunakan untuk menambahkan objek Book ke dalam daftar books pada objek Bookstore. Metode display_books digunakan untuk menampilkan daftar buku yang tersedia di toko.
