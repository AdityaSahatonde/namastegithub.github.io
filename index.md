<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="index.css">
    <title>To-do List</title>
</head>
<body>
  <main id="main"> 
      <header id="header">

      </header>

      <section id ="section">
        <h1 id="h1">To Do List</h1>
        <input type="text" id = "input" class="inp" placeholder="Add a Task">
        <input type="hidden" id="saveindex">
        <button type="button" id="btn" class="button">Add</button>
        <button type="button" id="savebtn" class="button" style="display: none;">Save</button>
        <table id="table" class="table1">
         
        </table>

      </section>

      <footer id = "footer">

      </footer>
      <script src="index.js"></script>
  </main>  
</body>
</html>
