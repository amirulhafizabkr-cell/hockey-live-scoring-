<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hockey Live Scoring</title>

  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f4f6f8;
      color: #222;
    }

    header {
      background: #111827;
      color: white;
      padding: 20px;
      text-align: center;
    }

    header h1 {
      margin: 0;
      font-size: 28px;
    }

    header p {
      margin: 8px 0 0;
      color: #d1d5db;
    }

    .container {
      max-width: 1100px;
      margin: auto;
      padding: 20px;
    }

    .section-title {
      margin-top: 30px;
      margin-bottom: 15px;
      font-size: 22px;
      border-left: 5px solid #111827;
      padding-left: 10px;
    }

    .live-card {
      background: white;
      border-radius: 12px;
      padding: 20px;
      margin-bottom: 15px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.08);
    }

    .match-status {
      display: inline-block;
      background: #dc2626;
      color: white;
      padding: 5px 10px;
      border-radius: 20px;
      font-size: 13px;
      margin-bottom: 15px;
    }

    .score-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 15px;
    }

    .team {
      width: 40%;
      font-size: 22px;
      font-weight: bold;
      text-align: center;
    }

    .score {
      width: 20%;
      text-align: center;
      font-size: 36px;
      font-weight: bold;
    }

    .info {
      margin-top: 15px;
      text-align: center;
      color: #555;
      font-size: 14px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 15px;
    }

    .small-card {
      background: white;
      border-radius: 12px;
      padding: 15px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.08);
    }

    .small-card h3 {
      margin-top: 0;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      background: white;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 2px 8px rgba(0,0,0,0.08);
    }

    th, td {
      padding: 12px;
      border-bottom: 1px solid #e5e7eb;
      text-align: left;
    }

    th {
      background: #111827;
      color: white;
    }

    footer {
      text-align: center;
      padding: 20px;
      margin-top: 30px;
      color: #666;
    }

    @media (max-width: 600px) {
      .score-row {
        flex-direction: column;
      }

      .team, .score {
        width: 100%;
      }

      .score {
        font-size: 32px;
      }
    }
  </style>
</head>

<body>

  <header>
    <h1>Hockey Live Scoring</h1>
    <p>2-Day Hockey Tournament | 96 Teams</p>
  </header>

  <div class="container">

    <h2 class="section-title">Live Match</h2>

    <div class="live-card">
      <div class="match-status">LIVE</div>

      <div class="score-row">
        <div class="team">Team A</div>
        <div class="score">0 - 0</div>
        <div class="team">Team B</div>
      </div>

      <div class="info">
        Category: Under 10 Boys | Field 1 | Match 1
      </div>
    </div>

    <h2 class="section-title">Upcoming Matches</h2>

    <div class="grid">
      <div class="small-card">
        <h3>Match 2</h3>
        <p>Team C vs Team D</p>
        <p>Time: 9:30 AM</p>
        <p>Field: 1</p>
      </div>

      <div class="small-card">
        <h3>Match 3</h3>
        <p>Team E vs Team F</p>
        <p>Time: 10:00 AM</p>
        <p>Field: 2</p>
      </div>

      <div class="small-card">
        <h3>Match 4</h3>
        <p>Team G vs Team H</p>
        <p>Time: 10:30 AM</p>
        <p>Field: 1</p>
      </div>
    </div>

    <h2 class="section-title">Top Scorer</h2>

    <table>
      <thead>
        <tr>
          <th>Rank</th>
          <th>Player</th>
          <th>Team</th>
          <th>Goals</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1</td>
          <td>No scorer yet</td>
          <td>-</td>
          <td>0</td>
        </tr>
      </tbody>
    </table>

  </div>

  <footer>
    Hockey Live Scoring Website
  </footer>

</body>
</html>
