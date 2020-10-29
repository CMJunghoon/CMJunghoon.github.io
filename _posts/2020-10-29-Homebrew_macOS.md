---
title: Homebrew ( macOS 패키지 관리자 )
author: CoolMint
date: 2020-10-29 11:00:00 +0900
categories: [MacOS, Homebrew]
tags: [Homebrew]
---

> masOS용 패키지 관리자
> 
> [Homebrew]([macOS 용 패키지 관리자 — Homebrew](https://brew.sh/index_ko))

## 1. 설치

```shell
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

## 2. 패키지 설치

> 터미널으로 사용하고 패키지 설치 ( 루비 / zsh 등등 )

```shell
$ brew install rbenv
```

> UI가 있는 Application 설치 ( 슬랙 / 텔레그램 / 제플린 등등 )

```shell
$ brew cask install slack
```

## 3. 패키지 Update

```
$ brew update rbenv
$ brew cask update slack
```

## 4. 패키지 삭제

```shell
$ brew remove rbenv
$ brew cask remove slack
```

## 5. 설치한 패키지 List 만들기

```shell
$ brew list --formula > brewList.txt  # 맥에 설치된 brew list을 파일로 작성

$ brew list --cask > brewCaskList.txt # 맥에 설치된 brew cask list을 파일로 작성
```

## 6. 패키지 List 설치

```shell
$ brew install $(cat brewList.txt)
$ brew install cask $(cat brewList.text)
or

$ brew install $(<brewList.txt)
$ brew install cask $(<brewList.text)
```
## 7. 참고
[https://whitepaek.tistory.com/3](https://whitepaek.tistory.com/3)
