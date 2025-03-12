**Task: Basic Todo List Manager using Bash**

**Goal:**

Create a simple "Todo List Manager" using Bash scripting, where tasks are saved in a plain text file. This project will introduce you to basic file handling, keeping track of tasks, and using some important Linux commands.

**Task Breakdown:**

**1. Step 1: Set Up the Project**

* Make a new folder called ```simple\_todo```.
* Inside this folder, create a text file called ```todo.txt``` to store your tasks.

The file should start off empty. Each task will go on its own line. If a task is finished, you will mark it with ```[DONE]``` at the beginning of the line.

**2. Step 2: Write the Bash Script**

* Write a Bash script called ```todo.txt``` that will let you manage the tasks. It should handle these commands:
  1. **Add a task**: Add a new task to the list (saved in ```todo.txt```).
  2. **List tasks**: Show all tasks, and show which are finished and which are not.
  3. **Mark a task as done**: Mark a specific task as finished.
  4. **Remove a task**: Delete a task from the list.
  5. **Help**: Show instructions on how to use the script.

**3. Step 3: Add Basic Features**

**Command 1: Add Task**

* You can add a new task by typing:

```bash
./todo.sh add "Task description"
```

**Command 2: List All Tasks**

* You can see all your tasks by typing:

```bash
./todo.sh list
```
* This will display everything in the ```todo.txt``` file. Tasks that are finished will have ```[DONE]``` in front of them.

**Command 3: Mark Task as Done**

* To mark a task as done, use the task number (starting from 1 for the first task):

```bash
./todo.sh done 2
```
* This command will go to the second task in the file and mark it as ```[DONE]```.

**Command 4: Remove a Task**

* You can delete a task by using its number:

```bash
./todo.sh remove 3
```
* This will delete the third task from the ```todo.txt``` file.

**Command 5: Help**

* You can see a list of available commands by typing:

```bash
./todo.sh help
```
* This will show short explanations of how to use each command.

**Step 4: Extra Challenges (Optional)**

1. **Backup the Todo List**:
   Each time you add or complete a task, save a copy of the todo.txt file as a backup. Name the backup todo\_backup.txt and save it in the same folder.
2. **Undo the Last Change**:
   Make a feature that lets you undo the last thing you did (like removing or marking a task as done). You can use the backup file from the step above to do this.
3. **Search for Tasks**:
   Add a search feature to find tasks that contain a specific word. For example:

```bash
./todo.sh search "groceries"
```
This will show all tasks that include the word "groceries."

**Linux Commands to Learn:**

While working on this task, you will use some basic Linux commands:

* **cat**: To show the contents of files (for displaying tasks).
* **echo**: To add new tasks to the todo.txt file.
* **sed**: To change specific lines in the file (for marking tasks as done).
* **rm**: To delete tasks.
* **touch**: To create files.
* **chmod**: To make your script executable (so it can run).

**Submission Requirements:**

1. A working todo.sh script.
2. A todo.txt file with at least 3 tasks.
3. A simple README file that explains how to use the script.

**What You'll Learn:**

* **Basic File Handling**: How to create, read, and edit files in Bash.
* **Basic Bash Scripting**: How to use simple loops, conditionals, and functions in Bash.
* **Linux Commands**: Understanding important commands like cat, sed, rm, and echo.
* **Keeping Track of Tasks**: How to manage data (like tasks) in a file.