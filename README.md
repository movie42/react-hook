# 리엑트 훅 연습 프로젝트

## 출처

freecodecampe에 있는 reack강의를 들으면서 작성한 코드
[reack project](https://www.youtube.com/watch?v=a_7Z7C_JCyo&t=811s)
[reack hook 공식문서](https://ko.reactjs.org/docs/hooks-intro.html)

## reack hook

class 바탕의 코드를 작성할 필요 없이 상태 값과 react의 여러 기능을 이용할 수 있다.

1. useState
   birthday reminder(2021.05.12)
   useState는 state와 setState 두 값을 가진다.(이름은 마음대로 바꿀 수 있다.)

```[javascript]
import React, {useState} from "react"

function example(){
    const [state, setState] = useState(0);

    return(
        <div>
            <h1>시작한지 {state}일</h1>
            <button onClick={()=> setState(state + 1)}>
                추가
            </button>
        </div>
    )
}
```

state는 현재 상태를 반영하여 출력한다. setState는 변경할 값을 셋팅할 함수다. useState에 파라미터로 들어가는 값은 초기값이며 state에 반영된다.
