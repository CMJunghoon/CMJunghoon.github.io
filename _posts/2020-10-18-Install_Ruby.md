---
title: Ruby 설치 / 업데이트 / 제거 ( MacOS )
author: CoolMint
date: 2020-10-18 15:00:00 +0800
categories: [MacOS, Ruby]
tags: [Ruby]
---

> macOS는 기본적으로 Ruby가 설치되어 있습니다.

## 1. rbenv이용하여 Ruby 설치.

```shell
$ brew install rbenv
```

## 2. 환경 설정파일 명령어 추가.

```shell
$ cd                   # Root로 이동
$ nano .bash_profile   # nano 편집기로 파일 열기
```

아래 명령어 추가.

```shell
eval "$(rbenv init -)"
```

> control + x 버튼을 누르면, 변경 내용을 저장 여부 Y 누르고, 엔터 치면 편집기 닫힘.

## 3. Ruby 버전 설치

```shell
$ rbenv install 2.7.0  # Ruby 원하는 버전을 입력하여 설치
$ rbenv rehash         # 설치한 Ruby 설치 후 재 실행
```

## 4. Ruby 버전 변경

```shell
$ rbenv global 2.7.0   # 시스템 전체를 지정한 버전으로 지정합니다. 
$ rbenv local 2.7.0    # 현재 디렉토리만 사용할 버전 지정합니다.
```

## 5. 적용된 Ruby 버전 확인

```shell
$ rbenv versions
```

## 6. Ruby 버전 삭제

```shell
$ rbenv uninstall 2.7.1  # 지정한 버전을 삭제 합니다.
```
