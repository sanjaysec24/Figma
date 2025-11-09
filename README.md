# Ex09 Event Registration Web Application
## Date:9-11-2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CELENZA 2026</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background: linear-gradient(135deg, #0b0b0d, #1a1a1f);
      color: #fff;
      overflow: hidden;
    }

    .page {
      display: none;
      height: 100vh;
      width: 100%;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      text-align: center;
      padding: 20px;
    }

    .active {
      display: flex;
    }

    .logo {
      font-size: 2.5em;
      font-weight: 700;
      color: #f7c942;
      letter-spacing: 2px;
    }

    button {
      background: #f7c942;
      border: none;
      color: #000;
      font-weight: 600;
      padding: 12px 30px;
      margin-top: 15px;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s;
    }

    button:hover {
      background: #ffdb4d;
      transform: scale(1.05);
    }

    input, select {
      width: 80%;
      padding: 12px;
      margin: 10px 0;
      border-radius: 10px;
      border: none;
      text-align: center;
      font-size: 1em;
    }

    h2 {
      font-size: 2em;
      margin-bottom: 20px;
    }

    #login {
      background: radial-gradient(circle, #0a0a0a, #1c1c1c);
    }

    #events {
      background: url('https://img.freepik.com/free-vector/music-festival-stage-neon-lights_1017-31763.jpg') center/cover no-repeat;
    }

    #register {
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
    }

    #info {
      background: radial-gradient(circle at center, #4b0082, #000);
      color: #f7c942;
    }


    .highlight {
      color: #f7c942;
    }

    .footer {
      margin-top: 20px;
      font-size: 0.9em;
      opacity: 0.8;
    }
    }
  </style>
</head>
<body>

  <!-- PAGE 1: LOGIN -->
  <div class="page active" id="login">
    <div class="logo">CELENZA 2026</div>
    <input type="text" placeholder="Username" id="username">
    <input type="password" placeholder="Password" id="password">
    <button onclick="nextPage('events')">Login</button>
  </div>

  <!-- PAGE 2: EVENTS -->
  <div class="page" id="events">
    <h2>Events</h2>
    <div class="event-list">
      <p>Day 1 : <span>HHT concert</span></p>
      <p>Day 2 : <span>U1 concert</span></p>
      <p>Day 3 : <span>HARRIS concert</span></p>
    </div>
    <button onclick="nextPage('register')">Register Now</button>
  </div>

  <!-- PAGE 3: REGISTRATION -->
  <div class="page" id="register">
    <div class="logo">CELENZA 2026</div>
    <h2>Registration Form</h2>
    <input type="text" placeholder="Name">
    <input type="text" placeholder="Reg No">
    <input type="text" placeholder="Dept">
    <input type="text" placeholder="Phone No">
    <select>
      <option>Select Event</option>
      <option>HHT Concert</option>
      <option>U1 Concert</option>
      <option>HARRIS Concert</option>
    </select>
    <button onclick="nextPage('info')">Submit Form</button>
  </div>

  <!-- PAGE 4: INFO -->
  <div class="page" id="info">
    <h2>Get ready to be part of the celebration!</h2>
    <div class="logo">CELENZA 2026</div>
    <p class="footer">For any info:<br><span class="highlight">@www.celenza26.com</span></p>
    <div class="crowd"></div>
  </div>

  <script>
    function nextPage(id) {
      document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>
</body>
</html>
```

## OUTPUT:
<img width="1920" height="1200" alt="Screenshot 2025-11-09 160002" src="https://github.com/user-attachments/assets/77c7340b-a985-4dfc-9626-f73c2c208fde" />

click here to view prototype 🔻

https://www.figma.com/proto/XftENAtZnmOMCwPmIQxujk/Untitled?node-id=0-1&t=TDhU7793cL9ifVzN-1

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
