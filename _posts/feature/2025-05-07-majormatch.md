---
layout: post
title: Major Matching | STEM Database
search_exclude: true
description: Get your major matched!
hide: false
permalink: /majormatch
---


<head>

  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      background: linear-gradient(to right, #fce4ec, #e1f5fe);
      color: #333;
    }
        header, .site-header, .top-banner {
  display: none !important;
    } 

    header {
      background-color: #006064;
      color: white;
      padding: 1.5rem 2rem;
      text-align: center;
    }

    header h1 {
      margin: 0;
    }

    .content {
      max-width: 900px;
      margin: 2rem auto;
      padding: 0 1.5rem;
    }

    h2 {
      color: #006064;
    }

    form {
      margin-top: 1rem;
      background-color: #ffffff;
      padding: 1.5rem;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }

    input[type="text"] {
      width: 100%;
      padding: 0.8rem;
      font-size: 1rem;
      margin-top: 0.5rem;
      border: 1px solid #ccc;
      border-radius: 8px;
    }

    button {
      margin-top: 1rem;
      padding: 0.8rem 1.5rem;
      background-color: #006064;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 1rem;
      cursor: pointer;
    }

    .result {
      margin-top: 2rem;
      background-color: #e0f2f1;
      padding: 1rem;
      border-radius: 10px;
      display: none; /* Will be shown via JS */
    }

    table {
      width: 100%;
      margin-top: 2rem;
      border-collapse: collapse;
    }

    th, td {
      padding: 0.8rem;
      text-align: left;
      border-bottom: 1px solid #ccc;
    }

    th {
      background-color: #b2dfdb;
    }
  </style>
</head>
<body>

  <header>
    <h1>Major Matching</h1>
    <p>Input your STEM project idea and find majors that align with your interests!</p>
  </header>

  <div class="content">
    <h2>🔍 Find Your Match</h2>
    <form id="matchForm">
      <label for="project">Describe your project type or topic:</label>
      <input type="text" id="project" name="project" placeholder="e.g., building a water filtration system" required />
      <button type="submit">Match Me!</button>
    </form>

    <div class="result" id="matchResult">
      <h3>🎓 Suggested Major:</h3>
      <p><strong id="matchedMajor">Environmental Engineering</strong></p>
    </div>

    <h2>📋 Student Project Database</h2>
    <table>
      <thead>
        <tr>
          <th>Name</th>
          <th>College</th>
          <th>Major</th>
          <th>Project</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Aiden Kim</td>
          <td>MIT</td>
          <td>Mechanical Engineering</td>
          <td>3D-printed drone prototype</td>
        </tr>
        <tr>
          <td>Rhea Patel</td>
          <td>Stanford</td>
          <td>Environmental Engineering</td>
          <td>Water purification system</td>
        </tr>
        <tr>
          <td>Lalita Chen</td>
          <td>UC Berkeley</td>
          <td>Computer Science</td>
          <td>AI-powered math tutor</td>
        </tr>
      </tbody>
    </table>
  </div>

  <script>
    // Example match simulation (just for demonstration)
    const form = document.getElementById('matchForm');
    const resultBox = document.getElementById('matchResult');
    const matchDisplay = document.getElementById('matchedMajor');

    form.addEventListener('submit', function(e) {
      e.preventDefault();
      const input = document.getElementById('project').value.toLowerCase();

      let match = "Engineering";
      if (input.includes("water") || input.includes("environment")) {
        match = "Environmental Engineering";
      } else if (input.includes("robot") || input.includes("mechanical")) {
        match = "Mechanical Engineering";
      } else if (input.includes("software") || input.includes("app") || input.includes("ai")) {
        match = "Computer Science";
      } else if (input.includes("bridge") || input.includes("structure")) {
        match = "Civil Engineering";
      }

      matchDisplay.textContent = match;
      resultBox.style.display = 'block';
    });
  </script>

</body>
</html>

