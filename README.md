# entri
Decorators and Exception Handling exercise no. 2
def read_file():
    file_name = input("Enter the file name: ")

    try:
        with open(file_name, 'r') as file:
            content = file.read()
            print("File content:\n", content)
    except FileNotFoundError:
        print(f"Error: The file '{file_name}' was not found.")

read_file()
