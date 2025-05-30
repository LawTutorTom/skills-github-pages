

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Bar Exam Mastery</title>
  <style>
    body {
      margin: 0;
      font-family: sans-serif;
      background: linear-gradient(to bottom, #ffffff, #e0f2fe);
      color: #1f2937;
    }
    header {
      padding: 1.5rem;
      text-align: center;
      background-color: white;
      box-shadow: 0 1px 4px rgba(0,0,0,0.1);
    }
    header h1 {
      font-size: 2.5rem;
      font-weight: bold;
      margin: 0;
    }
    header p {
      margin-top: 0.5rem;
      font-size: 1.125rem;
    }
    main {
      display: flex;
      flex-direction: column;
      gap: 2rem;
      padding: 1.5rem;
      max-width: 1000px;
      margin: auto;
    }
    @media (min-width: 1024px) {
      main {
        flex-direction: row;
      }
    }
    .section {
      flex: 1;
    }
    h2 {
      font-size: 1.5rem;
      font-weight: 600;
    }
    ul {
      list-style: disc inside;
      margin: 1rem 0;
      padding: 0;
    }
    .card {
      background-color: white;
      padding: 1.5rem;
      box-shadow: 0 4px 8px rgba(0,0,0,0.05);
      border-radius: 0.5rem;
      font-size: 0.9rem;
      color: #374151;
    }
    .contact-info p {
      margin: 0.5rem 0;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }
    .section img {
      width: 100%;
      border-radius: 1rem;
      box-shadow: 0 8px 16px rgba(0,0,0,0.1);
    }
    footer {
      text-align: center;
      padding: 1rem;
      font-size: 0.875rem;
      color: #6b7280;
      background-color: white;
      border-top: 1px solid #e5e7eb;
    }
  </style>
</head>
<body>
  <header>
    <h1>Bar Exam Mastery</h1>
    <p>One-on-one tutoring to help you pass with confidence</p>
  </header>

  <main>
    <section class="section">
      <h2>Why Choose Me?</h2>
      <ul>
        <li>Former bar exam grader and licensed attorney</li>
        <li>Tailored study plans for your learning style</li>
        <li>Flexible scheduling with Zoom or in-person sessions</li>
        <li>Extensive MBE and essay preparation strategies</li>
      </ul>

      <div class="card contact-info">
        <h3>Contact Information</h3>
        <p>📧 tutor@example.com</p>
        <p>📞 (123) 456-7890</p>
      </div>
    </section>

    <section class="section">
      <img src="https://images.unsplash.com/photo-1581092160613-eb7f28c7b1ef?fit=crop&w=800&q=80" alt="Studying for bar exam" />
    </section>
  </main>

  <footer>
    &copy; <span id="year"></span> Bar Exam Mastery. All rights reserved.
  </footer>

  <script>
    document.getElementById(\"year\").textContent = new Date().getFullYear();
  </script>
</body>
</html>

