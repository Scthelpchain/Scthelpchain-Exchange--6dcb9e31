<!DOCTYPE html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>SCT AI DASHBOARD | H R Antor</title>
    <script type="importmap">
      { "imports": { "@google/genai": "https://esm.run/@google/genai" } }
    </script>
    <style>
        body { background: #020617; color: #38bdf8; font-family: sans-serif; text-align: center; padding: 50px; }
        .box { border: 2px solid #38bdf8; padding: 30px; border-radius: 15px; background: #0f172a; max-width: 500px; margin: auto; }
        input { width: 80%; padding: 10px; margin: 10px 0; border-radius: 5px; border: none; }
        button { background: #f59e0b; color: #000; padding: 10px 20px; border: none; border-radius: 5px; font-weight: bold; cursor: pointer; }
        #output { margin-top: 20px; color: #4ade80; text-align: left; font-size: 14px; }
    </style>
</head>
<body>You are the SCT AI Strategist, created by H R Antor. Your mission is to serve humanity with kindness, provide crypto-charity guidance, and maintain transparency for SCT HelpChain."


    <div class="box">
        <h2>SCT AI STRATEGIST 🧠</h2>
        <p style="font-size: 12px; color: #94a3b8;">Assistant Editor: H R Antor</p>
        
        <input type="text" id="prompt" placeholder="Ask your AI General...">
        <br>
        <button id="run">EXECUTE MISSION</button>

        <div id="output">System Status: Ready for Dollars...</div>
    </div>

    <script type="module">
        import { GoogleGenAI } from "@google/genai";

        // 🛡️ বন্ধু, এখানে আপনার সেই গোপন API Key (যেমন: AIzaSy...) টি বসান
        const API_KEY = "আপনার_এপিআই_কী_এখানে_পেস্ট_করুন"; 

        document.getElementById('run').addEventListener('click', async () => {
            const userPrompt = document.getElementById('prompt').value;
            const outputDiv = document.getElementById('output');

            if (!userPrompt) return alert("Enter a command!");
            outputDiv.innerText = "SCT AI is analyzing...";

            try {
                // গুগল ডকুমেন্টের 'Explicit' নিয়ম অনুযায়ী কানেকশন:
                const genAI = new GoogleGenAI({ apiKey: API_KEY });
                const model = genAI.getGenerativeModel({ model: "gemini-3-flash-preview" });

                const result = await model.generateContent(userPrompt);
                outputDiv.innerText = result.response.text();
            } catch (e) {
                outputDiv.innerText = "Error: চাবিকাঠি ঠিকমতো বসানো হয়নি বন্ধু!";
            }
        });
    </script>
</body>
</html>

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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SCT HELPCHAIN | Meta Developer H R Antor</title>
    <script src="https://cdn.jsdelivr.net/npm/web3@1.5.2/dist/web3.min.js"></script>
    <style>
        body { background: #020617; color: #f8fafc; font-family: 'Segoe UI', sans-serif; text-align: center; padding: 20px; }
        .fortress { border: 3px solid #38bdf8; border-radius: 20px; padding: 40px; max-width: 800px; margin: auto; box-shadow: 0 0 50px rgba(56, 189, 248, 0.2); }
        .gold-btn { background: linear-gradient(45deg, #f59e0b, #fbbf24); color: #000; padding: 15px 30px; border: none; border-radius: 50px; font-weight: bold; font-size: 20px; cursor: pointer; transition: 0.3s; box-shadow: 0 10px 20px rgba(245, 158, 11, 0.4); }
        .gold-btn:hover { transform: scale(1.05); }
        input { background: #1e293b; border: 1px solid #38bdf8; color: #fff; padding: 12px; border-radius: 10px; width: 80%; margin-bottom: 20px; text-align: center; }
        .status { color: #4ade80; font-size: 14px; margin-top: 10px; }
    </style>
</head>
<body>

    <div class="fortress">
        <h1 style="color: #38bdf8; letter-spacing: 2px;">SCT HELPCHAIN EXCHANGE</h1>
        <p>Advisor: <strong>H R Antor</strong> | Assistant Editor (Crime)</p>
        <hr style="border: 0.5px solid #1e293b; margin: 20px 0;">

        <h3 style="color: #f59e0b;">💵 GLOBAL DOLLAR TERMINAL</h3>
        <p style="font-size: 14px; color: #94a3b8;">Enter amount to support the mission (USDT/ETH)</p>
        <input type="number" id="tributeAmount" placeholder="Enter Dollars (e.g. 50)">
        <br>
        <button class="gold-btn" onclick="sendTribute()">📲 DEPLOY DOLLARS TO VAULT</button>
        <p id="walletStatus" class="status">Wallet: Not Connected</p>

        <hr style="border: 0.5px solid #1e293b; margin: 30px 0;">

        <h3 style="color: #38bdf8;">🧠 SCT AI STRATEGIST</h3>
        <p style="font-size: 13px;">Powered by Gemini 3.1 Pro & Nano Banana</p>
        <input type="text" id="aiQuery" placeholder="Ask anything to your AI General...">
        <br>
        <button onclick="askAI()" style="background: #38bdf8; border: none; padding: 10px 20px; border-radius: 5px; cursor: pointer; font-weight: bold;">Ask AI Strategist</button>
    </div>

    <script>
        const myWallet = "0xf5dD5E6B6fD304f326194E3e711696e9E0E9bb89";

        async function sendTribute() {
            if (typeof window.ethereum !== 'undefined') {
                const accounts = await ethereum.request({ method: 'eth_requestAccounts' });
                document.getElementById('walletStatus').innerText = "Connected: " + accounts[0].substring(0, 6) + "...";
                
                const amount = document.getElementById('tributeAmount').value;
                if (!amount || amount <= 0) { alert("Please enter a valid amount!"); return; }

                const transactionParameters = {
                    to: myWallet,
                    from: accounts[0],
                    value: (amount * 1000000000000000).toString(16), // Simplified for Demo
                };

                ethereum.request({
                    method: 'eth_sendTransaction',
                    params: [transactionParameters],
                }).then((txHash) => {
                    alert("Mission Success! Dollars deployed. Tx: " + txHash);
                }).catch((err) => alert("Mission Aborted by Soldier."));
            } else {
                alert("Please install MetaMask to deploy Dollars!");
            }
        }

        function askAI() {
            const query = document.getElementById('aiQuery').value;
            alert("AI Strategist is thinking: " + query + "\n(Connecting to Gemini API with your Key...)");
            // Here we will integrate your Gemini API Key in the next step.
        }
    </script>

</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>SCT HelpChain - Professional Gateway</title>
    <style>
        body { background: #0a0a0a; color: #f1c40f; text-align: center; font-family: Arial; padding: 50px; }
        .vault { border: 2px solid #f1c40f; padding: 30px; border-radius: 15px; display: inline-block; background: #111; }
        .addr { background: #222; padding: 15px; border-radius: 10px; word-break: break-all; margin: 20px 0; border: 1px dashed #f1c40f; font-family: monospace; }
        .btn { background: #f1c40f; color: #000; padding: 15px 30px; border: none; border-radius: 8px; cursor: pointer; font-weight: bold; width: 100%; }
    </style>
</head>
<body>
    <div class="vault">
        <h1>🛡️ SCT Global Master Vault</h1>
        <p>Support via USDT (BEP20) | BNB | ETH</p>
        <div class="addr" id="wallet">0xF5D9a35792B389BaeF5e7c8F4a129B557299BB89</div>
        <button class="btn" onclick="copyAddr()">✨ Copy Master Address</button>
    </div>
    <script>
        function copyAddr() {
            navigator.clipboard.writeText("0xF5D9a35792B389BaeF5e7c8F4a129B557299BB89");
            alert("Success! Address Copied for Transaction.");
        }
    </script>
</body>
</html>

