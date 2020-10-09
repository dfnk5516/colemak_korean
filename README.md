# 윈도우용 콜맥(colemak) 한글 입력 프로그램
## 라이센스(license)
[GNU General Public License v3.0](https://ko.wikipedia.org/wiki/GNU_%EC%9D%BC%EB%B0%98_%EA%B3%B5%EC%A4%91_%EC%82%AC%EC%9A%A9_%ED%97%88%EA%B0%80%EC%84%9C)

## 소개
윈도우 운영체제에서 콜맥 자판을 한글과 함께 간편히 사용할 수 있는 프로그램입니다.
더불어 일반 쿼티 사용자가 본인의 컴퓨터를 쓰게 될 경우 바로 쿼티 자판으로 변경 또한 용이하도록 만들었습니다.<br>

### 장점
- 실행파일을 다운로드하여 단순히 실행하는 것만으로도 바로 콜맥 자판을 사용할 수 있을만큼 간편하면서도 강력합니다.<br>
- 일반 쿼티 사용자가 본인의 컴퓨터를 쓰게 될 경우, 바로 쿼티 자판으로 변경 가능하기에 단일 사용자를 목표로 만들어진 윈도우 운영체제의 한계를 극복할 수 있습니다.

### 단점
- 오토핫키의 한계로써, 낮은 단계에서 바로 입력을 넣는 것이 아니고 키 입력을 가로채서 바꿔 전달하는 것이기에 컴퓨터가 버벅이거나 연타를 할 경우 쿼티 자판의 키가 입력될 수 있습니다.(완벽한 입력기라고 할 수 없다.)
- 일부 프로그램 혹은 일부 검색창에서 적용안될 수 있습니다. 이 경우 쿼티로 바꿔서 써야합니다.<kbd>window</kbd>+<kbd>space</kbd>


## 설명
`키 입력을 가로채서 바꿔 전달해주는 것이기 때문에(키 매핑) windows 입력기가 Microsoft 한글 입력기 일경우에만 제대로 적용됩니다.`

colemak_korean 폴더 내부에 short_key_colemak 폴더와 short_key_qwerty 폴더가 있습니다. short_key_colemak 폴더는 단축키까지 콜맥 자판을 따라가는 것이고, short_key_qwerty 폴더는 기본 입력은 콜맥이지만, 단축키는 쿼티를 따라갑니다. 아직 콜맥자판이 익숙하지 않거나 혹은 기본 입력은 콜맥이 좋지만 단축키는 쿼티의 것을 그대로 사용하고 싶은 사람들을 위해 구분했습니다.

각각의 폴더 속에는 function_key_changed 와 function_key_default 로 나뉩니다. 일반적인 사용자라면 function_key_default 를 사용하면 됩니다. fuction_key_changed 는 개발자인 본인이 사용하기 편하도록 몇몇 키입력을 변경한 것으로, 그것은 하단의 사용법을 참고.


## 사용법
실행파일을 실행하거나 윈도우 부팅시에 자동 실행되도록 스케줄러에 등록(권장) 합니다.

<hr>

### 스케줄러 등록
1. windown 키 - '작업 스케줄러' 입력 - 작업 스케줄러 실행 - 작업 만들기<br>
2. 일반 탭 - 이름 : colemak, 가장 높은 수준의 권한으로 실행 `체크`<br>
3. 트리거 탭 - 새로 만들기 - 작업 시작 : 로그온할 때 - 확인
4. 동작 탭 - 새로 만들기 - 동작 : 프로그램 시작 - 프로그램/스크립트 찾아보기  - 실행하고자 하는 실행파일(colemak.exe) 지정 - 확인 <br>
5. 설정 탭 - 다음 시간 이상 작업이 실행되면 중지 `체크 해제`
6. 확인 - 작업 스케줄러 창 닫기
<hr>

### function_key_changed (변경 전 키 : 변경 후 키)
<kbd>F1</kbd> : <kbd>←</kbd><br>
<kbd>F2</kbd> : <kbd>↓</kbd><br>
<kbd>F3</kbd> : <kbd>↑</kbd><br>
<kbd>F4</kbd> : <kbd>→</kbd><br>
<kbd>F7</kbd> : <kbd>F2</kbd><br>
<kbd>F9</kbd> : <kbd>HOME</kbd><br>
<kbd>F10</kbd> : <kbd>END</kbd>



### 콜맥에서 쿼티로 전환(layout to qwerty)
<kbd>window</kbd>+<kbd>space</kbd><br>
![layout_state](https://public5516.s3.ap-northeast-2.amazonaws.com/colemak_korean.PNG)<br>
화면 최상단 + 최좌측에서 레이아웃을 변경할때 3초간 현재 레이아웃의 상태를 확인할 수 있습니다.



