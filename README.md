# employee-salary-system-using-html
<!DOCTYPE html>
<html>
  <head>
    <title>Employee Salary Processing System</title>
  </head>
  <body>
    <h1>Employee Salary Processing System</h1>
    <form action="">
      <label for="employee_name">Employee Name:</label>
      <input type="text" id="employee_name" name="employee_name"><br><br>
      <label for="position">Position:</label>
      <input type="text" id="position" name="position"><br><br>
      <label for="salary">Salary:</label>
      <input type="text" id="salary" name="salary"><br><br>
      <input type="submit" value="Submit">
    </form>
    <br>
    <table border="1">
      <tr>
        <th>Employee Name</th>
        <th>Position</th>
        <th>Salary</th>
      </tr>
      <tr>
        <td id="table_employee_name"></td>
        <td id="table_position"></td>
        <td id="table_salary"></td>
      </tr>
    </table>
    <script>
      document.querySelector('form').addEventListener('submit', function(event) {
        event.preventDefault();
        document.querySelector('#table_employee_name').innerHTML = document.querySelector('#employee_name').value;
        document.querySelector('#table_position').innerHTML = document.querySelector('#position').value;
        document.querySelector('#table_salary').innerHTML = document.querySelector('#salary').value;
      });
    </script>
  </body>
</html>
