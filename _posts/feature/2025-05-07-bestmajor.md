---
layout: post
title: What type of Major Should you Choose!
search_exclude: true
hide: false
permalink: /game
---
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>🔍 Project Match: Which Profile Fits You?</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&family=Nunito:wght@400;700&display=swap" rel="stylesheet">
  <style>
            header, .site-header, .top-banner {
  display: none !important;
    } 
    body {
      font-family: 'Nunito', sans-serif;
      background: linear-gradient(to right, #003366, #336699);
      color: #fff;
      padding: 30px;
      max-width: 900px;
      margin: auto;
      border-radius: 10px;
    }
    h1, h2 {
      text-align: center;
      margin-top: 20px;
    }
    .hero {
      background-color: #004080;
      padding: 20px;
      border-radius: 10px;
      margin-bottom: 20px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
    }
    .overview, .profiles {
      background-color: #0059b3;
      padding: 20px;
      border-radius: 10px;
      margin-bottom: 20px;
    }
    .profile {
      background-color: #1976d2;
      margin-top: 10px;
      padding: 10px;
      border-radius: 6px;
    }
    .question-step {
      display: none;
      background-color: #004d99;
      padding: 20px;
      border-radius: 10px;
      margin-top: 20px;
      text-align: center;
    }
    .options {
      display: flex;
      justify-content: space-around;
      flex-wrap: wrap;
      gap: 20px;
      margin-top: 20px;
    }
    .option-img {
      border: 4px solid transparent;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s ease;
      max-width: 150px;
    }
    .option-img:hover {
      border-color: #ffcc00;
      transform: scale(1.05);
    }
    .active {
      display: block;
    }
    .next-btn {
      margin-top: 20px;
      background-color: #ffcc00;
      color: #003366;
      border: none;
      padding: 12px 25px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 18px;
    }
    .result {
      display: none;
      background: linear-gradient(to right, #ffcc70, #ff9472);
      color: #002244;
      padding: 30px;
      border-radius: 15px;
      margin-top: 30px;
      font-family: 'Fredoka One', cursive;
      font-size: 20px;
      text-align: center;
      box-shadow: 0 6px 20px rgba(0,0,0,0.4);
    }
    .result h2 {
      font-size: 32px;
      color: #fff;
      text-shadow: 1px 1px 4px rgba(0,0,0,0.4);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>🎯 Here is a Buzzfeed Game</h1>
    <p style="text-align:center">See which one of these profiles you fit best with depending on your projects!</p>
  </div>

  <div class="overview">
    <h2>🔍 Project Matcher Overview</h2>
    <p>This fun quiz helps you match your personality and project interests to real students' profiles and suggests what college and major may suit you best!</p>
  </div>

  <div class="profiles">
    <h2>👥 Profile Examples</h2>
    <div class="profile"><strong>Alice - Environmental Engineer @ UC Berkeley</strong><br>Project: ML model to detect water contamination.</div>
    <div class="profile"><strong>Bob - Cognitive Science @ UCLA</strong><br>Project: Mental health chatbot with journaling features.</div>
    <div class="profile"><strong>Clara - Computer Science @ Stanford</strong><br>Project: Multiplayer game teaching chemistry through puzzles.</div>
    <div class="profile"><strong>Dev - Data Science @ UC San Diego</strong><br>Project: Visualized government data to optimize bus routes.</div>
    <div class="profile"><strong>Eva - Animation @ CalArts</strong><br>Project: Animated series explaining climate change.</div>
  </div>

  <div id="quiz-container">
    <div class="question-step active" id="q1">
      <h2>1. Choose your personality</h2>
      <div class="options">
        <img src="https://placehold.co/150x150/003366/ffffff?text=Creative" class="option-img" onclick="selectOption('personality', 'creative')">
        <img src="https://placehold.co/150x150/003366/ffffff?text=Analytical" class="option-img" onclick="selectOption('personality', 'analytical')">
        <img src="https://placehold.co/150x150/003366/ffffff?text=Empathetic" class="option-img" onclick="selectOption('personality', 'empathetic')">
        <img src="https://placehold.co/150x150/003366/ffffff?text=Logical" class="option-img" onclick="selectOption('personality', 'logical')">
      </div>
    </div>
    <div class="question-step" id="q2">
      <h2>2. Choose what you enjoy most in a project</h2>
      <div class="options">
        <img src="https://placehold.co/150x150/336699/ffffff?text=Design" class="option-img" onclick="selectOption('favoritePart', 'design')">
        <img src="https://placehold.co/150x150/336699/ffffff?text=Data+Analysis" class="option-img" onclick="selectOption('favoritePart', 'data analysis')">
        <img src="https://placehold.co/150x150/336699/ffffff?text=Storytelling" class="option-img" onclick="selectOption('favoritePart', 'storytelling')">
        <img src="https://placehold.co/150x150/336699/ffffff?text=Coding" class="option-img" onclick="selectOption('favoritePart', 'coding')">
      </div>
    </div>
    <div class="question-step" id="q3">
      <h2>3. What's your project style?</h2>
      <div class="options">
        <img src="https://placehold.co/150x150/004080/ffffff?text=Team-Based" class="option-img" onclick="selectOption('style', 'team')">
        <img src="https://placehold.co/150x150/004080/ffffff?text=Solo+Inventor" class="option-img" onclick="selectOption('style', 'solo')">
      </div>
    </div>
    <div class="question-step" id="q4">
      <h2>4. Which tool do you use the most?</h2>
      <div class="options">
        <img src="https://placehold.co/150x150/0059b3/ffffff?text=Python" class="option-img" onclick="selectOption('tool', 'python')">
        <img src="https://placehold.co/150x150/0059b3/ffffff?text=Adobe+Suite" class="option-img" onclick="selectOption('tool', 'adobe')">
        <img src="https://placehold.co/150x150/0059b3/ffffff?text=Excel" class="option-img" onclick="selectOption('tool', 'excel')">
        <img src="https://placehold.co/150x150/0059b3/ffffff?text=Unity" class="option-img" onclick="selectOption('tool', 'unity')">
      </div>
    </div>
    <div class="question-step" id="q5">
      <h2>5. Which of these motivates you most?</h2>
      <div class="options">
        <img src="https://placehold.co/150x150/1976d2/ffffff?text=Helping+Others" class="option-img" onclick="selectOption('motivation', 'helping')">
        <img src="https://placehold.co/150x150/1976d2/ffffff?text=Innovation" class="option-img" onclick="selectOption('motivation', 'innovation')">
        <img src="https://placehold.co/150x150/1976d2/ffffff?text=Solving+Mysteries" class="option-img" onclick="selectOption('motivation', 'mystery')">
        <img src="https://placehold.co/150x150/1976d2/ffffff?text=Artistic+Expression" class="option-img" onclick="selectOption('motivation', 'expression')">
      </div>
    </div>
  </div>

  <div id="result" class="result"></div>

  <script>
    let answers = {};
    let step = 1;

    function selectOption(key, value) {
      answers[key] = value;
      document.getElementById('q' + step).classList.remove('active');
      step++;
      const next = document.getElementById('q' + step);
      if (next) {
        next.classList.add('active');
      } else {
        showResult();
      }
    }

    const projectDB = [
      { student: "Alice", project: "Built a machine learning model to predict water contamination", college: "UC Berkeley", major: "Environmental Engineering", tags: ["data analysis", "analytical", "python", "helping"] },
      { student: "Bob", project: "Mental health tracking app with journaling/chatbot", college: "UCLA", major: "Cognitive Science", tags: ["user research", "empathetic", "solo", "helping"] },
      { student: "Clara", project: "Educational game to teach chemistry", college: "Stanford", major: "Computer Science", tags: ["design", "creative", "unity", "expression"] },
      { student: "Dev", project: "Visualized local government data for transportation", college: "UC San Diego", major: "Data Science", tags: ["data analysis", "logical", "excel", "innovation"] },
      { student: "Eva", project: "Animated climate science series for kids", college: "CalArts", major: "Animation", tags: ["storytelling", "creative", "adobe", "expression"] }
    ];

    function showResult() {
      let bestMatch = null;
      let bestScore = -1;

      for (const profile of projectDB) {
        let score = 0;
        for (const val of Object.values(answers)) {
          if (profile.tags.includes(val)) score++;
        }
        if (score > bestScore) {
          bestScore = score;
          bestMatch = profile;
        }
      }

      const result = document.getElementById('result');
      if (bestMatch) {
        result.innerHTML = `
          <h2>🎉 Congratulations! You Match With:</h2>
          <p><strong>👤 Student:</strong> ${bestMatch.student}</p>
          <p><strong>🎓 College:</strong> ${bestMatch.college}</p>
          <p><strong>📘 Major:</strong> ${bestMatch.major}</p>
          <p><strong>🛠 Project:</strong> ${bestMatch.project}</p>
        `;
        result.style.display = 'block';
        window.scrollTo({ top: document.body.scrollHeight, behavior: 'smooth' });
      }
    }
  </script>
</body>
</html>