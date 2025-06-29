<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Phxm Access</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #0b1320;
      color: #ffffff;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
  
    .container {
      background: #101d34;
      border-radius: 20px;
      padding: 30px 25px;
      width: 350px;
      box-shadow: 0 0 25px rgba(0, 255, 255, 0.1);
      text-align: center;
    }

    .title {
      color: #00ccff;
      font-size: 22px;
      font-weight: bold;
    }

    .subtitle {
      font-size: 12px;
      color: #cccccc;
      margin-top: 4px;
      margin-bottom: 25px;
    }

    .device-id {
      font-family: monospace;
      background: #0f1a2f;
      padding: 12px;
      border-radius: 10px;
      margin: 15px 0;
      display: inline-block;
      letter-spacing: 1px;
    }

    .copy-btn {
      background: #00ccff;
      color: #000;
      border: none;
      padding: 10px 16px;
      border-radius: 10px;
      cursor: pointer;
      font-weight: bold;
      margin-bottom: 20px;
      transition: background 0.3s ease;
    }

    .copy-btn:hover {
      background: #00b4e6;
    }

    .status {
      background: #2c2c2c;
      color: #ffcc00;
      padding: 8px 14px;
      border-radius: 8px;
      margin-bottom: 25px;
      font-size: 13px;
    }

    .instructions {
      text-align: left;
      font-size: 13px;
      color: #bbbbbb;
      margin-top: 10px;
    }

    .instructions strong {
      color: #ffffff;
    }

    .footer {
      margin-top: 30px;
      font-size: 11px;
      color: #666666;
    }
  </style>
</head>
<body>

  <div class="container">
    <div class="title">Phxm owner</div>
    <div class="subtitle">Secure Device Authentication</div>

    <div><strong>🔒 Your Device ID</strong></div>
    <div class="device-id" id="deviceId">EB4F-4GQG-0ALR-V33D</div>

    <button class="copy-btn" onclick="copyDeviceId()">📋 Copy Device ID</button>

    <div class="status">⏳ WAITING FOR ADMIN APPROVAL</div>

    <div class="instructions">
      <p><strong>How to use this ID:</strong></p>
      <ol>
        <li>Click "Copy Device ID" button above</li>
        <li>Go to Owner <strong>@phxm_owner</strong></li>
      </ol>
      <p>Contact owner directly after copying your device ID</p>
    </div>

    <div class="footer">PHXM SECURE ACCESS SYSTEM © 2023</div>
  </div>

  <script>
    function copyDeviceId() {
      const text = document.getElementById("deviceId").textContent;
      navigator.clipboard.writeText(text).then(() => {
        alert("Device ID copied to clipboard!");
      });
    }
  </script>

</body>
</html>
