<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Gay Test</title>
  <style>
    body { font-family: Arial, sans-serif; text-align: center; margin-top: 100px; background: #e0e7ff; }
    .hidden { display: none; }
    button { margin: 12px; padding: 10px 20px; font-size: 18px; border-radius: 7px; border: none; background: #6366f1; color: #fff; cursor: pointer; }
    button:hover { background: #818cf8; }
    #diagnosing { font-size: 24px; margin-bottom: 40px; }
    #main-menu { font-size: 40px; margin-bottom: 40px; }
    #backBtn { margin-top: 30px; background: #475569; }
  </style>
</head>
<body>
  <div id="main-menu">
    Gay Test
    <br>
    <button onclick="startTest()">Start</button>
  </div>

  <div id="question" class="hidden">
    <h1>Are You Gay?</h1>
    <button onclick="diagnose('yes')">Yes</button>
    <button onclick="diagnose('no')">No</button>
    <br>
    <button id="backBtn" onclick="backToMenu()">Return to Main Menu</button>
  </div>

  <div id="diagnosing" class="hidden">
    Diagnosing...
    <br>
    <img src="https://media.giphy.com/media/3o85xIO33l7RlmLR4I/giphy.gif" alt="Loading" width="80">
  </div>

  <div id="areYouSure" class="hidden">
    <h1>Are you sure?</h1>
    <button onclick="sureDiagnose('yes')">Yes</button>
    <button onclick="sureDiagnose('no')">No</button>
    <br>
    <button id="backBtn" onclick="backToMenu()">Return to Main Menu</button>
  </div>

  <script>
    function hideAll() {
      document.getElementById('main-menu').classList.add('hidden');
      document.getElementById('question').classList.add('hidden');
      document.getElementById('diagnosing').classList.add('hidden');
      document.getElementById('areYouSure').classList.add('hidden');
    }

    function startTest() {
      hideAll();
      document.getElementById('question').classList.remove('hidden');
    }

    function diagnose(answer) {
      hideAll();
      document.getElementById('diagnosing').classList.remove('hidden');
      setTimeout(function() {
        hideAll();
        if(answer === 'yes') {
          alert('Results: You are Gay.');
          backToMenu();
        } else {
          document.getElementById('areYouSure').classList.remove('hidden');
        }
      }, 2000);
    }

    function sureDiagnose(answer) {
      hideAll();
      document.getElementById('diagnosing').classList.remove('hidden');
      setTimeout(function() {
        hideAll();
        if(answer === 'yes') {
          alert('Results: You are most likely not gay.');
          backToMenu();
        } else {
          alert('Results: There is a 30% chance you are gay.');
          backToMenu();
        }
      }, 2000);
    }

    function backToMenu() {
      hideAll();
      document.getElementById('main-menu').classList.remove('hidden');
    }

    // Start at main menu
    backToMenu();
  </script>
</body>
</html>
