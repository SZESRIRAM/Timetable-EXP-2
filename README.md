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
'''
    {% load static %}
    <!doctype html>  
  <html>
    <head>
  <meta charset="utf-8" />
  <title>Timetable</title>
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <style>
    html,body {
      margin: 20px;
      font-family: "Times New Roman", Times, serif;
      background: #ffffff;
    }

    .header-img {
      width: 100%;
      max-width: 600px;
      display: block;
      margin: 0 auto 20px;
    }

    .page-header {
      text-align: center;
      margin-bottom: 10px;
      font-weight: bold;
      font-size: 20px;
    }

    .timetable-card {
      width: 780px;
      max-width: 96%;
      margin: 8px auto 26px;
      background: #ffb3ff;
      padding: 18px;
      border: 6px solid rgba(0,0,0,0.6);
      box-shadow: 6px 6px 0 rgba(0,0,0,0.6);
    }

    .grid {
      display: grid;
      grid-template-columns: 110px repeat(6, 1fr);
      gap: 12px;
    }

    .cell {
      min-height: 36px;
      padding: 6px 8px;
      border: 2px inset rgba(0,0,0,0.12);
    }

    .col-left {
      background: #ffeb3b;
      font-weight: bold;
      text-align: center;
      border: 3px solid #b38600;
    }

    .day-header {
      background: #ffeb3b;
      border: 3px solid #b38600;
      text-align: center;
      font-weight: bold;
      padding: 6px;
    }

    .slot {
      height: 34px;
      line-height: 34px;
      border: 2px inset rgba(0,0,0,0.2);
      background: rgba(255,255,255,0.25);
      text-align: center;
      font-weight: 600;
    }

    .lunch {
      grid-column: 2 / span 6;
      text-align: center;
      font-weight: bold;
      border: 16px inset rgba(0,0,0,0.12);
    }

    .subject-table-container {
      width: 780px;
      max-width: 96%;
      margin: 20px auto;
    }

    table.subjects {
      width: 100%;
      border-collapse: collapse;
    }

    table.subjects th,
    table.subjects td {
      border: 3px solid #222;
      padding: 8px 10px;
    }

    table.subjects th {
      background: #eee;
      font-weight: 700;
    }

    </style>
    </head>
    <body>

    <img class="header-img" src="{% static 'logo.png' %}" alt="College Logo">

    <div class="page-header">
    TIMETABLE - PONSRIRAM P (25011113)
    </div>

    <div class="timetable-card">
    <div class="grid">

      <div class="col-left">Day/Time</div>
      <div class="day-header">Monday</div>
      <div class="day-header">Tuesday</div>
      <div class="day-header">Wednesday</div>
      <div class="day-header">Thursday</div>
      <div class="day-header">Friday</div>
      <div class="day-header">Saturday</div>

      <div class="col-left">8-10</div>
      <div class="cell"><div class="slot">Python</div></div>
      <div class="cell"><div class="slot">English</div></div>
      <div class="cell"><div class="slot">Web</div></div>
      <div class="cell"><div class="slot">Free</div></div>
      <div class="cell"><div class="slot">English</div></div>
      <div class="cell"><div class="slot">English</div></div>

      <div class="col-left">10-12</div>
      <div class="cell"><div class="slot">Python</div></div>
      <div class="cell"><div class="slot">Web</div></div>
      <div class="cell"><div class="slot">Free</div></div>
      <div class="cell"><div class="slot">Free</div></div>
      <div class="cell"><div class="slot">Python</div></div>
      <div class="cell"><div class="slot">English</div></div>

      <div class="col-left">12-01</div>
      <div class="lunch">LunchBreak</div>

      <div class="col-left">01-03</div>
      <div class="cell"><div class="slot">Free</div></div>
      <div class="cell"><div class="slot">Python</div></div>
      <div class="cell"><div class="slot">MentorMeet</div></div>
      <div class="cell"><div class="slot">Free</div></div>
      <div class="cell"><div class="slot">Python</div></div>
      <div class="cell"><div class="slot">Free</div></div>

      <div class="col-left">03-05</div>
      <div class="cell"><div class="slot">Web</div></div>
      <div class="cell"><div class="slot">Web</div></div>
      <div class="cell"><div class="slot">Web</div></div>
      <div class="cell"><div class="slot">Free</div></div>
      <div class="cell"><div class="slot">Free</div></div>
      <div class="cell"><div class="slot">Free</div></div>

    </div>
    </div>

    <div class="subject-table-container">
    <table class="subjects">
      <tr>
        <th>S.No</th>
        <th>SubjectCode</th>
        <th>Subject name</th>
      </tr>
      <tr><td>1</td><td>19AI414</td><td>Fundamentals of Web Application Development</td></tr>
      <tr><td>2</td><td>19EN101</td><td>Communicative English</td></tr>
      <tr><td>3</td><td>19AI301</td><td>Python Programming</td></tr>
    </table>
    </div>

    </body>
    </html>
  '''


## OUTPUT
<img width="1891" height="980" alt="image" src="https://github.com/user-attachments/assets/05f254eb-4303-49b7-bc82-14126bfcdc19" />




## RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
