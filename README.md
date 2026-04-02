<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>SCT HelpChain Admin | H R Antor</title>
    <style>
        body { background: #020617; color: #38bdf8; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; text-align: center; padding: 20px; }
        .dashboard { border: 2px solid #38bdf8; max-width: 600px; margin: auto; padding: 30px; border-radius: 20px; box-shadow: 0 0 30px rgba(56, 189, 248, 0.3); background: #0f172a; }
        .btn { background: #38bdf8; color: #020617; padding: 12px 25px; border: none; cursor: pointer; font-weight: bold; border-radius: 8px; margin: 10px; width: 80%; transition: 0.3s; }
        .btn:hover { background: #7dd3fc; transform: scale(1.05); }
        input { padding: 12px; border-radius: 8px; border: 1px solid #38bdf8; background: #1e293b; color: white; width: 80%; margin-bottom: 15px; text-align: center; }
        .wallet-box { background: #1e293b; padding: 15px; border-radius: 10px; margin-top: 20px; border-left: 5px solid #4ade80; }
    </style>
</head>
<body>

    <div class="dashboard">
        <h1>🛡️ SCT HELPCHAIN</h1>
        <h3>Admin Dashboard: H R Antor</h3>
        <p>Assistant Editor (Crime) | Mathematics Developer</p>
        
        <hr style="border: 0.1px solid #334155;">

        <h3>🔐 Access Control</h3>
        <input type="password" id="adminPass" placeholder="Enter Admin Pin (e.g. 1234)">

        <div class="wallet-box">
            <h3>💎 Payment Gateway</h3>
            <p>Wallet: <span style="color:#4ade80">0xf5d3C...9bb89</span></p>
            <input type="text" id="target" placeholder="Recipient Address">
            <input type="number" id="amt" placeholder="Amount (BNB/Polygon)">
            <button class="btn" onclick="process()">🚀 SEND PAYMENT</button>
            <button class="btn" onclick="alert('Address Copied: 0xf5d3C0E5e1B0F89bB89...')">📥 RECEIVE PAYMENT</button>
        </div>

        <p style="font-size: 10px; margin-top: 20px;">System Secure | Gematria Logic Active</p>
    </div>

    <script>
        function process() {
            const pin = document.getElementById('adminPass').value;
            if(pin === "1234") { // এটি আপনার গোপন পাসওয়ার্ড, চাইলে বদলাতে পারেন
                alert("Authorization Successful! Connecting MetaMask...");
            } else {
                alert("🚨 Access Denied! Security Soldiers are Watching!");
            }
        }
    </script>
</body>
</html>
