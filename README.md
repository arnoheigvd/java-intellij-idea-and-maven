# CLI Application with Picocli

This project is a simple Command Line Interface (CLI) application built using the [Picocli](https://picocli.info/) library. The application has two subcommands (`hello` and `goodbye`) that demonstrate how to use Picocli to create a CLI with subcommands.

## Features

- **hello**: Prints a greeting message.
- **goodbye**: Prints a farewell message.
- You can pass options such as `--greetings` and `--farewells` to customize the messages.
- Default values are used when no name or message is provided.

## Structure

The project consists of the following key files:

- `Main.java`: The main class that handles command-line parsing and execution.
- `Hello.java`: A subcommand that prints a greeting message.
- `Goodbye.java`: A subcommand that prints a farewell message.

## Prerequisites

Make sure you have the following installed:

- **Java JDK 11+**
- **Maven** (for building the project)

## Build Instructions

1. **Clone the repository:**

   ```
   git clone <repository-url>
   cd <project-directory>
   ```

2. **Build the project using Maven:**
   ```
    mvn clean package
   ```
   This will generate a JAR file in the target directory.

3. **Running the Application**

   Once the project is built, you can run the application from the command line.
   Run the JAR

   ```
   java -jar target/<project-name>.jar [subcommand] [options]
   ```

4. **Example Usage**

    Print a greeting:
    ```
   java -jar target/myapp.jar hello
   ```
   Output: ```Hello World!```  

   Customize the greeting message:
   ```
   java -jar target/myapp.jar hello --greetings "Hi"
   ```
   Output: ``` Hi World! ```
  
   Say goodbye:
   ```
   java -jar target/myapp.jar goodbye
   ```
   Output: ``` Goodbye World! ```

   Customize the farewell message:
   ```
   java -jar target/myapp.jar goodbye --farewells "Farewell"
   ```
   Output: ``` Farewell World! ```

5. **Help and Version Information**

   You can display help and version information with the following commands:  
  
   Display help: ```java -jar target/myapp.jar --help```

   Display version: ```java -jar target/myapp.jar --version```
