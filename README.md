# Note

## [Java](https://namu.wiki/w/Java%20Virtual%20Machine?from=%EC%9E%90%EB%B0%94%20%EA%B0%80%EC%83%81%20%EB%A8%B8%EC%8B%A0#s-4)

method area 와 class loader 에 대해서 문득 궁금했었다.

[f-lab의 설명을 읽어보면 클래스로더와 자바 구조에대한 감을 좀 잡을수 있다.](https://f-lab.kr/insight/class-loader-and-jvm-20241124)

[자세한 그림](https://velog.io/@ddangle/Java-%ED%81%B4%EB%9E%98%EC%8A%A4-%EB%A1%9C%EB%8D%94%EB%9E%80)을 보니, 문득 이게 "어...? 괭장히 비(非)예외적이고, 구조적인 모습인데, 쓰래드별로 독립되어있는 스택이 정말 정석적으로 보였다 (물론 나는 코딩은 야메-독학으로 배운거니 설득력이 없는점이 있지만), 네이티브가 독립되어있는것도 신기하지만 가장 의문이 드는 점은, 레지스터가 렘에 박힌듯한 그림이었다.

[아....](https://doohong.github.io/2018/03/02/Java-runtime-data-area) new로 할당해서 메소드를 다루는게 정말 예술이다... PC Register라는 Stack-Based 방식이라는데, 어디서 들어봤지만 ~~어려워서 스킵~~ 조금 이따가 조사해보기로 하자

`skip - [1]`
---
---
`arrived - [1]`