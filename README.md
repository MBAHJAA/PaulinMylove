<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Secret</title>
    <style>
        body {
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            background-color: #bda4eb;
            text-align: center;
        }
        button, a {
            display: inline-block;
            padding: 10px 20px;
            font-size: 16px;
            margin: 0 10px;
            transition: transform 0.2s;
            text-decoration: none;
        }

        button {
            background-color: #814edf;
            color: white;
            border: none;
            border-radius: 10px;
        }

        .H1{
            color: white;
            font-family: sans-serif;
            text-align: center;
        }

    </style>
</head>
<body>
    <div style="padding-top: 6cm;">
        <img src="img/1.gif" alt="" style="width: 170px; height: 150px;">
    </div>
    <div>
        <H1 class="H1">Test</H1>
        <div>
            <button onclick="jawaban('ya')">Yes</button>
            <button onclick="ubahTeks()">No</button>
        </div>    
    </div>
   
    <script>
        function jawaban(pilihan) {
            window.location.href = "next.html";
        }

        function ubahTeks() {
            var tombolTidak = document.querySelector('button:nth-child(2)');
            var tombolYes = document.getElementById('yesButton');
            
            tombolTidak.innerText = 'Apakah Anda Yakin?';
            document.querySelector('button:nth-child(1)').style.transform = 'scale(1.1)';

            tombolTidak.onclick = function() {
                tombolTidak.innerText = 'Apakah Anda Serius?';
                document.querySelector('button:nth-child(1)').style.transform = 'scale(1.2)';

                tombolTidak.onclick = function() {
                    tombolTidak.innerText = 'Beneran????';
                    document.querySelector('button:nth-child(1)').style.transform = 'scale(1.3)';

                    tombolTidak.onclick = function() {
                        tombolTidak.innerText = 'Haaaaa';
                        document.querySelector('button:nth-child(1)').style.transform = 'scale(1.4)';

                        tombolTidak.onclick = function() {
                            tombolTidak.innerText = 'Atuuu';
                            document.querySelector('button:nth-child(1)').style.transform = 'scale(1.5)';

                            tombolTidak.onclick = function() {
                                tombolTidak.innerText = 'Senggg';
                                document.querySelector('button:nth-child(1)').style.transform = 'scale(1.6)';

                                tombolTidak.onclick = function() {
                                    tombolTidak.innerText = 'Pleaseeee';
                                    document.querySelector('button:nth-child(1)').style.transform = 'scale(1.7)';

                                    tombolTidak.onclick = function() {
                                        tombolTidak.innerText = 'Yaudah xixi';
                                        document.querySelector('button:nth-child(1)').style.transform = 'scale(1.8)';
                                        
                                        tombolTidak.onclick = function() {
                                            tombolTidak.innerText = 'Yes';
                                            document.querySelector('button:nth-child(1)').style.transform = 'scale(1)';

                                            tombolTidak.onclick = function() {
                                                tombolTidak.innerText = 'Yes';
                                                document.querySelector('button:nth-child(1)').style.transform = 'scale(1)';
                                                window.location.href = "next.html";
                                            };
                                        };
                                    };
                                };
                            };
                        };
                    };
                };
            };
        }
    </script>
</body>
</html>
