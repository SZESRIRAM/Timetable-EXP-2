# Ex02 Time Table
## Date:

## AIM
To write a html webpage page to display your slot timetable.

## ALGORITHM
### STEP 1
Create a Django-admin Interface.

### STEP 2
Create an App inside the Django project.

### STEP 2
Create a static folder uder the created App and insert HTML code.

### STEP 3
Create a simple table using ```<table>``` tag in html with the relevant attributes.

### STEP 4
Add rows using ```<tr>``` tag.

### STEP 5
Add your course schedule using ```<td>``` tag.

### STEP 6
Execute the program using runserver command.

## PROGRAM
home.html
  <!DOCTYPE html>
{% load static %}
<html>
<head>
  <title>Time Table</title>
  <style>
    body {
      font-family: "Roboto", sans-serif;
      background-color: #f9f9f9;
      text-align: center;
      margin: 20px;
    }

    h2 {
      color: #101011ff;
    }
    table {
      border-collapse: collapse;
      margin: 25px auto;
      width: 85%;
      background: white;
      box-shadow: 0px 0px 8px rgba(0, 0, 0, 0.2);
      border-radius: 10px;
    }

    th, td {
      border: 1px solid #555;
      padding: 10px;
      text-align: center;
    }

    th {
      background-color: #8bd6fcff;
      color: black;
    }

    td {
      font-weight: bold;
    }

    tr:nth-child(even) {
      background-color: #f7faf0ff;
    }

    .sub-table {
      width: 60%;
      margin-top: 30px;
    }

    .sub-table th {
      background-color: #0c0c0cff;
      color: white;
    }

    footer {
      margin-top: 20px;
      font-style: italic;
      color: #444;
    }
    </style>
    </head>
    <body>
    <img src={% static 'logo.png' %}>

    <h2>TIME TABLE BY PONSRIRAM (25011113)</h2>

    <table>
    <tr>
      <th>Day/Time</th>
      <th>Monday</th>
      <th>Tuesday</th>
      <th>Wednesday</th>
      <th>Thursday</th>
      <th>Friday</th>
      <th>Saturday</th>
    </tr>
    <tr>
      <td>8-10</td>
      <td>PYTHON</td>
      <td>ENG</td>
      <td>WEB</td>
      <td>FREE</td>
      <td>ENG</td>
      <td>ENG</td>
    </tr>
    <tr>
      <td>10-12</td>
      <td>PYTHON</td>
      <td>WEB</td>
      <td>FREE</td>
      <td>FREE</td>
      <td>Python</td>
      <td>ENG</td>
    </tr>
    <tr>
      <td>12-1</td>
      <td colspan="6" style="background:#00000;">L U N C H</td>
    </tr>
    <tr>
      <td>1-3</td>
      <td>FREE</td>
      <td>Python</td>
      <td>MENTOR</td>
      <td>FREE</td>
      <td>Python</td>
      <td>FREE</td>
    </tr>
    <tr>
      <td>3-5</td>
      <td>WEB</td>
      <td>WEB</td>
      <td>WEB</td>
      <td>FREE</td>
      <td>FREE</td>
      <td>FREE</td>
    </tr>
    </table>

    <table class="sub-table">
    <tr>
      <th>Subject Code</th>
      <th>Subject Name</th>
    </tr>
    <tr>
      <td>19AI414</td>
      <td>Fundamentals of Web Application Development (FWAD)</td>
    </tr>
    <tr>
      <td>19EN101</td>
      <td>Communicative english</td>
    </tr>
    <tr>
      <td>19AI301</td>
      <td>Python Programming</td>
    </tr>
    </table>

    </body>
    </html>



## OUTPUT


## RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
