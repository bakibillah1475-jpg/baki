<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Material Price Calculator</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
    }

    body{
      font-family: Inter, Arial, sans-serif;
      background:#eef2f7;
      min-height:100vh;
      display:flex;
      align-items:center;
      justify-content:center;
      padding:40px 20px;
      color:#111827;
    }

    .calculator{
      width:100%;
      max-width:900px;
      background:#ffffff;
      border-radius:24px;
      overflow:hidden;
      box-shadow:
      0 10px 25px rgba(0,0,0,0.08),
      0 2px 8px rgba(0,0,0,0.04);
    }

    .top-section{
      background:linear-gradient(135deg,#0f172a,#1e293b);
      padding:35px;
      color:white;
    }

    .top-section h1{
      font-size:32px;
      font-weight:700;
      margin-bottom:10px;
    }

    .top-section p{
      color:rgba(255,255,255,0.8);
      font-size:15px;
      line-height:1.6;
    }

    .content{
      padding:35px;
    }

    .grid{
      display:grid;
      grid-template-columns:repeat(2,1fr);
      gap:24px;
    }

    .input-group{
      display:flex;
      flex-direction:column;
    }

    .full{
      grid-column:1/-1;
    }

    label{
      margin-bottom:10px;
      font-size:14px;
      font-weight:600;
      color:#374151;
    }

    input,
    select{
      height:54px;
      border:1px solid #d1d5db;
      border-radius:14px;
      padding:0 16px;
      font-size:16px;
      transition:0.2s;
      background:white;
    }

    input:focus,
    select:focus{
      outline:none;
      border-color:#2563eb;
      box-shadow:0 0 0 4px rgba(37,99,235,0.12);
    }

    .locked{
      background:#f3f4f6;
      color:#6b7280;
      font-weight:700;
      cursor:not-allowed;
    }

    .calculate-btn{
      width:100%;
      height:58px;
      border:none;
      border-radius:16px;
      background:#2563eb;
      color:white;
      font-size:17px;
      font-weight:600;
      margin-top:35px;
      cursor:pointer;
      transition:0.25s;
    }

    .calculate-btn:hover{
      transform:translateY(-2px);
      background:#1d4ed8;
    }

    .results{
      margin-top:35px;
      background:#f8fafc;
      border:1px solid #e5e7eb;
      border-radius:22px;
      padding:28px;
    }

    .results h2{
      font-size:24px;
      margin-bottom:24px;
    }

    .result-grid{
      display:grid;
      grid-template-columns:repeat(2,1fr);
      gap:18px;
    }

    .card{
      background:white;
      border-radius:18px;
      padding:22px;
      border:1px solid #e5e7eb;
    }

    .card span{
      display:block;
      font-size:13px;
      color:#6b7280;
      margin-bottom:10px;
    }

    .card h3{
      font-size:26px;
      color:#111827;
      font-weight:700;
    }

    .final-card{
      background:#2563eb;
      color:white;
      border:none;
    }

    .final-card span{
      color:rgba(255,255,255,0.8);
    }

    .final-card h3{
      color:white;
    }

    @media(max-width:768px){

      .grid,
      .result-grid{
        grid-template-columns:1fr;
      }

      .top-section h1{
        font-size:26px;
      }

      .content{
        padding:24px;
      }

    }

  </style>
</head>
<body>

<div class="calculator">

  <div class="top-section">
    <h1>Material Price Calculator</h1>
    <p>
      Calculate quantity in PC, material price, color cost,
      adhesive cost, and final per-piece price automatically.
    </p>
  </div>

  <div class="content">

    <div class="grid">

      <div class="input-group full">
        <label>Measurement Unit</label>

        <select id="unit">
          <option value="inch">Inch</option>
          <option value="cm">CM</option>
          <option value="meter">Meter</option>
        </select>
      </div>

      <div class="input-group">
        <label>Locked Value</label>
        <input type="number" value="75000" readonly class="locked">
      </div>

      <div class="input-group">
        <label>Thickness (MM)</label>
        <input type="number" id="thickness" placeholder="Enter thickness">
      </div>

      <div class="input-group">
        <label>Height</label>
        <input type="number" id="height" placeholder="Enter height">
      </div>

      <div class="input-group">
        <label>Weight</label>
        <input type="number" id="weight" placeholder="Enter weight">
      </div>

      <div class="input-group">
        <label>Pound Price</label>
        <input type="number" id="poundPrice" placeholder="Enter pound price">
      </div>

      <div class="input-group">
        <label>Number of Colors</label>
        <input type="number" id="colors" placeholder="Enter color quantity">
      </div>

    </div>

    <button class="calculate-btn" onclick="calculateResult()">
      Calculate Price
    </button>

    <div class="results">

      <h2>Calculation Result</h2>

      <div class="result-grid">

        <div class="card">
          <span>Quantity</span>
          <h3 id="quantity">0 PC</h3>
        </div>

        <div class="card">
          <span>Per PC Material Price</span>
          <h3 id="materialPrice">0 Tk</h3>
        </div>

        <div class="card">
          <span>Color Cost</span>
          <h3 id="colorCost">0 Tk</h3>
        </div>

        <div class="card">
          <span>Adhesive Cost</span>
          <h3 id="adhesiveCost">0 Tk</h3>
        </div>

        <div class="card final-card full">
          <span>Final Per PC Price</span>
          <h3 id="finalPrice">0 Tk</h3>
        </div>

      </div>

    </div>

  </div>

</div>

<script>

  function convertToInch(value, unit){

    if(unit === "cm"){
      return value / 2.54;
    }

    if(unit === "meter"){
      return value * 39.3701;
    }

    return value;
  }

  function calculateResult(){

    const unit = document.getElementById("unit").value;

    let height =
      parseFloat(document.getElementById("height").value) || 0;

    let weight =
      parseFloat(document.getElementById("weight").value) || 0;

    let thickness =
      parseFloat(document.getElementById("thickness").value) || 0;

    let poundPrice =
      parseFloat(document.getElementById("poundPrice").value) || 0;

    let colors =
      parseFloat(document.getElementById("colors").value) || 0;

    // Auto convert to inch
    height = convertToInch(height, unit);
    weight = convertToInch(weight, unit);

    // Quantity Formula
    const quantity =
      75000 / height / weight / thickness;

    // Material Price Per PC
    const materialPrice =
      poundPrice / quantity;

    // Color Cost
    const colorCost =
      colors * 0.15;

    // Adhesive Cost
    const adhesiveCost =
      weight * 0.2;

    // Final Price
    const finalPrice =
      materialPrice +
      colorCost +
      adhesiveCost;

    // Output
    document.getElementById("quantity").innerHTML =
      quantity.toFixed(2) + " PC";

    document.getElementById("materialPrice").innerHTML =
      materialPrice.toFixed(4) + " Tk";

    document.getElementById("colorCost").innerHTML =
      colorCost.toFixed(4) + " Tk";

    document.getElementById("adhesiveCost").innerHTML =
      adhesiveCost.toFixed(4) + " Tk";

    document.getElementById("finalPrice").innerHTML =
      finalPrice.toFixed(4) + " Tk";
  }

</script>

</body>
</html>
