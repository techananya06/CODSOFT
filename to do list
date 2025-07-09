todo_list = []

def show_menu():
    print("\n--- TO-DO LIST MENU ---")
    print("1. View Tasks")
    print("2. Add Task")
    print("3. Remove Task")
    print("4. Exit")

while True:
    show_menu()
    choice = input("Enter your choice (1-4): ")

    if choice == "1":
        print("\nYour Tasks:")
        if not todo_list:
            print("No tasks yet!")
        else:
            for i, task in enumerate(todo_list, 1):
                print(f"{i}. {task}")

    elif choice == "2":
        task = input("Enter the task to add: ")
        todo_list.append(task)
        print("Task added!")

    elif choice == "3":
        if not todo_list:
            print("No tasks to remove.")
        else:
            for i, task in enumerate(todo_list, 1):
                print(f"{i}. {task}")
            index = int(input("Enter task number to remove: "))
            if 0 < index <= len(todo_list):
                removed = todo_list.pop(index - 1)
                print(f"Removed: {removed}")
            else:
                print("Invalid number.")

    elif choice == "4":
        print("Goodbye!")
        break

    else:
        print("Please enter a valid option.")
