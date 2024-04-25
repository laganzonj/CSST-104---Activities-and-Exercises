# exercise_activity-CSST104-3B
Compilation of activities and exercises in CSST 104

<html>
<head>
    <title>Button Links</title>
    <style>
        /* Style the button container */
        .btn-container {
            overflow: hidden;
            border: 1px solid #ccc;
            background-color: #f1f1f1;
        }

        /* Style the buttons */
        .btn-container button {
            background-color: inherit;
            float: left;
            border: none;
            outline: none;
            cursor: pointer;
            padding: 14px 16px;
            transition: 0.3s;
        }

        /* Change background color of buttons on hover */
        .btn-container button:hover {
            background-color: #ddd;
        }

        /* Create an active/current button class */
        .btn-container button.active {
            background-color: #ccc;
        }
    </style>
</head>
<body>

<div class="btn-container">
    <button class="btn" onclick="openLink('https://github.com/laganzonj/exercise_activity-CSST104-3B/commit/ee868a6be03ac46869f448ceaf9ff07abadce1a4')" id="btn1">Link 1</button>
    <button class="btn" onclick="openLink('https://www.example.com/link2')" id="btn2">Link 2</button>
    <button class="btn" onclick="openLink('https://www.example.com/link3')" id="btn3">Link 3</button>
</div>

<script>
    function openLink(url) {
        window.location.href = url;
    }
</script>

</body>
</html>
