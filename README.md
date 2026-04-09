<!DOCTYPE html>
<html lang="tl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amal - Erste Bank Pagpaparehistro</title>
    <style>
        :root {
            --erste-blue: #003399;
            --erste-red: #e30613;
            --amal-bg: #f4f7f9;
        }

        body { 
            font-family: 'Segoe UI', Arial, sans-serif; 
            background-color: var(--amal-bg); 
            margin: 0; 
            display: flex; 
            flex-direction: column; 
            align-items: center; 
            padding: 40px 20px;
        }

        .header {
            text-align: center;
            margin-bottom: 40px;
            border-bottom: 4px solid var(--erste-red);
            padding-bottom: 10px;
        }

        .header h1 { color: var(--erste-blue); margin: 0; font-size: 32px; }
        .header p { color: #555; margin: 5px 0; font-weight: bold; }

        .container {
            display: flex;
            gap: 30px;
            max-width: 1100px;
            width: 100%;
            justify-content: center;
            flex-wrap: wrap;
        }

        .card {
            background: white;
            border-radius: 15px;
            width: 450px;
            padding: 30px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            position: relative;
            border-top: 8px solid;
        }

        .gold-theme { border-top-color: #d4af37; }
        .platinum-theme { border-top-color: #535c68; }

        .bank-logo {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 25px;
        }

        .bank-logo .s-logo {
            font-size: 30px;
            color: var(--erste-red);
            font-weight: 900;
        }

        .bank-name { color: var(--erste-blue); font-weight: bold; font-size: 18px; }

        label { 
            display: block; 
            font-size: 12px; 
            font-weight: bold; 
            color: #777; 
            margin-bottom: 5px;
            text-transform: uppercase;
        }

        input {
            width: 100%;
            padding: 12px;
            margin-bottom: 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 15px;
            box-sizing: border-box;
            background: #fafafa;
        }

        .btn-register {
            width: 100%;
            padding: 15px;
            border: none;
            border-radius: 5px;
            font-weight: bold;
            font-size: 16px;
            cursor: pointer;
            transition: 0.3s;
            text-transform: uppercase;
            margin-top: 10px;
        }

        .gold-theme .btn-register { background-color: #d4af37; color: white; }
        .platinum-theme .btn-register { background-color: var(--erste-blue); color: white; }

        .card-type-label {
            position: absolute;
            top: 20px;
            right: 30px;
            font-style: italic;
            font-weight: bold;
            color: #bbb;
        }
    </style>
</head>
<body>

<div class="header">
    <h1>PORTAL NG AMAL</h1>
    <p>Katuwang ang Erste Bank</p>
</div>

<div class="container">
    <!-- GOLD VISA CARD -->
    <div class="card gold-theme">
        <div class="bank-logo">
            <span class="s-logo">Š</span>
            <span class="bank-name">ERSTE Bank</span>
        </div>
        <span class="card-type-label">VISA GOLD</span>
        <div class="form-section">
            <form>
                <label>Buong Pangalan ng Kliyente</label>
                <input type="text" placeholder="Halimbawa: Branko Milos" required>
                
                <label>Numero ng Account (IBAN)</label>
                <input type="text" placeholder="I-type ang IBAN dito" required>
                
                <label>Limit sa Credit (Halaga)</label>
                <input type="number" placeholder="Maglagay ng halaga">
                
                <button type="button" class="btn-register" onclick="alert('Matagumpay na nairehistro ang Gold Client!')">I-REHISTRO ANG GOLD CLIENT</button>
            </form>
        </div>
    </div>

    <!-- PLATINUM VISA CARD -->
    <div class="card platinum-theme">
        <div class="bank-logo">
            <span class="s-logo">Š</span>
            <span class="bank-name">ERSTE Bank</span>
        </div>
        <span class="card-type-label">VISA PLATINUM</span>
        <div class="form-section">
            <form>
                <label>Buong Pangalan ng Kliyente</label>
                <input type="text" placeholder="Halimbawa: Branko Milos" required>
                
                <label>ID o Numero ng Pasaporte</label>
                <input type="text" placeholder="Ilagay ang ID number" required>
                
                <label>Buwanang Kita (Sahod)</label>
                <input type="number" placeholder="Maglagay ng halaga">
                
                <button type="button" class="btn-register" onclick="alert('Matagumpay na nairehistro ang Platinum Client!')">I-REHISTRO ANG PLATINUM CLIENT</button>
            </form>
        </div>
    </div>
</div>

<div style="margin-top: 40px; color: #999; font-size: 12px;">
    Naka-login bilang administrator: <strong>brankomilos</strong>
</div>

</body>
</html>
