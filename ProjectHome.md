# Qt용 한글 입력기 모듈 qimhangul #

이 프로젝트는 Qt의 입력 모듈 기능을 이용해서 한국어 입력 모듈을 개발하는 프로젝트입니다.

## 기능 ##
  * 지원하는 자판: 두벌식, 두벌식 옛글, 세벌식 390, 세벌식 최종, 세벌식 순아래, 세벌식 옛글
  * 한글 조합과 한자 변환을 위한 내부 구현은 [libhangul](http://code.google.com/p/libhangul)을 사용하고 있습니다.

## 설치 방법 ##
가급적 직접 빌드하지 말고 각 배포판에서 제공하는 바이너리를 사용하시기 바랍니다.
데비안의 경우
```
 # apt-get install qimhangul-qt4
```
명령으로 설치 가능합니다.

## 빌드 방법 ##
```
 $ qmake -makefile
 $ make
 # make install
```

## 설정 방법 ##
환경 변수 `QT_IM_MODULE`이 다음과 같은 값중 하나로 설정되어야 합니다.
```
 hangul2 : 두벌식
 hangul2y : 두벌식 옛글
 hangul39 : 세벌식390
 hangul3f : 세벌식최종
 hangul3s : 세벌식순아래
 hangul3y : 세벌식옛글
 hangulro : 로마자
 hangulahn : 안마태
```

## 버그 리포트 ##
  * http://code.google.com/p/qimhangul/issues/list

## 참고 ##
  * libhangul: http://code.google.com/p/libhangul/
  * imhangul: http://code.google.com/p/imhangul/