# ElfOnShelf

    <button onclick="append('1')">1</button>
    <button onclick="append('2')">2</button>
    <button onclick="append('3')">3</button>
    <button onclick="append('0')">0</button>
  </div>
</div>

<script>
  const display = document.getElementById("display");

  function append(value) {
    display.value += value;
  }

  function clearDisplay() {
    display.value = "";
  }

  function calculate() {
    try {
      display.value = eval(display.value);
    } catch {
      display.value = "Error";
    }
  }
</script>

</body>
</html>
