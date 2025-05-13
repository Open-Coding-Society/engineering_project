---
layout: post
title: STEM Engineering Database Hub
search_exclude: true
description: Explore STEM projects, match to majors, discover engineering fields, and connect with peers!
hide: true
menu: nav/home.html
---


<head>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to right, #e0f7fa, #e1bee7);
      color: #333;
    }

    header {
      background-color: #6a1b9a;
      color: white;
      padding: 1.5rem 2rem;
      text-align: center;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }

    header h1 {
      margin: 0;
      font-size: 2.5rem;
    }

    header p {
      margin-top: 0.5rem;
      font-size: 1.1rem;
    }

    .container {
      max-width: 1000px;
      margin: 2rem auto;
      padding: 0 1.5rem;
      display: grid;
      gap: 1.5rem;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    }

    .card {
      background: white;
      border-radius: 12px;
      padding: 1.5rem;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      transition: transform 0.2s ease;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    .card h2 {
      margin-top: 0;
      color: #6a1b9a;
    }

    .card p {
      font-size: 0.95rem;
      color: #555;
    }

    .card a {
      display: inline-block;
      margin-top: 1rem;
      color: #6a1b9a;
      font-weight: bold;
      text-decoration: none;
    }

    footer {
      text-align: center;
      padding: 1rem;
      background-color: #f3e5f5;
      margin-top: 3rem;
      font-size: 0.9rem;
      color: #777;
    }
  </style>
</head>
<body>


  <div class="container">
    <div class="card">
      <h2>🎓 Major Matching</h2>
      <p>View a database of past students, their college majors, and STEM projects. Enter your project type to get matched with potential majors!</p>
      <a href="/flocker_frontend/majormatch">Explore Majors →</a>
    </div>

    <div class="card">
      <h2>⚙️ Engineering Types & Careers</h2>
      <p>Learn about different engineering disciplines and future job opportunities. Participate in a survey to see what’s most popular among students!</p>
      <a href="/flocker_frontend/survey">Explore Majors →</a>
    </div>

    <div class="card">
      <h2>💬 Q&A Forum</h2>
      <p>Ask questions, give answers, and explore a database of frequently asked questions. Great for peer support!</p>
      <a href="/flocker_frontend/posts">Explore Majors →</a>
    </div>
  </div>

  <footer>
    &copy; 2025 STEM Database Project | Built with ❤️ by Students
  </footer>

</body>
