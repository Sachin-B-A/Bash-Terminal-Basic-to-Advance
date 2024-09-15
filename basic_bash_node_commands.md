
# Basic Bash, Terminal, and Node Commands

## WSL Commands (Windows Subsystem for Linux):

1. **`pwd`**  
   *Print Working Directory*: Displays the current directory you're in.
   ```bash
   pwd
   ```

2. **`cd`**  
   *Change Directory*: Navigate to a specific directory.  
   Example:  
   ```bash
   cd desktop/Coding
   ```

   - To go back one level, use:  
   ```bash
   cd ..
   ```

   - To go back two levels:  
   ```bash
   cd ../..
   ```

3. **`ls`**  
   *List*: Lists all files and directories in the current directory.
   ```bash
   ls
   ```

4. **`mkdir`**  
   *Make Directory*: Creates a new directory.  
   Example:
   ```bash
   mkdir myFolder
   ```

5. **`touch`**  
   *Create a File*: Creates a new file.
   ```bash
   touch filename.txt
   ```

6. **`cat`**  
   *Concatenate and Display*: Displays the content of a file.
   ```bash
   cat filename.txt
   ```

7. **Edit using Vim Editor:**
   - Open a file with `vim`:  
     ```bash
     vim filename.txt
     ```

   - To enter **Insert Mode** (to edit the file), press:  
     `i`

   - To exit without saving:  
     Press `esc` and type `:q!`

   - To save changes and exit:  
     Press `esc` and type `:wq!`

8. **`mv`**  
   *Move or Rename a File*:  
   Example (Move `hello.txt` to `hellofolder`):
   ```bash
   mv hello.txt hellofolder/
   ```

9. **`cp`**  
   *Copy Files*:  
   Example (Copy `hello.txt` to `hello` folder):
   ```bash
   cp hello.txt hello/
   ```

   - To copy directories (including all contents), use the `-r` flag:  
     Example (Copy `demo` directory one level up):
     ```bash
     cp -r demo ../
     ```

---

## Node.js Commands

1. **`node`**  
   Starts the Node.js interactive shell (REPL). You can execute JavaScript code directly.
   ```bash
   node
   ```

2. **Running JavaScript Files**  
   Execute a JavaScript file using Node.js.
   ```bash
   node filename.js
   ```

3. **Using Vim to Write and Run Code**  
   You can write your JavaScript code in a file using Vim and run it with Node.js:
   - Open a file with `vim`:
     ```bash
     vim a.js
     ```
   - Insert your code and save the file, then run:
     ```bash
     node a.js
     ```

4. **`npm` (Node Package Manager)**  
   Manages project dependencies from the npm registry.

   - To list installed packages in your project:
     ```bash
     npm list
     ```

   - For a list of all possible npm commands, simply run:
     ```bash
     npm
     ```
