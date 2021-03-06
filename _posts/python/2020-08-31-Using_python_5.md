---
layout: post
title: "파이썬에서 유용한 기능 정리(1) - enumerate, zip, randint"
author: Peter
categories: [Python]
image: https://user-images.githubusercontent.com/52132160/91701420-3db1f400-ebb2-11ea-8d9e-f11cad524fc0.png

sitemap:
changefreq: daily
priority: 1.0
---

---

이번 포스트에서는 파이썬을 사용하면서 유용하게 사용할 수 있는 기능들을 공유 해 보려고 한다.
지금부터 소개할 세 가지 기능 모두 눈으로는 알고 있으나 막상 사용하려면 잘 기억이 안나서 이번 기회에 정리 해 보았다.

---

### 1. enumerate

- 반복문을 사용 시 사용하게 되는데 인덱스 번호와 원소를 tuple 형태로 변환하여 반환시켜 준다.
  ![image](https://user-images.githubusercontent.com/52132160/91699005-954e6080-ebae-11ea-8c3f-473c29a3454f.png)
  <br>

![image](https://user-images.githubusercontent.com/52132160/91699231-f1b18000-ebae-11ea-9a2b-05b2654b0fc6.png)

이렇게 인덱스랑 원소를 따로 출력할 수도 있다.
<br><br>

---

### 2.zip

- zip은 같은 길이의 인덱스를 인덱스끼리 매칭시켜 하나의 tuple로 변환시켜주는 기능인데 여러 개의 리스트를 처리할 때 용이하다.
  ![image](https://user-images.githubusercontent.com/52132160/91699687-9b910c80-ebaf-11ea-94c1-5adaacaeb334.png)
  <br>

![image](https://user-images.githubusercontent.com/52132160/91699963-0f331980-ebb0-11ea-8d40-7d495a47895b.png)
만약 이런 식으로 리스트의 길이가 맞지 않으면 그냥 무시(오류x)하고 일치하는 인덱스끼리만 매칭된다.
<br><br>

![image](https://user-images.githubusercontent.com/52132160/91700118-53261e80-ebb0-11ea-9bdb-3da1c5b1fb1d.png)
리스트 3개도 거뜬하다!
<br><br>

---

### 3. randint

- randint는 학교에서 과제가 나오면 무조건 쓰게 되있는 녀석인데 지정한 범위 내에서 난수 값을 생성해 준다.
  ![image](https://user-images.githubusercontent.com/52132160/91700423-d34c8400-ebb0-11ea-9f12-a1077b1de58c.png)
  위 그림과 같이 0 ~ 100 사이의 난수를 생성하여 반환한다.
  <br><br>

![image](https://user-images.githubusercontent.com/52132160/91700666-35a58480-ebb1-11ea-959d-820db9b42a30.png)
이렇게 변수에다가 설정해서 사용하는 경우가 많다.
<br><br>

다음에 또 유용한 게 있으면 가져 오도록 하겠다.

---
