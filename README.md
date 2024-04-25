# exercise_activity-CSST104-3B
Compilation of activities and exercises in CSST 104
<head>
    <title>Tabbed Links</title>
    <style>
        /* Style the tab */
        .tab {
            overflow: hidden;
            border: 1px solid #ccc;
            background-color: #f1f1f1;
        }

        /* Style the buttons inside the tab */
        .tab button {
            background-color: inherit;
            float: left;
            border: none;
            outline: none;
            cursor: pointer;
            padding: 14px 16px;
            transition: 0.3s;
        }

        /* Change background color of buttons on hover */
        .tab button:hover {
            background-color: #ddd;
        }

        /* Create an active/current tablink class */
        .tab button.active {
            background-color: #ccc;
        }

        /* Style the tab content */
        .tabcontent {
            display: none;
            padding: 6px 12px;
            border: 1px solid #ccc;
            border-top: none;
        }
    </style>
</head>
<body>

<div class="tab">
    <button class="tablinks" onclick="openTab(event, 'link1')" id="defaultOpen">Link 1</button>
    <button class="tablinks" onclick="openTab(event, 'link2')">Link 2</button>
    <button class="tablinks" onclick="openTab(event, 'link3')">Link 3</button>
</div>

<div id="link1" class="tabcontent">
    <h3>Content of Link 1</h3>
    <p><a href="https://www.example.com/link1">Visit Link 1</a></p>
</div>

<div id="link2" class="tabcontent">
    <h3>Content of Link 2</h3>
    <p><a href="https://www.example.com/link2">Visit Link 2</a></p>
</div>

<div id="link3" class="tabcontent">
    <h3>Content of Link 3</h3>
    <p><a href="https://www.example.com/link3">Visit Link 3</a></p>
</div>

<script>
    function openTab(evt, tabName) {
        var i, tabcontent, tablinks;
        tabcontent = document.getElementsByClassName("tabcontent");
        for (i = 0; i < tabcontent.length; i++) {
            tabcontent[i].style.display = "none";
        }
        tablinks = document.getElementsByClassName("tablinks");
        for (i = 0; i < tablinks.length; i++) {
            tablinks[i].className = tablinks[i].className.replace(" active", "");
        }
        document.getElementById(tabName).style.display = "block";
        evt.currentTarget.className += " active";
    }

    // Get the element with id="defaultOpen" and click on it
    document.getElementById("defaultOpen").click();
</script>
