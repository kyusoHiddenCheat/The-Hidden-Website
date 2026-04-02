<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hidden Cheat { by @exclsv_apat }</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
        }

        body {
            height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            background: black;
            padding: 20px;
            position: relative;
        }

        .status-container {
            position: absolute;
            top: 20px;
            left: 50%;
            transform: translateX(-50%);
            text-align: center;
        }

        .device-count {
            color: #9932cc;
            font-size: 14px;
            margin-top: 5px;
        }

        .page-title {
            color: #0ff0fc;
            font-size: 25px;
            text-align: center;
            position: absolute;
            top: 80px;
            left: 50%;
            transform: translateX(-50%);
            white-space: nowrap;
        }

        .hub-image {
            width: 250px;
            height: auto;
            margin: 5px 0;
        }

        .page-subtitle {
            color: #ccc;
            font-size: 14px;
            text-align: center;
            margin-bottom: 10px;
        }

        .buttons {
            display: flex;
            flex-direction: column;
            gap: 15px;
            align-items: center;
        }

        .my-button {
            padding: 10px 20px;
            font-size: 15px;
            color: #f8f8ff;
            background: #353839;
            border: none;
            border-radius: 8px;
            width: 260px;
            text-align: center;
            cursor: pointer;
        }

        .my-button:hover {
            background: #5ba0ff;
            transform: translateY(-2px);
        }

        .my-button:active {
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <div class="status-container">
        <div class="page-detect">online</div>
        <div class="device-count">Devices Online: <span id="count">0</span></div>
    </div>
    
    <h1 class="page-title">THE HIDDEN CHEAT</h1>
    
    <img src="https://media1.giphy.com/media/v1.Y2lkPTZjMDliOTUya3lpNTAydGYxaXAyamRzeDBuazR1Z3VmeTNnMXlocTA2eXg1am53bSZlcD12MV9naWZzX3NlYXJjaCZjdD1n/12bF3AWU423YeA/200w.webp" alt="Hub GIF" class="hub-image">
    
    <h2 class="page-subtitle">Executed by @exclsv_apat</h2>
    
    <div class="buttons">
        <button class="my-button" onclick="window.location.href='https://t.me/Hidden_Cheat'">
            Download Terminal Cheat
        </button>
        <button class="my-button" onclick="window.location.href='https://t.me/exclsv_apat'">
            Download Injector Cheat
        </button>
        <button class="my-button" onclick="window.location.href='https://t.me/exclsv_apat'">
            REPORT TO OWNER
        </button>
    </div>

    <script>
        const namespace = "The-Hidden-Website";
        const key = "online-devices";

        fetch(`https://api.countapi.xyz/hit/${namespace}/${key}`)
            .then(response => response.json())
            .then(data => {
 
                fetch(`https://api.countapi.xyz/get/${namespace}/${key}`)
                    .then(res => res.json())
                    .then(info => {
                        document.getElementById("count").textContent = info.value;
                    });
            })
            .catch(error => console.log("Error loading count:", error));
    </script>
</body>
</html> .catch(error => console.log("Error loading count:", error));
    </script>
</body>
</html>
