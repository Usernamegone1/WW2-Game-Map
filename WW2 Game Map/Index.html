<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>WWII Strategy Game - Battlefront Command</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #eef3f7;
      margin: 0;
      padding: 0;
    }
    h1 {
      text-align: center;
      color: #2c3e50;
      margin-top: 10px;
    }
    .map-container {
      position: relative;
      max-width: 1000px;
      margin: 0 auto;
    }
    .map-container img {
      width: 100%;
      border: 3px solid #2c3e50;
      border-radius: 10px;
    }
    .controls, .dice-roll, .log {
      max-width: 1000px;
      margin: 20px auto;
      text-align: center;
    }
    button {
      margin: 6px;
      padding: 10px 18px;
      font-size: 16px;
      border-radius: 5px;
      background-color: #3498db;
      color: white;
      border: none;
      cursor: pointer;
    }
    button:hover {
      background-color: #2980b9;
    }
    .log {
      background: #fff;
      padding: 10px;
      height: 200px;
      overflow-y: auto;
      border: 2px solid #ccc;
    }
    #dice {
      width: 70px;
      height: 70px;
      line-height: 70px;
      border-radius: 10px;
      background: #fff;
      font-size: 36px;
      font-weight: bold;
      display: inline-block;
      margin: 10px;
      border: 3px solid #2c3e50;
      cursor: pointer;
      user-select: none;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }
    .flags {
      text-align: center;
      margin-top: 10px;
    }
    .flags img {
      height: 32px;
      margin: 0 10px;
    }
  </style>
</head>
<body>
  <h1>Battlefront Command - WWII Strategy Game</h1>
  <div class="flags">
    <img src="https://flagcdn.com/de.svg" alt="Germany">
    <img src="https://flagcdn.com/fr.svg" alt="France">
    <img src="https://flagcdn.com/gb.svg" alt="UK">
    <img src="https://flagcdn.com/ru.svg" alt="Russia">
    <img src="https://flagcdn.com/us.svg" alt="USA">
  </div>

  <div class="map-container">
    <img src="https://upload.wikimedia.org/wikipedia/commons/e/e9/WWII_Europe_Map_1941.jpg" alt="WWII Europe Map" usemap="#ww2map">
    <map name="ww2map">
      <area shape="rect" coords="420,150,480,200" href="#" alt="Berlin" onclick="selectRegion('Berlin'); return false;">
      <area shape="rect" coords="200,220,260,260" href="#" alt="London" onclick="selectRegion('London'); return false;">
      <area shape="rect" coords="250,250,310,290" href="#" alt="Paris" onclick="selectRegion('Paris'); return false;">
      <area shape="rect" coords="320,300,380,340" href="#" alt="Rome" onclick="selectRegion('Rome'); return false;">
      <area shape="rect" coords="480,180,540,220" href="#" alt="Warsaw" onclick="selectRegion('Warsaw'); return false;">
    </map>
  </div>

  <div class="controls">
    <button onclick="setUnit('Infantry')">Infantry</button>
    <button onclick="setUnit('Tank')">Tank</button>
    <button onclick="setUnit('Air Force')">Air Force</button>
    <button onclick="setUnit('Navy')">Navy</button>
  </div>

  <div class="dice-roll">
    <div id="dice" onclick="rollDice()">🎲</div>
    <p id="dice-result">Click the dice to roll your attack</p>
  </div>

  <div class="log" id="log"></div>

  <script>
    let selectedRegion = null;
    let selectedUnit = null;
    let currentModifier = 0;
    const conqueredRegions = {};

    const modifiers = {
      "Infantry": 0,
      "Tank": 2,
      "Air Force": 1,
      "Navy": 2
    };

    function selectRegion(region) {
      if (conqueredRegions[region]) {
        log(`${region} is already conquered!`);
        return;
      }
      selectedRegion = region;
      log(`Selected region: ${region}`);
    }

    function setUnit(unit) {
      selectedUnit = unit;
      currentModifier = modifiers[unit];
      log(`Selected unit: ${unit} (Modifier: +${currentModifier})`);
    }

    function rollDice() {
      if (!selectedRegion || !selectedUnit) {
        log("Please select both a unit and a region first.");
        return;
      }
      const roll = Math.floor(Math.random() * 6) + 1;
      const total = roll + currentModifier;
      document.getElementById("dice-result").innerText = `Roll: ${roll} + ${currentModifier} = ${total}`;

      const defenderRoll = Math.floor(Math.random() * 6) + 1;
      const success = total > defenderRoll;

      const outcome = success
        ? `✔️ Success! ${selectedUnit} defeats enemy in ${selectedRegion} (Defender rolled ${defenderRoll})`
        : `❌ Failed! ${selectedUnit} couldn't break through in ${selectedRegion} (Defender rolled ${defenderRoll})`;

      if (success) {
        conqueredRegions[selectedRegion] = true;
        highlightRegion(selectedRegion);
      }

      log(outcome);
    }

    function highlightRegion(regionName) {
      log(`${regionName} has been conquered!`);
    }

    function log(message) {
      const logEl = document.getElementById('log');
      const time = new Date().toLocaleTimeString();
      logEl.innerHTML += `[${time}] ${message}<br>`;
      logEl.scrollTop = logEl.scrollHeight;
    }
  </script>
</body>
</html>
