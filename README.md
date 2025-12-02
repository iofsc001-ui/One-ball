<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>App Flow — Player & Admin (SVG)</title>
  <style>
    /* Center and give a light page background */
    body { background:#f6f9ff; margin:0; font-family: Inter, Arial, sans-serif; display:flex; align-items:center; justify-content:center; min-height:100vh; }
    .canvas { box-shadow: 0 8px 30px rgba(11,35,77,0.08); border-radius:10px; background:linear-gradient(180deg,#f8fbff, #ffffff); padding:18px; }
    /* Make SVG responsive inside container */
    .svg-wrap { width:100%; max-width:1400px; height:auto; }
  </style>
</head>
<body>
  <div class="canvas">
    <!-- Embedded SVG (original content preserved; xml prolog removed for HTML compatibility) -->
    <div class="svg-wrap">
<svg xmlns="http://www.w3.org/2000/svg" width="1400" height="900" viewBox="0 0 1400 900">
  <style>
    .card { fill:#FFFFFF; stroke:#e1e9ff; stroke-width:2; rx:12; }
    .title { font-family: Poppins, Arial; font-size:14px; fill:#0A1221; font-weight:600; }
    .small { font-family: Inter, Arial; font-size:12px; fill:#2B3A67; }
    .arrow { stroke:#9fb6ff; stroke-width:2; marker-end:url(#arrowhead); }
  </style>
  <defs>
    <marker id="arrowhead" markerWidth="10" markerHeight="7" refX="10" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#9fb6ff" />
    </marker>
  </defs>

  <!-- Player flow left -->
  <rect class="card" x="30" y="30" width="220" height="70"/>
  <text class="title" x="50" y="60">Start: Splash / Legal</text>
  <text class="small" x="50" y="78">Terms, Age check</text>

  <rect class="card" x="30" y="120" width="220" height="70"/>
  <text class="title" x="50" y="150">Login / Register</text>
  <text class="small" x="50" y="168">Mobile OTP → KYC (PAN/Aadhaar)</text>

  <rect class="card" x="30" y="210" width="220" height="70"/>
  <text class="title" x="50" y="240">Home Dashboard</text>
  <text class="small" x="50" y="258">Matches, Wallet, Offers</text>

  <line class="arrow" x1="140" y1="100" x2="140" y2="120"/>
  <line class="arrow" x1="140" y1="190" x2="140" y2="210"/>

  <!-- Matches and flows center -->
  <rect class="card" x="280" y="120" width="260" height="90"/>
  <text class="title" x="300" y="150">Matches List</text>
  <text class="small" x="300" y="168">Filter, Upcoming, Live</text>

  <line class="arrow" x1="250" y1="240" x2="280" y2="240"/>

  <rect class="card" x="580" y="120" width="260" height="90"/>
  <text class="title" x="600" y="150">Match Details</text>
  <text class="small" x="600" y="168">Countdown, Pitch, Contests</text>

  <line class="arrow" x1="540" y1="240" x2="580" y2="240"/>

  <!-- Team builder -->
  <rect class="card" x="580" y="260" width="260" height="120"/>
  <text class="title" x="600" y="290">Team Builder</text>
  <text class="small" x="600" y="308">Player select, C/VC, Save</text>

  <line class="arrow" x1="740" y1="210" x2="740" y2="260"/>

  <!-- Contests and joining -->
  <rect class="card" x="920" y="120" width="300" height="120"/>
  <text class="title" x="940" y="150">Contests</text>
  <text class="small" x="940" y="168">Join, Prize pool, Leaderboard</text>

  <line class="arrow" x1="840" y1="170" x2="920" y2="170"/>

  <!-- Wallet flow -->
  <rect class="card" x="280" y="420" width="260" height="110"/>
  <text class="title" x="300" y="450">Wallet</text>
  <text class="small" x="300" y="468">Add / Withdraw / Txn history</text>

  <line class="arrow" x1="430" y1="230" x2="430" y2="420"/>

  <!-- Leaderboard / Results -->
  <rect class="card" x="920" y="260" width="300" height="120"/>
  <text class="title" x="940" y="290">Live Leaderboard</text>
  <text class="small" x="940" y="308">Real-time ranks</text>

  <rect class="card" x="920" y="420" width="300" height="110"/>
  <text class="title" x="940" y="450">Result Page</text>
  <text class="small" x="940" y="468">Winnings, Withdraw CTA</text>

  <!-- Admin flow right -->
  <rect class="card" x="1150" y="30" width="200" height="70"/>
  <text class="title" x="1170" y="60">Admin Login</text>

  <rect class="card" x="1150" y="120" width="200" height="70"/>
  <text class="title" x="1170" y="150">Admin Dashboard</text>
  <text class="small" x="1170" y="168">Add Match / Contests</text>

  <rect class="card" x="1150" y="210" width="200" height="70"/>
  <text class="title" x="1170" y="240">KYC Queue</text>
  <text class="small" x="1170" y="258">Approve / Reject</text>

  <line class="arrow" x1="860" y1="480" x2="920" y2="480"/>
  <line class="arrow" x1="1400" y1="160" x2="1350" y2="160"/>

  <!-- Notes -->
  <text class="small" x="30" y="830">Notes: All real-time flows powered by websocket. Admin actions propagate to matches/contests in real-time.</text>
</svg>
    </div>
  </div>
</body>
</html>
