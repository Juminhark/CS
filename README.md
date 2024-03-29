# CS(Computer Science)

## reference

- [Inpa Dev](https://inpa.tistory.com/entry/%F0%9F%91%A9%E2%80%8D%F0%9F%92%BB-%EB%8F%99%EA%B8%B0%EB%B9%84%EB%8F%99%EA%B8%B0-%EB%B8%94%EB%A1%9C%ED%82%B9%EB%85%BC%EB%B8%94%EB%A1%9C%ED%82%B9-%EA%B0%9C%EB%85%90-%EC%A0%95%EB%A6%AC)

## 개발 면접

### [js 개발면접 단골 질문](https://www.youtube.com/watch?v=zrzZXhDiiLs)

- 이정도 내용은 설명을 할줄알아야 한다

프론트엔드에서 면접 질문을 구분해보자면

- javascript
- 알고리즘
- 최적화
- 네트워크
- 협업
- css
- 이슈관리
- 형상관리
- nodejs
- browser 개발

그중 javascript 관련 질문 요약

- prototype
  prototype이 뭐예요?
  function.bind 되는 이유는?
  상속을 구현해볼래요?

- this
  this는 언제 결정되나요
  arrow function this는?
  this를 변경시키려면?
  call, apply

*

- debugging
  버그 문제를 어떻게 해결해요?
  본인만의 디버깅 방식은?
  calling stack?
  nerwork 오류 상황에 어떻게 확인해요?

* step into
* breaking / net

- closure
  closure를 정의한다면?
  closure를 활용한 구현경험?
  커링 아세요?
  고차함수는 뭔가요?

* scope closure에 대한 이해를 정리해볼필요가있다

- FP(Functional Programming)
  배열의 고차함수 어떤것을 사용하세요?
  reduce 한번 구현해보세요
  합성은 상속과 어떤 장점이 있나요?
  immutable? 그것의 단점도 있나요?

*

- OOP(Object-Oriented Programing)
  ES Classes 상속 경험있어요?
  객체를 나누는 단위는?
  애플리케이션 의존성을 낮추는 방법은?

*

- 비동기
  Promise, async/await 차이는?
  promise 패턴 설명해보세요
  setTimeout에 promise적용한다면?
  동시에 여러개의 관계없는 요청을 한다면?
  Micro task queue?

*

- 객체
  객체 표현 방식 중 자주 사용하는 것은?
  class, prototype, literal 차이?
  자주 사용하는 메서드는?
  JSON 데이터 파싱시 가장 신경쓰는것은?

* Object 와 object의 차이

- 기타
  generator 뭔가요?
  ES Next 관심있는 문법은?
  정규표현식은 언제 써봤어요?

### [신입 백엔드 개발 면접 질문](https://zero-base.co.kr/event/media_BE_school_qna)

- 면접을 통과하기 위해 답을 찾고 외우는 것이아니라 스스로 질문에 대답할수 있는 기본기가 있는지를 확인

1.  HTTP METHOD에 대해 설명해 보세요
    HTTP METHOD에는 get, post, put, delete가 있습니다
    단순히 종류를 나열하는 것이 아닌, get과 post간의 차이점에 대해 말할수 있어야한다
    get은 client에서 server로 어떠한 리소스로부터 정보를 요청하기 위해 사용되는 mehtod이다
    즉, server에서 어떤 데이터를 가져와서 보여줄 때, 값이나 채용, 상태 등을 바꾸지 않는 경우에 사용한다
    post는 리소스를 생성/업데이트하기 위해 서버에 데이터를 보내는데 사용되는 method이다
    서버상의 데이터 값이나 상태를 바꾸기 위해서 사용한다
    주요 차이점으로는, get 요청은 캐시가 되나, post는 캐시 되지 않는다
    get은 브라우저에 기록되지만 post는 기록되지 않는다

2.  HTTP 상태 코드에 대해 아는 대로 말해보세요
    주요 상태 코드(200, 404, 503) 정도는 알고 있어야 한다

- 200 : OK, 요청이 성공적으로 되었습니다. 정보는 요청에 따른 응답을 반환됩니다
- 404 : 서버는 요청받은 리소스를 찾을 수 없습니다. 브라우저에서는 알려지지 않은 URL을 의미합니다
  APL에서 종점은 적절하지만 리소스 자체는 존재하지 않음을 의미할 수 있습니다.
  서버들은 인증받지 않은 client로부터 리소스를 숨기기 위하여 이 응답을 403 대신에 전송할 수도 이씁니다
- 503 : 서버가 요청을 처리할 준비가 되지 않았습니다. 유지 보수를 위해 작동이 중단되거나 과부하가 걸린 서버일 경우 발생합니다.

지원자분꼐서 가지고 계신 백엔드 개발 경험 중 상황별로 어떤 상태 코드를 반환하도록 설계하였는지 설명할수있어야 합니다. 이 외에도 1번대부터 5번대 상태 코드까지 각각 대략적으로 어떤 의미인지를 알고 있어야합니다
1xx(정보) : 요청받았으며, 프로세스가 계속 진행합니다
2xx(성공) : 요청을 성공적으로 받았으며 인식했고 수용합니다
3xx(리다이렉션) : 요청 완료를 위해 추가 작업 조치가 필요합니다
4xx(클라이언트 오류) : 요청의 문법이 잘못되었거나 요청을 처리할 수 없습니다
5xx(서버 오류) : 서버가 명백히 유효한 요청에 대해 충족을 실패했습니다

3. 프로세스와 스레드의 차이에 대해 설명해 보세요
   프로세스는 자원을 할당받는 작업의 단위이며, 스레드는 프로세스가 할당받은 자원을 이용하는 실행의 단위.
   스레드는 자원을 공유한다는 점이 차이점이 있습니다.

4. RDB와 NoSQL의 차이에 대해 설명해 보세요.
   RDBMS는 정해진 스키마가 존재하고, NoSQL는 정해진 스키마가 없다는 것이 가장 큰 차이입니다.
   NoSQL은 정해진 스키마가 없을 때 데이터 구조 변화가 자유롭고 데이터 분산이 용이하다는 장점이 이지만, 데이터 중복이 발생하거나 데이터 변경 시에 연산이 오래 걸린다는 단점이 있습니다.

5. DB에서 인덱스를 잘 사용하면 어떤 장점이 있을까요?
   DB의 인덱스를 잘 사용하는 것은 데이터를 검색하는 시점에 성능 차이에 큰 영향을 미칩니다. 대용량 데이터를 담고 있는 DB테이블에서 필요한 데이터를 빨리찾기 위해 인덱스가 필요합니다. 인덱스가 업거나 적절한 인덱스를 찾지 못할 경우 데이터가 담겨있는 테이블 전체를 읽어야 하기에 데이터 조회 시간이 오래 걸립니다. 인덱스는 DB데이터의 주소를 갖고 있는 것을 의미하며, 원하는 데이터를 빠르게 찾을 수 있다는 장점을 가지고 있습니다

6. GC 가비지 컬렉션에 대해 아는 대로 설명하시오
   GC 가비비 컬렉션은 프로그래머가 동적으로 할당한 메모리 영역 중 더 이상 쓰이지 않는 가비지 영역을 찾아서 해제하는 기능을 의미합니다. 답변 시 Full GC에 대해서도 설명할 수 있으면 좋습니다
   자바 메모리는 Young, Old, Perm 세 영역으로 나뉩니다. 이 중 Perm(Permanent)영역은 거의 사용되지 않으며 Young(Eden, Survivor), Old 2가지 영역으로 나뉘어 있습니다. 객체는 처음 생성되었을 때 Young 영역에 있다가 Old 영역으로 넘어가게 되는데, Old 영역이 꽉 찼을 때 Full GC가 발생하게 됩니다. full GC가 발생하면 애플리케이션에 부하가 발생하여 성능이 Full GC 발생 순간에 저하됩니다. 자바 성능상 이슈를 유발할 수 있는 Full GC의 이론에 대해 알아두면 좋습니다

7. 병렬 프로그래밍에 대해 아나요? 프로그래밍을 해본적이 있나요?
   큰 문제를 작게 나누어 동시에 해결할 때 병렬 프로그래밍을 사용합니다. 지원자분께서 멀티 프로세싱 or 멀티 쓰레딩을 구현해 본 경헙을 함께 설명할 수 있다면 좋습니다
   ex) python의 pthread 라이브러리르 사용한 멀티 스레딩 경험
   추가적으로 병렬 프로그래밍은 큰 문제를 프로세스 혹은 스레드가 나누어 처리를 하기 때문에 처리 속도가 향상된다는 장점을 가지고 있습니다. 단점으로는 구현 난이도가 올라간다는 점입니다. 특히 큰 문제를 일정량씩 나누고, 각 분리된 테스크를 어떻게 배정해서 처리할 것인지에 대한 고민이 필요합니다. 또한, 여러 스레드가 하나의 데이터를 공유한 경우에 아래 8번 문제를 유의해야합니다

