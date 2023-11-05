<!DOCTYPE html>
<html>
<head>
    <title>تاريخ وعرض نص</title>
    <style>
        #عرض_النص {
            font-family: Arial, sans-serif;
            font-size: 18px;
            color: #333;
            padding: 10px;
            border: 1px solid #ccc;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <label for="التاريخ">الرجاء اختيار تاريخ:</label>
    <input type="date" id="التاريخ">
    <button onclick="عرضالنص()">عرض النص</button>
    <div id="عرض_النص"></div>

    <script>
        function عرضالنص() {
            var التاريخ = document.getElementById("التاريخ").value;
            var النص;
            switch (التاريخ) {
                case "2023-11-01":
                    النص = "نص يناسب اليوم الأول";
                    break;
                case "2023-11-02":
                    النص = "نص يناسب اليوم الثاني";
                    break;
                case "2023-11-03":
                    النص = "نص يناسب اليوم الثالث";
                    break;
                // يُمكنك متابعة الإضافة لجميع أيام الشهر هنا
                case "2023-11-30":
                    النص = "نص يناسب اليوم الثلاثين";
                    break;
                default:
                    النص = "الرجاء اختيار تاريخ آخر.";
            }
            document.getElementById("عرض_النص").innerHTML = النص;
        }
    </script>
</body>
</html>
# NOTI
