# CSS의 기초
* 1. 색 넣기
```html
<p style="color:blue">
```
*  와 같이 작성
* 2. margin, padding의 차이점
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        * {
            margin: 0;
        }
    </style>
</head>
<body>
    <img src="http://jhbum.pe.kr/web/4w/images/cat.jpg">
</body>
</html>
```
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <img src="http://jhbum.pe.kr/web/4w/images/cat.jpg">
</body>
</html>
```
* 이 둘의 차이점을 비교해보자
* padding은 글자와 border사이의 거리를, margin은 border와 여백의 거리를 뜻한다는 것을 알 수 있음 
* padding에 색 넣기
```css
* {
    margin: 0;
}
h1{
    padding: 10px;
    background-color: rgb(202, 99, 39);
    color:rgb(0, 0, 0)
}
p{
    padding: 8px;
    background-color: rgb(255, 199, 47);
    color:rgb(0, 0, 0)
}
h2{
    padding: 9px;
    background-color: rgb(252, 158, 35);
    color:rgb(0, 0, 0)
}
h4{
    padding: 8px;
    background-color: rgb(252, 158, 35);
    color:rgb(0, 0, 0)
}
ol{
    padding: 8px;
    background-color: rgb(255, 199, 47);
    color:rgb(0, 0, 0)
}
```
