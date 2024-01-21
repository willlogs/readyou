<div id="terminal" style="background-color: black; color: white; padding: 10px;">
    <p id="output"></p>
    <input type="text" id="input" style="width: 100%; color: black;">
</div>

<script>
    document.getElementById("input").addEventListener("keypress", function(event) {
        if (event.key === "Enter") {
            event.preventDefault();
            var input = document.getElementById("input").value;
            var output = document.getElementById("output");
            if (input.toLowerCase() === "help") {
                output.innerHTML += "Hello World<br>";
            }
            document.getElementById("input").value = "";
        }
    });
</script>