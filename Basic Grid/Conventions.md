# 규칙(Convention)

 jqGrid의 인스턴스는 속성과 함수, 이벤트를 포함하는 Javascript 객체이다. 여기서 이 인스턴스가 가질 수 있는 속성은 문자열(String)이나 숫자(number), 배열(Array), 불 대수(Boolean)를 비롯한 객체(Object)를 포함한다.



## 호출 규칙

### 자바 스크립트 코드

```javascript
jQuery("#grid_id").jqGrid(options);
```

### HTML

```HTML
<html>
    <body>
        <table id="grid_id"></table>
    </body>
</html>
```

- `grid_id`는  `table` 태그의 id 값으로 정의되며, 그리드의 이름으로 사용된다.
- `option`은 설정 값을 담은 `name:value`형태의 배열이다. 어떠한 설정 값은 그냥 value이고, 어떤 것은 이벤트 처리 함수(function)일 수 있다. jqGrid가 작동하는데 필수적인 설정 값  또한 존재한다.



다음은 My First Grid 예제이다.