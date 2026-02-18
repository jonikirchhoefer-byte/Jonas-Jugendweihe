# Jonas-Jugendweihe
Jugendweihe Eintrittskarte 
<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Jugendweihe Einladung</title>
  <style>
    body {
      margin: 0;
      font-family: "Segoe UI", sans-serif;
      background: linear-gradient(135deg, #f6d365, #fda085);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #333;
    }
    .card {
      background: white;
      padding: 3rem 2.5rem;
      border-radius: 24px;
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
      text-align: center;
      max-width: 420px;
      width: 90%;
    }
    h1 {
      font-size: 2.2rem;
      margin-bottom: 0.5rem;
    }
    h2 {
      font-weight: 400;
      margin-top: 0;
      color: #666;
    }
    .date {
      font-size: 1.4rem;
      margin: 1.5rem 0 0.5rem;
      font-weight: 600;
    }
    .time {
      font-size: 1.2rem;
      margin-bottom: 2rem;
    }
    .divider {
      width: 60px;
      height: 4px;
      background: #fda085;
      margin: 1.5rem auto;
      border-radius: 2px;
    }
    footer {
      font-size: 0.9rem;
      color: #777;
    }
      .rsvp p {
      margin-bottom: 0.8rem;
      font-weight: 500;
    }
    .rsvp button {
      padding: 0.7rem 1.2rem;
      margin: 0.3rem;
      border: none;
      border-radius: 20px;
      font-size: 1rem;
      cursor: pointer;
      transition: transform 0.1s ease, box-shadow 0.1s ease;
      box-shadow: 0 4px 10px rgba(0,0,0,0.15);
    }
    .rsvp button:hover {
      transform: translateY(-2px);
    }
    .rsvp button.no {
      background: #eee;
      color: #333;
    }
    .rsvp button:not(.no) {
      background: #fda085;
      color: white;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Meine Jugendweihe</h1>
    <h2>Jonas Kirchhöfer</h2>
    <h3>Du bist herzlich eingeladen</h3>

    <div class="divider"></div>

    <div class="date">16. Mai 2026</div>
    <div class="time">Beginn um 15:30 Uhr</div>

    <div class="rsvp">
      <p>Gib mir bitte Bescheid:</p>
      <button onclick="antwort('dabei')">Ich bin dabei</button>
      <button class="no" onclick="antwort('nicht dabei')">Ich bin nicht dabei</button>
    </div>

    <footer>
      Ich freue mich, diesen besonderen Tag mit dir zu feiern ✨
    </footer>
  </div>
  <script>
    function antwort(status) {
      alert('Danke für deine Rückmeldung! Du bist ' + status + '.');
    }
  </script>
</body>
</html>
