# BookStoreApi
1. Create a web API with ASP.NET Core and MongoDB
2. Choose a directory on your development machine for storing the data. For example, C:\BooksData on Windows. Create the directory if it doesn't exist. The mongo Shell doesn't create new directories.  Console: mongod --dbpath <data_directory_path>
3. Open another command shell instance. Connect to the default test database by running the following command: mongosh
4. Run the following command in a command shell: use BookStore: Console: db.createCollection('Books')
5. Define a schema for the Books collection and insert two documents using the following command: db.Books.insertMany([{ "Name": "Design Patterns", "Price": 54.93, "Category": "Computers", "Author": "Ralph Johnson" }, { "Name": "Clean Code", "Price": 43.15, "Category": "Computers","Author": "Robert C. Martin" }])
6. View the documents in the database using the following command: db.Books.find().pretty()
