# Aayu Language 🚀

**Aayu** is a brand new, highly readable, intent-driven programming language designed to bridge the gap between human thought and executable code.

## 🧠 How it Works

Aayu follows a clean, modern compilation pipeline:
**Human Intent** → **Aayu Code** → **AST (Abstract Syntax Tree)** → **Execution**

The language features a custom lexer, parser, and interpreter, enabling features like structured records, variable declarations, loops, error handling, and tasks (functions) in a natural syntax.

---

## 📂 Projects

### 1. Student Management API (Pure Aayu)
This repository contains a fully functional **Student Management API** built entirely in **Pure Aayu** to demonstrate the language's backend capabilities.

**Features Implemented:**
- `Student` entity record.
- File I/O operations (`read` and `write` to `students.txt`) for persistent data storage.
- Modularized architecture using Aayu's `use` keyword.
- Custom tasks simulating an API Layer (POST, GET, PUT, DELETE).
- CRUD operations.

#### Example: `student.aayu`
```aayu
record Student.
    name
    age
    email
end.
```

#### Example: `main.aayu`
```aayu
use api.
use routes.

show "=== Student API ===".
run start_server.

run post_student with "Ayush" and "21" and "test@test.com".
run get_student_route.

run put_student with "Ayush" and "22" and "test@test.com".
run get_student_route.

run delete_student_route.
```

---

## 🚀 Running the Project

Ensure you have Python installed to run the interpreter.

```bash
python run.py project_8_student_api/main.aayu
```

**Expected Output:**
```text
=== Student API ===
API Started
POST /student
Student Created
GET /student
Ayush,21,test@test.com
PUT /student
Student Updated
GET /student
Ayush,22,test@test.com
DELETE /student
Student Deleted
```

---

## 🛠️ Future Roadmap (Phase 2)

Aayu is rapidly evolving! The next steps for the language include:
1. **Building more Real-World Projects:**
   - E-Commerce System
   - Task Manager
   - HTTP Web Backend Framework
2. **Aayu Specification v1.0:** Freezing the syntax and features.
3. **VS Code Extension:** Adding official syntax highlighting and IntelliSense for `.aayu` files.
4. **GitHub Linguist PR:** Registering Aayu as an official GitHub language!