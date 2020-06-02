# 이벤트(Events)

  이벤트에 대해 취할 action을 gird의 속성(property)으로 설정한다.  예를 들면

[함수(Method)]() 참조

```javascript
var lastSet;
jQuery("#girdid").jqGrid({
...
    onSelectRow: function(id) {
		if(id && id == lastSet){
            jQuery("#girdid").restoreRow(lastSet);
            lastSet = id;
        }
        jQurey("#gridid").editRow(id, true);
    }
})
```

 위의 예시는 행이 선택되었을 때의 이벤트를 보여주고 있다. 





## 이벤트 리스트

| 이벤트 | 파라미터 | 설명 |
| ------ | -------- | ---- |
| afterInsertRow | rowid, rowdata, rowelem    | 이 이벤트는 행이 추가될 때마다 발생한다. `rowid`는 추가된 행의 id 값이다. `rowdata`는 추가될 행의 값(data)의 배열이다. |
|        |          |      |
|        |          |      |



## triggered 이벤트(new in v4.3.2)



## 실행 순서

이하는 ajax 요청에 의해 만들어지는 이벤트의 순서이다.

1. `beforeRequest`
2. `loadBeforeSend`
3. `serializeGridData`
4. `loadError`
5. `beforeProcessing`
6. `gridComplete`
7. `loadComplete`