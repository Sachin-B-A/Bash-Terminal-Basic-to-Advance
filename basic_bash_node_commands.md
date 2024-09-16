---

### **Basic Bash and Terminal Commands**

#### **WSL Commands (Windows Subsystem for Linux)**
1. **`pwd`**  
   *Print Working Directory*: Displays the current directory.
   ```bash
   pwd
   ```

2. **`cd`**  
   *Change Directory*: Navigate to a specific directory.  
   Example:  
   ```bash
   cd desktop/Coding
   ```
   - To go back one level:
     ```bash
     cd ..
     ```
   - To go back two levels:
     ```bash
     cd ../..
     ```

3. **`ls`**  
   *List*: Lists all files and directories.
   ```bash
   ls
   ```
   - **Variations**:
     - `ls -l`: Detailed list view.
     - `ls -r`: Reverse order listing.
     - `ls -t`: Sort by time last modified.
     - `ls -lt`: Combine detailed list and time sorting.
     - `ls -la`: List all, including hidden files.
     - `ls -s`: Sort by file size.
     - `ls -lR | grep .json`: Find files with a particular format.

4. **`mkdir`**  
   *Make Directory*: Creates a new directory.  
   Example:
   ```bash
   mkdir newdir
   ```

5. **`touch`**  
   *Create a File*: Creates a new file.  
   Example:
   ```bash
   touch filename.txt
   ```

6. **`cat`**  
   *Concatenate and Display*: Displays file content.  
   - To overwrite file content:
     ```bash
     cat > text.txt
     ```
   - To append to a file:
     ```bash
     cat >> text.txt
     ```

7. **Vim Editor**  
   - Open a file with Vim:
     ```bash
     vim hi.txt
     ```
   - To enter **Insert Mode**, press:
     ```bash
     i
     ```
   - To exit without saving, press `esc` and type:
     ```bash
     :q!
     ```
   - To save and exit, press `esc` and type:
     ```bash
     :wq!
     ```

8. **`mv`**  
   *Move or Rename a File*:  
   - Move a file to a folder:
     ```bash
     mv hello.txt hellofolder/
     ```
   - Rename a file:
     ```bash
     mv hello.txt renamed.txt
     ```

9. **`cp`**  
   *Copy Files*:  
   Example (Copy `hello.txt` to `hello` folder):
   ```bash
   cp hello.txt hello/
   ```
   - To copy directories (recursively):
     ```bash
     cp -r demo ../
     ```

10. **`rm`**  
    *Remove/Delete Files*:
    ```bash
    rm hello.txt
    ```
    - To delete a directory and its contents:
      ```bash
      rm -r hello/
      ```

---

### **Node.js Commands**

1. **`node`**  
   Start the Node.js interactive shell (REPL).
   ```bash
   node
   ```

2. **Running JavaScript Files**  
   Run a JavaScript file using Node.js:
   ```bash
   node a.js
   ```

3. **`npm` (Node Package Manager)**  
   - List installed packages:
     ```bash
     npm list
     ```
   - To see all available `npm` commands:
     ```bash
     npm
     ```

---

### **Advanced Bash Commands**

1. **Chaining Commands**  
   Combine multiple commands in one line.
   ```bash
   mkdir newdir && cd newdir
   ```

2. **File Permissions with `chmod`**  
   Change file permissions:
   ```bash
   chmod ugo-rwx filename
   ```
   - `ugo`: User, Group, Others.
   - `rwx`: Read, Write, Execute.

   Examples:
   - Grant execute permission to the user:
     ```bash
     chmod u+x NewFolder.txt
     ```
   - Allow user to write and execute:
     ```bash
     chmod u+wx NewFolder.txt
     ```
   - Remove write and execute permissions from user:
     ```bash
     chmod u-wx NewFolder.txt
     ```
   - Give full permissions (read, write, execute) to everyone:
     ```bash
     chmod 777 NewFolder.txt
     ```

3. **`echo`**  
   Display a message:
   ```bash
   echo "Hello World"
   ```

4. **Viewing File Content**  
   - Display the first 10 lines of a file:
     ```bash
     head hello.txt
     ```
   - Display the last 10 lines of a file:
     ```bash
     tail hello.txt
     ```
   - Display the first 20 lines of a file:
     ```bash
     head -20 hello.txt
     ```

5. **Word Count with `wc`**  
   Count the number of lines in a file:
   ```bash
   wc -l hello.txt
   ```

6. **Command Chaining**  
   Chain commands together using `|`:
   ```bash
   grep "Yess" hellotext.txt | wc -l
   ```
   - To search for a word (case-insensitive):
     ```bash
     grep -hi "Yess" hellotext.txt
     ```

---
