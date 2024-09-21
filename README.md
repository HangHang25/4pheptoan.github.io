<html lang="vi">
<body>
    <h1>Tính Toán Cơ Bản</h1>

    <label for="a">Số a:</label>
    <input type="number" id="a" value="0"><br><br>

    <label for="b">Số b:</label>
    <input type="number" id="b" value="0"><br><br>

    <button onclick="tinhToan()">Tính toán</button>

    <h2>Kết quả:</h2>
    <p id="tong">Tổng: </p>
    <p id="hieu">Hiệu: </p>
    <p id="tich">Tích: </p>
    <p id="thuong">Thương: </p>

    <script>
        function tinhToan() {
            var a = parseFloat(document.getElementById("a").value);
            var b = parseFloat(document.getElementById("b").value);
            
            var tong = a + b;
            var hieu = a - b;
            var tich = a * b;
            var thuong = b !== 0 ? a / b : 'Không thể chia cho 0';

            document.getElementById("tong").innerText = "Tổng: " + tong;
            document.getElementById("hieu").innerText = "Hiệu: " + hieu;
            document.getElementById("tich").innerText = "Tích: " + tich;
            document.getElementById("thuong").innerText = "Thương: " + thuong;
        }
    </script>
</body>
</html>
