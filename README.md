# Introduction

프론트앤드 개발자를 베이스로 하는 컴퓨터학부 졸업생

- TypeScript, JavaScript, Python, C#
- React
- Node.js
- React-Native, Unity

# Featured Project

## PACEMAKER

자연어로 구성된 영어 문단을 입력으로 받아서 이를 기반으로 객관식 문제를 생성하거나, 질문에 대한 답변을 생성하는 것을 핵심으로 하는 서비스입니다.

주된 사용 목적은 비대면으로 교육을 진행하는 상황에서 집중력의 유지와 학생들의 이해도 증진입니다.

핵심 기능은 영문으로 구성된 자연어 단락을 입력받아서 이를 기반으로 질문(질의문)을 생성하는 것과 입력된 자연어 단락을 기반으로 질문에 대한 답변을 생성하는 것입니다.

현재 NLP 서버가 동작하고 있지 않아서 핵심 기능은 동작하지 않는 상태입니다.

해당 서비스에서 프로젝트 매니저와 프론트엔드를 담당하였습니다.

현재 해당 서비스는 교내시연 이후 AI서버의 부재와 서버 배포에 어려움이 있어서 정상적인 동작을 제공하지 않습니다.

따라서 제가 당시에 주로 맡았던 파트인 Front-End에 더미데이터를 포함하여 재배포하였습니다.

현재는 내부의 더미데이터에 의해 동작하며 < id: "test", pw: "test" > 로 로그인하여 테스트할 수 있습니다.



> Diagrams

[PACEMAKER][pacemaker-repo]의 README에 수록하여 놓았습니다.



Repository: [pacemaker][pacemaker-repo]

Deploy: [PACEMAKER][pacemaker-domo]

[pacemaker-repo]: https://github.com/KLumy/pacemaker-spa-client
[pacemaker-domo]: https://klumy.github.io/pacemaker-spa-client/

> 용어

- 교사(Leader) : 채널을 생성하여 문서를 등록하고 이를 기반으로 문제를 생성하는 역할을 맡는 사용자
- 학생(Runner) : 교사가 생성한 채널에 가입하여 교사가 제공한 문제를 풀거나 공개된 문서를 읽는 사용자

> Front-End

- JavaScript
- React
- Redux

> Back-End

- Python

- mySQL

- Django

- Docker

- Question Generate(UniLm v.1)

## AIKU

일종의 인공지능 스피커로, 사용자는 음성 명령을 통해서 해당 서비스를 이용할 수 있습니다.

음성 명령은 자연어를 기본으로 하고 있으며, 한국어를 통한 사용이 가능합니다.

이를 위해서 입력된 자연어를 바탕으로 질의에 대한 답변을 생성하는 NLP모듈을 포함합니다.

현재 인공지능 서버가 동작하지 않기 때문에 사용할 수 없는 서비스 입니다.

해당 서비스에서 프론트엔드 파트를 담당하였습니다.



> Diagrams

<details>
    <summary>Class Diagram</summary>
    <img src="https://user-images.githubusercontent.com/30566564/123922273-d37d0200-d9c2-11eb-9c24-6e9f6de2fa6e.jpg" alt="Web ClassDiagram" style="zoom:80%;" />
</details>
<details>
    <summary>Sequence Diagram</summary>
    <img src="https://user-images.githubusercontent.com/30566564/123922282-d5df5c00-d9c2-11eb-9843-a3c7bb775cd8.jpg" alt="Event Loop old" style="zoom:80%;" />
</details>