8. ?? 병렬 프로그래밍을 할 때 어떤 부분을 유의해야 하나요? 세마포어와 뮤텍스에 대해 알고 있나요? 생길 수 있는 문제는?
   뮤텍스는 한 스레드, 프로세스에 의해 소유될 수 있는 key를 기반으로 합니다. 반면 세마포어는 현재 공유자원에 접근할 수 있는 스레드, 프로세스의 수를 나타내는 값을 기반으로 합니다. 뮤텍스나 세마포어를 쓰더라도 데드락이 발생할 수 있습니다

9. 트러블슈팅을 해본 경험이 있나요?
   백엔드 개발을 하면서 막혔던 부분과 해결과정, 그리고 그 과정을 통해 깊이 알게 된 개념을 한 가지 정도 풀어서 설명할 수 있으면 좋습니다

10. 가장 기억에 남는 백엔드 프로젝트의 구조를 그려보세요
    프로젝트의 DB 설계부분과 백엔드 사이의 관계가 보이도록 그려야 합니다. Springboot 프로젝트를 한 경우에 아래의 이미지처럼 controller, service, repository를 나누어 백엔드 프로젝트를 구성했음을 명시해야 합니다

11. LRU 캐시에 대해 설명하시오
    LRU 캐시는 Least Recently Used 캐시로 캐시 메모리가 다 차면, 가장 오랫동안 사용되지 않았던 캐시를 메모리에서 삭제하는 알고리즘입니다. 캐시를 교체하는 알고리즘이 어떤 것 들이 있는지 이해해두면 좋습니다

