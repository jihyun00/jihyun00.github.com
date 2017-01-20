---
layout: page
title: AWS EC에 ssh로 접속할 때 주의할 점
categories: technique
comments: true
author: Jihyun Choi
permalink: /technique
---

별 거 아니긴 한데 다음에 생성할 떄 까먹을까봐 기록해둔다.

### 인스턴스 생성 초기에 Security groups 설정하기

1. Security 그룹 들어가서 group 하나 created 하고
2. created 한 group에 Inbound tab에 edit
3. HTTP, SSH 추가

### 인스턴스 SSH 접속하기

- 인스턴스에 접속하기 위해 ssh key가 필요함. ssh key를 다운받거나 기존에 있는 걸 사용.

### SSH 권한 설정

- 처음 ssh key를 다운받으면 644로 설정되어 있음. ssh 접속시 권한이 너무 열려있다며 접속이 안됨.
- 400 으로 권한 설정을 바꿔주면 해결.
