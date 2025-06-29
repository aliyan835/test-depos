<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Tıklama Canavarı</title>
  <style>
    body {
      font-family: sans-serif;
      text-align: center;
      margin-top: 100px;
      background: #f0f0f0;
    }
    h1 {
      font-size: 2.5rem;
    }
    #puan {
      font-size: 3rem;
      color: #0077cc;
    }
    #buton {
      padding: 20px 40px;
      font-size: 1.5rem;
      margin-top: 30px;
      background: #0077cc;
      color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }
    #buton:hover {
      background: #005fa3;
    }
  </style>
</head>
<body>
  <h1>Tıklama Canavarı</h1>
  <div>Puanın: <span id="puan">0</span></div>
  <button id="buton">Tıkla Bakalım!</button>

  <script>
    let puan = 0;
    const puanAlani = document.getElementById('puan');
    const buton = document.getElementById('buton');

    buton.addEventListener('click', () => {
      puan++;
      puanAlani.textContent = puan;

      if (puan === 10) {
        alert("10 puan! Parmak ısındı 🔥");
      } else if (puan === 50) {
        alert("50 oldu! Mouse yandı 😱");
      } else if (puan === 100) {
        alert("100 puan! Tıklama efsanesi oldun! 👑");
      }
    });
  </script>
</body>
</html>
