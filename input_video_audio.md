# 오디오 파일, 비디오 파일 집어넣기, 하이퍼 링크  + 목록, 선택지 만들기
* 이전 레드향 파일에 오디오와 비디오 덧붙이기
* 파일 속에 들어있어야 함
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <title>상품 소개 페이지</title>
    <style>
        table, th, td {
            border:1px solid rgb(158, 255, 182);
            border-collapse: collapse;
        }
        th, td { padding:10px 20px; }
        th {
            background-color:rgb(253, 255, 107);
        }
        td {
            background-color:rgb(185, 255, 232);
        }
    </style>
</head>
<body>
    <img src="tangerines.jpg" alt="레드향">
    <div id="container">
        <audio src="spring.mp3" autoplay></audio>
        <h1>레드향</h1>
        <p>껍질에 붉은 빛이 돌아 <b>레드향</b>이라고 부른다</p>
        <p>레드향은 <em>한라봉과 귤을 교배</em>한 것으로 <br>일반 귤보다 2~3배 크고, 과육이 붉고 통통하다</p>
        <p><i>비타민 C</i>와 <i>비타민 P</i>가 풍부해 <br><b>혈액순환, 감기예방</b> 등에 좋은 것으로 알려져 있다.</p>
    </div>
    <div id="container">
        <h2>레드향 샐러드 레시피</h2>
        <p><b>재료: </b> 레드향 1개, 아보카도 1개, 샐러드 채소 30g</p>
        <p><b>드레싱: </b>올리브유 1큰술, 레몬즙 2큰술, 꿀 1큰술, 소금 약간</p>
        <h4>재료 준비</h4>
        <ol type="I">
            <li>샐러드 채소를 씻어 물기를 제거한 후 먹기 좋게 썰어서 준비합니다.</li>
            <li>레드향과 아보카도, 토마토도 먹기 좋게 자릅니다.</li>
        </ol>
        <h4>드레싱 준비</h4>
        <ol type="I" start="3">
            <li>드레싱 재료를 믹서에 한꺼번에 넣고 갈아 줍니다.</li>
        </ol>
        <h4>샐러드 완성</h4>
        <ol type="I" start="4">
            <li>볼에 샐러드 채소와 레드향, 아보카도, 토마토를 넣고 드레싱을 뿌리면 끝!</li>
        </ol>
        <video src="salad.mp4" width="700" controls></video>
        <img src="salad.jpg" alt="샐러드">
    </div>
    <div id="container">
        <h2>상품 구성</h2>
        <p><a href="file:///C:/Users/user/Desktop/Web%20Pro/check.html">레드향 구매 미리보기</a></p>
        <a href="https://smartstore.naver.com/inhane/products/6419770126?gclid=CjwKCAiAy_CcBhBeEiwAcoMRHM2C_K-su9bnIeWBszBrY1c6qeOhllqg6LOZzI7J4zf0Khd304mqKRoCOe8QAvD_BwE"><p>레드향 구매하기 -></p><img src="레드향.jpg" alt="레드향"></a>
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
    </div>
</body>
</html>
```
* input으로 로그인 페이지 만들기
```html
<!DOCTYPE html>
<html lang="ko">
    <head>
        <meta charset="UTF-8">
        <title>label 태그 사용</title>
    </head>
    <body>
        <label for="user-id">아이디(6자 이상)</label>
        <input type="text" id="user-id">
        <label for="user-pwd">패스워드(6자 이상)</label>
        <input type="password" pwd="user-pwd">
    </body>
</html>
```
* 선택 박스 만들기
```html
<!DOCTYPE html>
<html lang="ko">
    <head>
        <body>
            <h1>레드향 주문하기</h1>
            <fieldset>상품 선택</fieldset>
            <p><b>주문할 상품을 선택해 주세요</b></p>
            <ul>
                <li>
                    <label><input type="checkbox" value="s_3">선물용 3kg</label>
                    <input type="number"개>
                </li>
                <li>
                    <label><input type="checkbox" value="s_5">선물용 5kg</label>
                    <input type="number"개>
                </li>
                <li>
                    <label><input type="checkbox" value="s_3">가정용 3kg</label>
                    <input type="number"개>
                </li>
                <li>
                    <label><input type="checkbox" value="s_5">가정용 5kg</label>
                    <input type="number"개>
                </li>
            </ul>
        </body>
    </head>
</html>
```
