
<html>
<head>
<title>TODO List</title>
 <style>
    body {
        justify-content: center;
        align-items: center;
        background-color: #FFFFE0;
    }

    .container {
background-color: #FFB6C1;
padding: 20px;
text-align: center;
 width: 300px;
}
label{
font-family: Comic Sans MS;
}

h1{
font-family:Segoe Print;
color:#6e4646;
}

  
</style>

</head>


<body>

<div class="container">
    <h1>TODO</h1>

    <label id="demo">WAKEUP</label>
    <input type="checkbox" id="checkbox1" onchange="todo('checkbox1', 'demo')">
    <br>

    <label id="cli">TEA</label>
    <input type="checkbox" id="checkbox2" onchange="todo('checkbox2', 'cli')">
    <br>

    <label id="clo">FOOD</label>
    <input type="checkbox" id="checkbox3" onchange="todo('checkbox3', 'clo')">
</div>






<script>
function todo(checkboxId, textId) {
    let checkbox = document.getElementById(checkboxId);
    let text = document.getElementById(textId);

    if (checkbox.checked) {
        text.style.textDecoration = "line-through"; // Apply strikethrough
    } else {
        text.style.textDecoration = "none"; // Remove strikethrough
    }
}
</script>

</body>
</html>
