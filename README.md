body {
  margin: 0;
  font-family: sans-serif;
  height: 100vh;
  display: flex;
  flex-direction: row;
}

.controls {
  width: 40%;
  padding: 15px;
  overflow-y: auto;
  background: #f9f9f9;
}

#map {
  width: 60%;
  height: 100%;
}

/* Inputs & Buttons */
input,
button,
select,
textarea {
  margin: 5px 0;
  padding: 10px;
  width: 100%;
  border-radius: 6px;
  border: 1px solid #ccc;
  box-sizing: border-box;
}

button {
  background: #4CAF50;
  color: white;
  border: none;
  font-size: 16px;
  cursor: pointer;
}

button:hover {
  opacity: 0.8;
}

.chat-box {
  height: 120px;
  overflow-y: auto;
  padding: 10px;
  border: 1px solid #ccc;
  background: #eee;
}

.vehicle-list {
  display: flex;
  gap: 10px;
}

.vehicle {
  flex: 1;
  padding: 10px;
  text-align: center;
  border: 1px solid #333;
  border-radius: 6px;
  cursor: pointer;
  background: white;
}

.vehicle.active {
  background: #4CAF50;
  color: white;
}

/* MOBILE RESPONSIVE */
@media (max-width: 768px) {

  body {
    flex-direction: column;
  }

  .controls {
    width: 100%;
    height: 55vh;
  }

  #map {
    width: 100%;
    height: 45vh;
  }

  .vehicle {
    flex: 0 0 48%;
  }

  h2, h3 {
    font-size: 18px;
  }
}
