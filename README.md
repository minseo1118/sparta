<!DOCTYPE html>
<html>

<head>
    <title>자바스크립트 문법 연습하기!</title>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
</head>
<script>
    function checkResult() {

        let people = [
            { 'name': '서영', 'height': 165 },
            { 'name': '현아', 'height': 170 },
            { 'name': '영환', 'height': 175 },
            { 'name': '서연', 'height': 162 },
            { 'name': '지용', 'height': 190 },
            { 'name': '예지', 'height': 168 }
        ]

        $('#q2').empty();

        people.forEach(a => {
            let name = a['name'];
            let height = a['height'];
            let temp_html = `<p>${name}의 키는 ${height}cm 입니다.</p>`;
            $('#q2').append(temp_html);

            //같은 명령 
            //let temp_html = `<p>${a['name']}는 ${a['age']살입니다.</p>`;
            //$('#q2').append(temp_html);

        });
    }
</script>

<body>
    <div class="top-part">
        <h1>자바스크립트 문법 연습하기!</h1>
    </div>
    <hr />
    <br>
    <h2>1. 함수</h2>
    <div class="button-part">
        <button onclick="checkResult()">결과 확인하기!</button>
    </div>
    <div class="list-part">
        <h2>2. 붙이기</h2>
        <div id="q1">
            <p>사과</p>
            <p>귤</p>
            <p>감</p>
        </div>
    </div>
    <div class="list-part">
        <h2>3. 붙이기</h2>
        <div id="q2">
            <p>영수는 24살입니다.</p>
            <p>세종은 30살입니다.</p>
            <p>수영은 20살입니다.</p>
        </div>
    </div>
</body>

</html>
