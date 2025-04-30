# MWAD-EX_03-To-Do-List-using-JavaScript
## Date:30-04-2025

## Name:  GOKUL S
## Ref.No:212223040051

## AIM
To create a To-do Application with all features using JavaScript.

## ALGORITHM
### STEP 1
Build the HTML structure (index.html).

### STEP 2
Style the App (style.css).

### STEP 3
Plan the features the To-Do App should have.

### STEP 4
Create a To-do application using Javascript.

### STEP 5
Add functionalities.

### STEP 6
Test the App.

### STEP 7
Open the HTML file in a browser to check layout and functionality.

### STEP 8
Fix styling issues and refine content placement.

### STEP 9
Deploy the website.

### STEP 10
Upload to GitHub Pages for free hosting.

## PROGRAM
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Activity App</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f2f5;
      margin: 0;
      padding: 0;
    }

    .container {
      max-width: 400px;
      margin: 80px auto;
      background: white;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0,0,0,0.1);
    }

    h1 {
      text-align: center;
      color: #333;
    }

    .input-container {
      display: flex;
      gap: 10px;
      margin-bottom: 20px;
    }

    input[type="text"] {
      flex: 1;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    button {
      padding: 10px 20px;
      border: none;
      background-color: #28a745;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }

    button:hover {
      background-color: #218838;
    }

    ul {
      list-style: none;
      padding: 0;
    }

    li {
      padding: 10px;
      background-color: #fafafa;
      border: 1px solid #ddd;
      border-radius: 5px;
      margin-bottom: 10px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    li.completed {
      text-decoration: line-through;
      color: gray;
    }

    li button {
      background-color: #dc3545;
      border: none;
      color: white;
      padding: 6px 10px;
      border-radius: 3px;
      cursor: pointer;
    }

    li button:hover {
      background-color: #c82333;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>My Activity List</h1>
    <div class="input-container">
      <input type="text" id="taskInput" placeholder="Add a new task..." />
      <button onclick="addTask()">Add</button>
    </div>
    <ul id="taskList"></ul>
  </div>

  <script>
    function addTask() {
      const input = document.getElementById("taskInput");
      const taskText = input.value.trim();

      if (taskText === "") return;

      const li = document.createElement("li");
      li.textContent = taskText;

      li.addEventListener("click", function () {
        li.classList.toggle("completed");
      });

      const deleteBtn = document.createElement("button");
      deleteBtn.textContent = "Delete";
      deleteBtn.onclick = function () {
        li.remove();
      };

      li.appendChild(deleteBtn);
      document.getElementById("taskList").appendChild(li);
      input.value = "";
    }
  </script>
</body>
</html>



## OUTPUT
![Screenshot 2025-04-30 090517](https://github.com/user-attachments/assets/f9ccc716-e256-451f-bbad-606d5eb39b62)


## RESULT
The program for creating To-do list using JavaScript is executed successfully.
