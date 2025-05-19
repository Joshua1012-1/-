<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>계좌번호 복사</title>
  <style>
    button {
      font-size: 16px;
      padding: 10px 20px;
      border-radius: 8px;
      border: none;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <p id="account">123456-78-901234</p>
  <button onclick="copyText()">계좌번호 복사</button>

  <script>
    function copyText() {
      const text = document.getElementById("account").innerText;
      navigator.clipboard.writeText(text).then(() => {
        alert("복사되었습니다!");
      });
    }
  </script>
</body>
</html>
