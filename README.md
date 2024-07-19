<html>
    <head>
        <title>thrift stores | fun places</title>
    </head>
    <body>
        <input type="text" id="myInput" onkeyup="myFunction()" placeholder="Search for names.." title="Type in a name">
        <ul id="myUL">
        <li><a target="_blank" href="https://www.summithumane.org/thrift-shop">#1: Happy Talls</a></li>
        <li><a target="_blank" href="https://goodwillakron.org/shop/find-a-store/">#2: Goodwill</a></li>
        <li><a target="_blank" href="https://ohioamishcountry.info/directory/home-hope-thrift-store/">#3: Home and Hope</a></li>
        <li><a target="_blank" href="#">#4:</a></li>
        <li><a target="_blank" href="#">#5:</a></li>
        <li><a target="_blank" href="#">#6:</a></li>
        <li><a target="_blank" href="#">#7:</a></li>
        </ul>
        <a style="color: white; font-size: 25px;" href="https://mcallisterschool.github.io/places/">home</a>        
        <script>
            function myFunction() {
                var input, filter, ul, li, a, i, txtValue;
                input = document.getElementById("myInput");
                filter = input.value.toUpperCase();
                ul = document.getElementById("myUL");
                li = ul.getElementsByTagName("li");
                for (i = 0; i < li.length; i++) {
                    a = li[i].getElementsByTagName("a")[0];
                    txtValue = a.textContent || a.innerText;
                    if (txtValue.toUpperCase().indexOf(filter) > -1) {
                        li[i].style.display = "";
                    } else {
                        li[i].style.display = "none";
                    }
                }
            }
            </script>
    </body>
</html>
