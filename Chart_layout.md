# 텍스트를 표현하는 다양한 스타일
* 이전에 배운 table을 사용하면 표 형태가 되지 않았지만, css를 사용하면 표의 형태를 만들 수 있다.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        table{
            caption-side: bottom;
            border: 1px solid #000;
        }
        td, th{
            border: 1px dotted #000;
            padding: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <h2>상품 구성</h2>
    <table>
        <caption>선물용과 가정용 상품 구성</caption>
            <tr>
                <th>용도</th>
                <th>중량</th>
                <th>갯수</th>
                <th>가격</th>
            </tr>
            <tr>
                <td>선물용</td>
                <td>3kg</td>
                <td>11~16과</td>
                <td>35,000원</td>
            </tr>
            <tr>
                <td>선물용</td>
                <td>5kg</td>
                <td>18~26과</td>
                <td>52,000원</td>
            </tr>
            <tr>
                <td>가정용</td>
                <td>3kg</td>
                <td>11~18과</td>
                <td>30,000원</td>
            </tr>
            <tr>
                <td>가정용</td>
                <td>5kg</td>
                <td>18~26과</td>
                <td>47,000원</td>
            </tr>
    </table>
</body>
</html>
```
* 이전에 사용했던 레드향의 표에 css를 추가 하였다.
* style에 있는 class : table에 collapse를 넣으면 테두리가 1 줄이 된다
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        table{
            caption-side: bottom;
            border: 1px solid #000;
            border-collapse: collapse;
        }
        td, th{
            border: 1px dotted #000;
            padding: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <h2>상품 구성</h2>
    <table>
        <caption>선물용과 가정용 상품 구성</caption>
            <tr>
                <th>용도</th>
                <th>중량</th>
                <th>갯수</th>
                <th>가격</th>
            </tr>
            <tr>
                <td>선물용</td>
                <td>3kg</td>
                <td>11~16과</td>
                <td>35,000원</td>
            </tr>
            <tr>
                <td>선물용</td>
                <td>5kg</td>
                <td>18~26과</td>
                <td>52,000원</td>
            </tr>
            <tr>
                <td>가정용</td>
                <td>3kg</td>
                <td>11~18과</td>
                <td>30,000원</td>
            </tr>
            <tr>
                <td>가정용</td>
                <td>5kg</td>
                <td>18~26과</td>
                <td>47,000원</td>
            </tr>
    </table>
</body>
</html>
```
* %, px
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        div{
            border: 2px solid #000;
            margin-bottom: 20px;
        }
        .box1{
            width: 400px;
            height: 100px;
        }
        .box2{
            width: 50%;
            height: 100px;
        }
    </style>
</head>
<body>
    <div class="box1"></div>
    <div class="box2"></div>
</body>
</html>
```
* 상자 꾸미기: shadow, radius 등등
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        div{
            border: 2px solid #000;
            margin-bottom: 20px;
            width: 200px;
            height: 100px;
        }
        .box {
                box-shadow: 4px -5px 10px 6px rgb(146, 0, 0);
            }
        .box2 {
           box-shadow: 4px -5px 10px 6px rgb(35, 0, 160);
        }
    </style>
</head>
<body>
    <div class="box"></div>
    <div class="box2"></div>
</body>
</html>
```
* 상자의 테두리를 표현하는 세가지 기법
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        div{
            border: 2px solid #000;
            margin-bottom: 20px;
            width: 200px;
            height: 100px;
        }
        #box1{
            border-style: solid;
        }
        #box2{
            border-style: dashed;
        }
        #box3{
            border-style: dotted;
        }
    </style>
</head>
<body>
    <div id="box"></div>
    <div id="box2"></div>
    <div id="box3"></div>
</body>
</html>
```
