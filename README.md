# Rework
This repo is used to test beta version of vendetta themes created by me. 
<!DOCTYPE html>
<html>
<head>
  <title>GitHub README Popup Example</title>
  <style>
    /* Styling for the popup container */
    .popup-container {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.5);
    }

    /* Styling for the popup box */
    .popup-box {
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: #fff;
      padding: 20px;
      border-radius: 5px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
    }

    /* Styling for the close button */
    .popup-close {
      position: absolute;
      top: 10px;
      right: 10px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <h1>GitHub README Popup Example</h1>
  <p>Click the button below to open the popup.</p>
  <!-- Button to trigger the popup -->
  <button id="popupButton">Open Popup</button>

  <!-- Popup container -->
  <div class="popup-container" id="popupContainer">
    <!-- Popup box -->
    <div class="popup-box">
      <!-- Close button -->
      <span class="popup-close" id="popupClose">&times;</span>
      <h2>This is a Popup</h2>
      <p>This is some content inside the popup.</p>
    </div>
  </div>

  <!-- JavaScript to handle the popup functionality -->
  <script>
    const popupButton = document.getElementById('popupButton');
    const popupContainer = document.getElementById('popupContainer');
    const popupClose = document.getElementById('popupClose');

    popupButton.addEventListener('click', () => {
      popupContainer.style.display = 'block';
    });

    popupClose.addEventListener('click', () => {
      popupContainer.style.display = 'none';
    });
  </script>
</body>
</html>
