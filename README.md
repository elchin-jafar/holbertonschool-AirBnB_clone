<h1 align="center">
<font face="Anta" size="25">AirBnB clone - The console</font>
</h1>

![GIF](./assets/563b97a87fa44cff9d001760.gif)

This project introduces a command-line interpreter (CLI) to manage AirBnB elements. It's the first step in creating a full web app replica of AirBnB. The CLI allows users to interact with different objects—users, states, cities, places, amenities, reviews—using simple commands.

<h2 align="center">AirBnB Clone Command Interpreter</h2>

To start the AirBnB Clone Command Interpreter, follow these steps:
1. Clone the repository from GitHub:
```
git clone https://github.com/zabitaguliyeva/holbertonschool-AirBnB_clone.git
```
2. Navigate to the project directory:
```
cd holbertonschool-AirBnB_clone
```
3. Run the command interpreter:
```
./console.py
```

<h2 align="center">How to Use the Command Interpreter</h2>

The command interpreter supports the following commands:

- `EOF`: Exit the command interpreter.
- `all`: Retrieve all objects from the storage.
- `create`: Create a new object.
- `destroy`: Delete an object.
- `help`: Display help information.
- `quit`: Exit the command interpreter.
- `show`: Display information about an object.
- `update`: Update an object.

The command interpreter supports the following objects:

- `Amenity`
- `BaseModel`
- `City`
- `Place`
- `Review`
- `State`
- `User`


<h3 align="center">Using the Console</h3>


To get help on a specific command, type `help <command>` in the command interpreter. For example:
```
(hbnb) help create
Create a new instance of a class.
Usage: create <class name>
```

To create a new object, type `create <object>` in the command interpreter. For example:
```
(hbnb) create User
4628b005-1a65-4402-ace3-4fff871e31aa
```

To display all objects, type `all` in the command interpreter. For example:
```
(hbnb) all
["[User] (4628b005-1a65-4402-ace3-4fff871e31aa) {'id': '4628b005-1a65-4402-ace3-4fff871e31aa', 'created_at': datetime.datetime(2024, 2, 28, 17, 31, 12, 823645), 'updated_at': datetime.datetime(2024, 2, 28, 17, 31, 12, 823908)}"]
```

To display all objects of a specific type, type `all <object>` in the command interpreter. For example:
```
(hbnb) all User
["[User] (4628b005-1a65-4402-ace3-4fff871e31aa) {'id': '4628b005-1a65-4402-ace3-4fff871e31aa', 'created_at': datetime.datetime(2024, 2, 28, 17, 31, 12, 823645), 'updated_at': datetime.datetime(2024, 2, 28, 17, 31, 12, 823908)}"]
```

To display information about an object, type `show <object> <id>` in the command interpreter. For example:
```
(hbnb) show User 4628b005-1a65-4402-ace3-4fff871e31aa
[User] (4628b005-1a65-4402-ace3-4fff871e31aa) {'id': '4628b005-1a65-4402-ace3-4fff871e31aa', 'created_at': datetime.datetime(2024, 2, 28, 17, 31, 12, 823645), 'updated_at': datetime.datetime(2024, 2, 28, 17, 31, 12, 823908)}
```

To update an object, type `update <object> <id> <attribute> <value>` in the command interpreter. For example:
```
(hbnb) update User 4628b005-1a65-4402-ace3-4fff871e31aa first_name "Betty"
```

To delete an object, type `destroy <object> <id>` in the command interpreter. For example:
```
(hbnb) destroy User 4628b005-1a65-4402-ace3-4fff871e31aa
```

To exit the command interpreter, type `quit` or `EOF` in the command interpreter. For example:
```
(hbnb) quit
```

To run the command interpreter in non-interactive mode, echo the command and pipe it into the command interpreter. For example:
```
echo "help" | ./console.py
```


<h2 align="center">Testing</h2>

Unit tests for the command interpreter are located in the [tests](./tests/) directory. To run the tests, navigate to the project directory and run the following command:

```
python3 -m unittest discover tests
```
