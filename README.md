<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For You ❤️</title>

<style>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #1a1a1a, #2b2b2b);
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    text-align: center;
}

.container {
    max-width: 500px;
}

input {
    padding: 10px;
    border: none;
    border-radius: 8px;
    margin-top: 10px;
}

button {
    padding: 10px 20px;
    border: none;
    border-radius: 8px;
    background: #ff4d6d;
    color: white;
    cursor: pointer;
    margin-top: 10px;
}

.letter {
    display: none;
    margin-top: 20px;
    background: rgba(255,255,255,0.05);
    padding: 20px;
    border-radius: 15px;
}
</style>
</head>

<body>

<div class="container">
    <h2>Enter the secret code 💌</h2>
    <input type="password" id="code" placeholder="Enter code">
    <br>
    <button onclick="checkCode()">Open</button>

    <div class="letter" id="letter">
        <h2>For You ❤️</h2>
        <p>
        I don’t know how to start this…  
        but from the moment you came into my thoughts,  
        something changed inside me.  

        You became that quiet smile I carry,  
        that thought I return to without trying.  

        Even from far away,  
        you feel close in a way I can't explain.  

        Maybe one day I’ll say this to you in person…  
        but for now, this little page holds a piece of what I feel.  

        — Someone who thinks of you 🌙
        </p>
    </div>
</div>

<script>
function checkCode() {
    let code = document.getElementById("code").value;
    if(code === "Aqra") {
        document.getElementById("letter").style.display = "block";
    } else {
        alert("Wrong code...");
    }
}
</script>

</body>
</html>
