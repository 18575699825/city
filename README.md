# city
aaa
<!DOCTYPE html>
<html>
<head lang="en">
    <meta charset="UTF-8">
    <title></title>
    <style>
        * {
            padding: 0;
            margin: 0;
        }
        ul {
            list-style: none;
        }

        .wrap {
            width: 330px;
            height: 30px;
            margin: 100px auto 0;
            background-image: url(imgs/bg.jpg);
            padding-left: 10px;
        }

        .wrap li {
            float: left;
            width: 100px;
            height: 30px;
            margin-right: 10px;
            position: relative;
        }

        .wrap a {
            color: black;
            text-decoration: none;
            display: block;
            width: 100px;
            height: 30px;
            text-align: center;
            line-height: 30px;
            background-image: url(imgs/libg.jpg);
        }

        .wrap li ul {
            position: absolute;
            display: none;
        }
    </style>
    <script src="jquery-1.11.1.min.js"></script>
    <script>
        $(document).ready(function () {
            // mouseenter事件 是 鼠标经过时触发的事件
            /*$(".wrap li").mouseenter(function () {
                $(this).children("ul").show();
            });

            $(".wrap li").mouseleave(function () {
                $(this).children("ul").hide();
            });*/

            /*$(".wrap li").hover(function () {
                //alert("1");
                $(this).children("ul").show();
            }, function () {
                $(this).children("ul").hide();
            });*/

            /*$(".wrap li").hover(function () {
                /!*alert("1");*!/
                var $this = $(this).children("ul");
                var isShow = $this.css("display");
                if(isShow === "block") {
                    $this.hide();
                } else {
                    $this.show();
                }
            });*/

            $(".wrap li").hover(function () {
                $(this).children("ul").slideToggle();
            });

        });
    </script>
</head>
<body>
    <div class="wrap">
        <ul>
            <li>
                <a href="#">一级菜单1</a>
                <ul>
                    <li><a href="#">二级菜单1</a></li>
                    <li><a href="#">二级菜单2</a></li>
                    <li><a href="#">二级菜单3</a></li>
                </ul>
            </li>
            <li>
                <a href="#">一级菜单1</a>
                <ul>
                    <li><a href="#">二级菜单1</a></li>
                    <li><a href="#">二级菜单2</a></li>
                    <li><a href="#">二级菜单3</a></li>
                </ul>
            </li><li>
            <a href="#">一级菜单1</a>
            <ul>
                <li><a href="#">二级菜单1</a></li>
                <li><a href="#">二级菜单2</a></li>
                <li><a href="#">二级菜单3</a></li>
            </ul>
        </li>
        </ul>
    </div>
</body>
</html>
