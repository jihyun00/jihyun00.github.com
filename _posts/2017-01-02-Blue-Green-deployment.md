---
layout: page
title: Blue-Green deployments
categories: technique
comments: true
author: Jihyun Choi
tags: [deployments, blue, green]
permalink: /technique
---

# Blue-Green deployments

Blue, Green 은 동일한 환경이다. 운영이 Blue 환경에서 일어나고 있다고 가정해보자.
무언가 추가를 해서 새로운 소프트웨어를 릴리즈하고 싶다. 이럴 경우 Green 환경에 새로운 소프트웨어를 추가하고, 운영을 Green 환경으로 변경시킨다.
문제가 생기면, Blue 환경으로 다시 rollback 할 수 있다.

Blue, Green 환경으로 변경시키는 방식은 매우 간단하다. Blue에서 Green 환경으로 변경시키고 싶으면 라우터가 Green 환경을 가리키게 하면 된다.
