def categorize_command(command):
    # Dictionary of commands and their categories
    command_categories = {
        "for": "Looping Structure",
        "while": "Looping Structure",
        "if": "Conditional Statement",
        "else": "Conditional Statement",
        "elif": "Conditional Statement",
        "def": "Function Definition",
        "return": "Function Definition",
        "import": "Module Import",
        "open": "File I/O",
        "close": "File I/O",
        "read": "File I/O",
        "write": "File I/O",
        "list": "Data Structures",
        "tuple": "Data Structures",
        "dict": "Data Structures",
        "set": "Data Structures",
        "append": "Data Structures (List)",
        "pop": "Data Structures (List)",
        "insert": "Data Structures (List)",
        "sort": "Data Structures (List)",
        "join": "String Methods",
        "split": "String Methods",
        "len": "Built-in Functions",
        "range": "Built-in Functions",
        "print": "Built-in Functions",
        "input": "Built-in Functions",
        "type": "Built-in Functions",
        "map": "Higher-Order Functions",
        "filter": "Higher-Order Functions",
        "lambda": "Anonymous Functions",
        "class": "Object-Oriented Programming",
        "self": "Object-Oriented Programming",
        "constructor": "Object-Oriented Programming",
        "inheritance": "Object-Oriented Programming",
        "try": "Error Handling",
        "except": "Error Handling",
        "finally": "Error Handling"
    }

    # Check if the command is in the dictionary
    if command in command_categories:
        return command_categories[command]
    else:
        return "Command not found in the list. Please add it."

# Example usage
def main():
    print("Enter a programming command to categorize:")
    command = input().strip()

    category = categorize_command(command)
    print(f"The command '{command}' belongs to the category: {category}")

if __name__ == "__main__":
    main()

