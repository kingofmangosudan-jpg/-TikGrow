n# -TikGrow
TikGrow    MVP
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TikGrow - زيادة المتابعين</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f5f6fa;
      color: #222;
    }

    .header {
      background: #111;
      color: white;
      padding: 20px;
      text-align: center;
    }

    .header h1 {
      font-size: 30px;
    }

    .header p {
      margin-top: 8px;
      color: #ccc;
    }

    .container {
      max-width: 500px;
      margin: 30px auto;
      padding: 20px;
    }

    .card {
      background: white;
      border-radius: 18px;
      padding: 25px;
      box-shadow: 0 5px 20px rgba(0,0,0,0.08);
      margin-bottom: 20px;
    }

    .card h2 {
      margin-bottom: 15px;
      text-align: center;
    }

    input {
      width: 100%;
      padding: 15px;
      border: 1px solid #ddd;
      border-radius: 12px;
      margin-bottom: 15px;
      font-size: 16px;
      direction: ltr;
    }

    button {
      width: 100%;
      padding: 15px;
      border: none;
      border-radius: 12px;
      background: #111;
      color: white;
      font-size: 17px;
      cursor: pointer;
    }

    button:hover {
      opacity: 0.9;
    }

    .points {
      text-align: center;
      font-size: 25px;
      font-weight: bold;
      margin: 15px 0;
    }

    .status {
      text-align: center;
      margin-top: 15px;
      color: #555;
    }

    .footer {
      text-align: center;
      padding: 25px;
      color: #777;
      font-size: 14px;
    }
  </style>
</head>

<body>

  <div class="header">
    <h1>🚀 TikGrow</h1>
    <p>منصة نمو وتفاعل لحسابات تيك توك</p>
  </div>

  <div class="container">

    <div class="card">
      <h2>👤 حسابك</h2>

      <input
        type="text"
        id="username"
        placeholder="@username"
      >

      <button onclick="startGrow()">
        ابدأ الآن
      </button>

      <div class="status" id="status">
        أدخل اسم مستخدم تيك توك للبدء
      </div>
    </div>

    <div class="card">
      <h2>⭐ نقاطك</h2>

      <div class="points" id="points">
        100
      </div>

      <p style="text-align:center;">
        نقطة
      </p>
    </div>

    <div class="card">
      <h2>📈 نظام TikGrow</h2>

      <p style="line-height:1.8; text-align:center;">
        اكسب النقاط من خلال التفاعل،
        ثم استخدم نقاطك للحصول على خدمات النمو.
      </p>
    </div>

  </div>

  <div class="footer">
    TikGrow MVP © 2026
  </div>

  <script>
    function startGrow() {

      const username =
        document.getElementById("username").value.trim();

      const status =
        document.getElementById("status");

      if (username === "") {
        status.innerText =
          "⚠️ اكتب اسم مستخدم تيك توك أولاً";
        return;
      }

      status.innerText =
        "✅ تم تسجيل الحساب: " + username;

    }
  </script>

</body>
</html>