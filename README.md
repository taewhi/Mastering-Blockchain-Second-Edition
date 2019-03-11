# 블록체인 완전정복 2/e
[에이콘출판사](http://acornpub.co.kr)에서 출간한 [블록체인 완전정복 2/e](http://acornpub.co.kr/book/mastering-blockchain-2e)의 코드 저장소입니다. 원서는 [팩트출판사(Packt)](https://www.packtpub.com/)에서 출간한 [Mastering Blockchain - Second Edition](https://www.packtpub.com/big-data-and-business-intelligence/mastering-blockchain-second-edition?utm_source=github&utm_medium=repository&utm_campaign=9781788839044)입니다. 이 책을 처음부터 끝까지 진행하는 데 필요한 모든 보조 프로젝트 파일이 담겨 있습니다.
## 이 책에 관하여
블록체인은 여러 노드에 걸쳐 복제되는 분산 원장으로, 트랜잭션 기록을 변경 불가능하고, 투명하며, 암호화하여 안전하게 보관하도록 해줍니다. 블록체인 기술은 암호화폐의 근간이며, 금융, 정부, 언론 등 거의 모든 산업 분야에 적용되고 있습니다. 블록체인 완전정복, 제 2판에서는 전면 개정증보를 거쳐, 선도 기술인 블록체인과 그 구현에 대해 자세히 설명하였습니다.

이 책에서는 먼저 블록체인 기술의 기반 기술인 분산 시스템과 암호학의 기초를 설명하고 어떻게 데이터를 안전하게 보관하는지 알려줍니다. 암호화폐의 메커니즘과 탈중앙화 가상 머신인 이더리움을 사용하여 애플리케이션을 개발하는 방법을 익히게 될 것입니다. 여러 가지 블록체인 솔루션도 살펴보고 리눅스 재단에서 주관하여 블록체인 기술의 발전을위해 협업하고 있는 하이퍼레저 산하의 비즈니스 블록체인 프레임워크에 대해서도 소개합니다. 화폐 이외의 블록체인 솔루션을 구현하는 방법과 블록체인을 활용한 사물 인터넷, 블록체인 확장성, 그리고 이렇게 매혹적이고 강력한 블록체인 기술의 미래 전망에 관해서도 확인하실 수 있습니다.
## 이용 안내
모든 코드는 폴더별로 구성되어 있으며, 폴더명은 Chapter02와 같이 장별로 분리되어 있습니다.

코드느 다음과 같은 모습입니다.
```
pragma solidity ^0.4.0; 
contract TestStruct { 
  struct Trade 
  { 
    uint tradeid; 
    uint quantity; 
    uint price;  
    string trader; 
  } 
 
  // 이 구조체는 아래처럼 초기화하여 사용하면 된다. 
 
  Trade tStruct = Trade({tradeid:123, quantity:1, price:1, trader:"equinox"}); 
 
} 
```

* 이 책의 모든 예제는 우분투(Ubuntu) 16.04.1 LTS 지니얼(Xenial)과 맥 OS(Mac OS) 버전 10.13.2에서 개발되었습니다. 따라서, 우분투 혹은 다른 유닉스 계열 시스템을 사용하는 편이 좋습니다. 물론 윈도우든 리눅스든, 지원되는 아무 운영체제나 사용해도 되지만, 예제, 특히 설치 관련 예제는 운영체제에 맞게 변경해야 할 수도 있습니다.
* 암호화 관련 예제는 OpenSSL 1.0.2g [1 Mar 2016] 버전의 커맨드라인 도구로 개발했습니다.
* 이더리움 솔리디티 예제는 리믹스(Remix) IDE로 개발했으며, 리믹스 IDE는 https://remix.ethereum.org/ 에서 온라인으로 구할 수 있습니다.
* 이더리움 관련 예제는 이더리움 비잔틴(Ethereum Byzantine) 릴리스로 개발했습니다. 이 글을 쓰는 시점에서는 비잔틴이 최신 버전이며, https://www.ethereum.org/ 에서 다운로드할 수 있습니다.
* IoT 관련 예제는 빌로스(Vilros) 사의 라즈베리 파이(Raspberry Pi) 키트를 사용해 개발했지만, 적당한 다른 최신 모델이나 키트를 사용해도 됩니다. 구체적으로, IoT의 하드웨어 예제를 구축하는 데에는 라즈베리 파이 3 모델 B v1.2를 사용했습니다. IoT 예제에 필요한 Node.js 서버를 운영하고 관련 패키지를 다운로드하는 데는 Node.js v8.9.3과 npm v5.5.1을 사용했습니다.
* 스마트 계약을 배포(deployment)하는 일부 예제에 트러플(Truffle) 프레임워크를 사용했으며, 트러플 프레임워크는 http://truffleframework.com/ 에서 구할 수 있습니다. npm을 통해 최신 버전을 다운로드해도 됩니다.

## 관련 도서 상품

### 에이콘출판사
* [블록체인 완전정복 2/e](http://acornpub.co.kr/book/mastering-blockchain-2e)
* [블록체인 해설서](http://acornpub.co.kr/book/blockchain-guide)
* [블록체인 기술과 혁신적 서비스 개발 활용](http://acornpub.co.kr/book/blockchain-application)
* [블록체인 개념구축](http://acornpub.co.kr/book/blocks-chains)
* [비트코인과 블록체인, 탐욕이 삼켜버린 기술](http://acornpub.co.kr/book/bitcoin-blockchain)
* [이더리움을 활용한 블록체인 프로젝트 구축](http://acornpub.co.kr/book/blockchain-projects)

### 팩트출판사
* [Mastering Blockchain](https://www.packtpub.com/big-data-and-business-intelligence/mastering-blockchain?utm_source=github&utm_medium=repository&utm_campaign=9781787125445)
* [Building Blockchain Projects](https://www.packtpub.com/big-data-and-business-intelligence/building-blockchain-projects?utm_source=github&utm_medium=repository&utm_campaign=9781787122147)
* [Blockchain and Cryptocurrency (Bitcoin, Ethereum) Essentials [Video]](https://www.packtpub.com/application-development/blockchain-and-cryptocurrency-bitcoin-ethereum-essentials-video?utm_source=github&utm_medium=repository&utm_campaign=9781788990837)