- 캐시 교체 알고리즘의 종류 예시
  - FIFO(First In First Out)
  - LFU(Least Frequently Used)
  - LRU(Least Recently Used)

12. 연결 리스트에서 값을 찾는데 시간 복잡도가 얼마나 걸리는가? 더 개선된 구조가 있는지? 단점은?
    O(n)의 복잡도가 걸립니다. 뒤쪽 원소도 빠르게 검색할 수 있는 Doubly Linked List 구조도 있으며, 이는 저장공간이 더 필요하다는 단점이 있습니다. 그외에 Circular Linked List 등도 있습니다. 연결 리스트를 수도 코드로 간단하게 구현할 줄도 알면 좋습니다

```
수도코드 (한글버전)
1. 데이터와 다음 데이터의 값을 가진 노드를 생성한다.
　 1-1. 새 노드 생성시 다음값으로 null로 가리킨다.
　 1-2. 새 링크드 리스트 생성시 객체를 생성한다.

2. 링크드 리스트에 맞는 메소드함수를 구현한다.
　 2-1. append(data) :
　 　 2-1-1. 헤드가 없으면 헤드 노드를 생성하고 null을 가리킨다.
　 　 2-1-2. 만약 헤드가 null을 가리키면, 헤드가 새로 생성된 데이터를 가리키게 한다.
　 　 2-1-3. 만약 헤드가 다음 데이터를 가르키고 있으면 그 다음 데이터가 새로운 데이터를 가리키게 하고 데이터를 추가한다.
　 2-2. removeAt(location) : 데이터의 위치에 따라 데이터를 삭제한다.
　 　 2-2-1. 삭제하고자 하는 데이터의 이전 데이터가 삭제하고자 하는 데이터의 다음 데이터를 가리키게 하고 삭제할 데이터는 null을 가리키게 한다.
　 　 2-2-2. 만약 리스트의 첫번째를 삭제하려면 헤드를 다음 데이터로 바꾸고 삭제할 데이터를 삭제한다.
　 2-3. indexOf(data) : 데이터를 순서대로 따라가면서 인덱스를 더해준다. 일치하는 데이터를 찾으면 인덱스를 반환한다.
　 2-4. remove(data) : 데이터 값을 기준으로 삭제를 원할 때 인덱스의 값을 찾아 일치하는 값을 removeAt(index)로 삭제한다.
　 2-5. insert(location, data) : 원하는 위치에 데이터를 추가할 때 인덱스 값을 기준으로 위치를 찾고 데이터를 추가한다.
　 2-6. isEmpty() : 자료의 수가 0 이상이면 false를 반환한다.
　 2-7. length() : 리스트내 전체 자료의 수를 반환한다.
```

13. 스택 2개를 활용해서 Queue처럼 가동하는 클래스를 만들어보세요
    예를 들어 1 2 3 4를 큐에 넣으면 순서대로 1 2 3 4가 나옵니다. 이를 선입선출이라고 합니다. 하지만 스택은 1 2 3 4를 넣으면, 4 3 2 1이 나옵니다. 스택은 큐와 다르게 선입후출의 구조입니다. 하지만, 스택 2개를 활용하는 경우. 2번째 스택에 아무것도 없는 상태에서 pop를 수행한다면 첫 번째 스택에 쌓여있는 값을 2번째 스택으로 이관시킬 수 있습니다.

