---
layout: post
title: PythonRPC
---

python으로 rpc 구현하기.

보편화된 서버개발 순서는 일반적으로 다음과 같다. 
 
  1. 패킷정의
  2. flow 작성
  2. 서버 적용, 클라이언트 적용
  3. 테스트

이러다보니 특정기능(패킷의 프로토콜 추가) 하나만 추가되어도 서버와 클라이언트에서 해야할 것들이 무척 성가시다. 그래서 최근에는 RPC(Remote Process Call)가 나오게 되었다. 
RPC(Remote Process Call)는 클라이언트에서는 함수를 호출하고 서버에서는 함수를 구현하여 통신하는 구조로 XML-RPC나 SOAP이 이에 속한다. RPC는 서버와 클라이언트 개발자가 프로토콜에 신경쓸 일이 없어져서 무척 편리하다. 그러나 단점으로는 생각보다 빠르지도 않고 설치에 적잖은 노력을 해야 한다.
python의 경우, 우분투에 빌트인 된 프로그램이다. 그리고 강력한 서드파티 엔진들이 많다. 아래 내용들은 python을 이용하여 다음과 같은 것들을 구현했다.

패킷 수정없이 서버에 신기능 추가
클라이언트에서 서버에 있는 리눅스 쉘과 파이썬 명령어를 리모트로 호출(RPC)

간단히 말해서 "Python으로 RPC(Remote Process Call)을 쉽게 따라해본다"가 목적이다.

[Python RPC](https://github.com/VintageAppMaker/PythonRPC)