Repository: [AISpeaker-AIKU](https://github.com/KLumy/AISpeaker)

> Front-End

- JavaScript(Vanilla + jQuery(아주 약간))

> Back-End

- Python

- Django

- MySQL

- Question Answering

## Rhine Labs

문화상품권 사용에 어려움을 겪던 중 이를 개선하기 위해 만들어진 서비스입니다.

자세한 사용방법은 해당 서비스의 레포지토리에서 찾아볼 수 있습니다.

AIKU에서 사용하였던 프론트엔드 구조를 재구성하여 조금 더 다듬어서 사용되었습니다.

서버가 존재하지 않는 웹 서비스입니다.



> Diagrams

<details>
    <summary>Class Diagram</summary>
    <img src="https://user-images.githubusercontent.com/30566564/123922374-ee4f7680-d9c2-11eb-9b7a-54d7b681c31f.jpg" alt="ClassDiagram" style="zoom:80%;" />
</details>
<details>
    <summary>Sequence Diagram</summary>
    <img src="https://user-images.githubusercontent.com/30566564/123922383-f14a6700-d9c2-11eb-8e7c-dd60283ea6b1.jpg" alt="EventFlow" style="zoom:80%;" />
    <img src="https://user-images.githubusercontent.com/30566564/123922392-f3acc100-d9c2-11eb-9633-b9f3b81a6fc6.jpg" alt="MakeGiftcard" style="zoom:80%;" />
</details>



Repository: [rhine-labs][rhine-labs-repo]

Deploy: [Rhine Labs][rhine-labs]

[rhine-labs-repo]: https://github.com/KLumy/RhineLabs
[rhine-labs]: https://rhinelab-toolbox.netlify.app/

> Front-End

- JavaScript(Vanilla + jQuery(아주 약간))

## ROOT SEARCH

연관검색어 자동 추적 검색 지원 솔루션으로 계획된 서비스입니다.

검색어를 입력하면 해당 검색어를 기반으로 논리적 연관성을 가진 검색어를 자동으로 추적하여 추가적인 검색을 수행합니다.

검색어는 서버에 캐싱되어 재검색시 빠르게 결과를 제공할 수 있는 기능을 포함합니다.

해당 서비스의 프론트엔드는 Rhine Labs의 구조를 기반으로 기능과 구조를 확장하여 개발되었습니다.

이 서비스에서 프론트엔드를 담당하였습니다.



> Diagrams

<details>
    <summary>Class Diagram</summary>
    <img src="https://user-images.githubusercontent.com/30566564/123922094-a92b4480-d9c2-11eb-8431-cf24ef041e5b.jpg" alt="ClassDiagram" style="zoom:80%;" />
</details>
<details>
    <summary>Sequence Diagram</summary>
    <img src="https://user-images.githubusercontent.com/30566564/123922157-b6483380-d9c2-11eb-9ba9-25b58ce7deb9.jpg" alt="SearchKeyword" style="zoom:80%;" />
</details>

​    

Front-End Repository: [root-search-client][root-search-client-repo]

Back-End Repository: [root-search-server][root-search-server-reop]

Deploy: [ROOT SEARCH][root-search]

[root-search-client-repo]: https://github.com/RootSearch/root-search-client
[root-search-server-reop]: https://github.com/RootSearch/root-search-server
[root-search]: https://rootsearch.github.io/root-search-client/

> Front-End

- JavaScript(Vanilla + jQuery(아주 약간))

> Back-End

- C#

- .Net Core

- Redis

## ANotablePad

서버-클라이언트 모델의 구현을 목적으로 한 프로젝트로, 중앙에 서버를 두고 하나의 클라이언트가 그린 그림을 다수의 클라이언트에게 동일하게 보여주는 기능을 하는 서비스입니다.

클라이언트는 유니티를 이용해서 만들어졌고, 서버는 동일한 언어를 유지하고자 .Net 서버로 구성되었습니다.

간단한 작동 절차는 다음과 같습니다. 중앙에 Name Server를 두고 클라이언트는 Name Server로 접속합니다. 클라이언트가 Name Server에서 방을 만들면 Room Server 프로세스가 생성되어서 클라이언트의 연결을 변경합니다. 이후 Room Server가 서비스를 제공하고 그 방을 나오면 다시 Name Server로 접속하는 구조입니다.

다른 프로젝트보다 초기에 수행한 프로젝트로 완성도가 비교적 낮고 조잡하지만,기초적인 네트워크  다수 사용하여 만든 프로젝트입니다.

이 프로젝트는 1인 프로젝트로 진행되었습니다.

AnotablePad Repositories :

- [AnotablePad_Client](https://github.com/KLumy/AnotablePad_Client)

- [ANotablePad_ClientPC](https://github.com/KLumy/ANotablePad_ClientPC)

- [AnotablePad_RoomServer](https://github.com/KLumy/AnotablePad_RoomServer)

- [AnotablePad_NameServer](https://github.com/KLumy/AnotablePad_NameServer)

> Client

- C#
- Unity

> Server

- C#
- .Net Framework

## DWS

UP 방법론의 실습을 위해 진행한 프로젝트 입니다.
서비스의 기능이나 디자인보다는 개발을 진행하는 과정 자체에 초점을 맞추었습니다.
기능 자체는 단순한 전자 손목시계로, 저희 팀은 철저하게 실존하는 손목시계를 구현하는 것을 목표로 하였습니다.

저는 이 프로젝트에서 전반적인 설계와 디자인, 그리고 각 기능을 총괄하는 컨트롤러와 이벤트 시스템의 구현을 담당하였습니다.
이외에도 저에게 할당된 문서화를 위한 서류작업과 발표 자료 제작을 수행하였습니다.

Java 이외에 Redmin과 젠킨스 등 생소한 도구를 새롭게 익히는 경험이 되었습니다.

> Diagrams

[Digital Watch System](https://github.com/KLumy/OOAD_DWS4)의 README에 수록하여 놓았습니다.]



DWS Repositories :

[Digital Watch System](https://github.com/KLumy/OOAD_DWS4)



> Client

- JAVA