[관련하여 잘 정리된 블로그 글 함께 첨부합니다.](https://limkydev.tistory.com/185)

14. CI/CD란? 적용해 본 적이 있나요?
    CI/CD란 서비스 빌드부터 배포까지의 과정을 자동화하는 과정입니다. github로 코드 커밋 했을 때 해당 동작을 감지하여 jenkins 가 자동으로 빌드하도록 설계해 본 경험이 있다 등의 경험을 함께 이야기하면 좋습니다.

15. 마이크로 서비스와 모놀리틱 서비스의 차이
    마이크로 서비스는 개별 서비스 단위로 개발하는 방식이고, 모놀리틱 서비스는 하나의 통합된 패키지로 개발하는 방식입니다. 마이크로 서비스는 개별 서비스 단위로 나누어져 있어 해당 부분만 수정 및 배포하기에 좋고, 필요한 부분만 확장하기에도 용이하다는 장점이 있습니다.

### [면접 질문 정리](https://gmlwjd9405.github.io/tags.html#%EB%A9%B4%EC%A0%91)

## setTimeout() : 비동기 함수, 논블로킹 함수

## Synchronous / Asynchronous

synchronous는 작업 시간을 함께 맞춰서 실행한다는 뜻. 작업을 맞춰 실행한다는 말은 요청한 작업에 대해 완료 여부를 따져 순차대로 처리하는것.

asynchronous는 요청한 작업에 대해 완료 여부를 따지지 않기 때문에 작신의 다음 작업을 그대로 수행한다

![sync-async](/assets/sync_async.png)

## Blocking / Non-Blocking

다른 요청의 작업을 처리하기 위해 현재 작업을 block(차단, 대기)하며 프로세스를 실행하는지의 유무에 따라 blocking/non-blocking으로 나뉜다.

synchronous/asynchronous 가 전체적인 작업에 대한 순서적인 흐름 유무라면, blocking/non-blocking은 전체적인 작업의 흐름 자체를 막는지의 유무로 볼수 있다.

![blocking_non-blocking](/assets/block_nonblock.png)

## 동기/비동기 + 블로킹/논블로킹 조합

- Sync Blocking
- Async Blocking
- Sync Non-Bloking
- Async Non-Blocking

![combination](/assets//combinaion.png)

### sync blocking

```js
const fs = require('fs'); // 파일 시스템 모듈 불러오기

// 동기적으로 파일 읽기
const data1 = fs.readFileSync('file1.txt', 'utf8'); // file1을 sync으로 read 함
console.log(data1); // 파일 내용 출력하고 적절한 처리를 진행

const data2 = fs.readFileSync('file2.txt', 'utf8');
console.log(data2);

const data3 = fs.readFileSync('file3.txt', 'utf8');
console.log(data3);
```

### async non-blocking

```js
// 비동기적으로 파일 읽기
const fs = require('fs'); // 파일 시스템 모듈 불러오기

fs.readFile('file.txt', 'utf8', (err, data) => {
  // 파일 읽기 요청과 콜백 함수 전달
  if (err) throw err; // 에러 처리
  console.log(data); // 파일 내용 출력
});

fs.readFile('file2.txt', 'utf8', (err, data) => {
  if (err) throw err;
  console.log(data);
});

fs.readFile('file3.txt', 'utf8', (err, data) => {
  if (err) throw err;
  console.log(data);
});

console.log('done'); // 작업 완료 메시지 출력
```

### sync non-blocking

```js
const fs = require('fs');
const { promisify } = require('util'); // 유틸리티 모듈 불러오기
const readFileAsync = promisify(fs.readFile); // fs.readFile 함수를 Promise 객체를 반환하는 함수로 변환

async function readFiles() {
  try {
    // Promise.all() 메소드를 사용하여 여러 개의 비동기 작업을 병렬로 처리합니다. (비동기 논블로킹)
    const [data1, data2, data3] = await Promise.all([
      readFileAsync('file.txt', 'utf8'), // file.txt 파일을 읽습니다.
      readFileAsync('file2.txt', 'utf8'), // file2.txt 파일을 읽습니다.
      readFileAsync('file3.txt', 'utf8'), // file3.txt 파일을 읽습니다.
    ]);

    // 파일 읽기가 완료되면 data에 파일 내용이 들어옵니다.
    console.log(data1); // file.txt 파일 내용을 출력합니다.
    console.log(data2); // file2.txt 파일 내용을 출력합니다.
    console.log(data3); // file3.txt 파일 내용을 출력합니다.

    // 파일 비교 로직 실행...
  } catch (err) {
    throw err;
  }
}

readFiles(); // async 함수를 호출
```

## 소프트웨어 용어

parameter : 매개변수
argument : 인수 : 함수나 서브루틴, 명령을 사용할 때 주어지는 변수

## 컴퓨터의 수체계

- int 는 정수형을 처리하기 위한 변수.
- 과거 컴퓨터는 cpu는 16bit(2byte)씩 연산
- 현재 cpu는 34bit(4byte), 64bit(8byte) 를 이용
- cpu의 연산을 최적화하기 위한 data크기를 설정한것이 변수단위

- 32bit cpu의 처리 비트수.
- char: 8비트 정수형
- short: 16비트 정수형
- int: 32비트 정수형
- long long: 64비트 정수형
