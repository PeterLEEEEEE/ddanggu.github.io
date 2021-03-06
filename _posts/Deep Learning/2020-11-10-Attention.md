---
layout: post
title: "Transformer를 공부하기 위해 얻은 지식들"
author: Peter
categories: [NLP]
image: https://user-images.githubusercontent.com/52132160/91701420-3db1f400-ebb2-11ea-8d9e-f11cad524fc0.png

sitemap:
changefreq: daily
priority: 1.0
comments: true
---

---

Transformer는 이전에 공부하였던 RNN, LSTM과 같은 내용과는 많이 다른 점을 알 수 있었다. 문제는 하나를 공부하기 위해 계속 위로 올라가서 다시 공부해야하는 일이 생겼지만 알게모르게 처음 공부하였을 때 애매한 지식으로 넘어갔던 부분은 채울 수 있었다.

---

### Attention Mechanism

<p>
트랜스포머를 들어가기 전 항상 언급되는 것이 있다, 바로 Attention Mechanism 이다.(어텐션으로 부르도록 하겠다)
어텐션은 어떻게 등장하게 되었을까? 기존에 RNN 기반의 seq2seq 모델이 번역 모델로서 널리 사용되고 있었다. 하지만 치명적인 문제가 존재하였는데, 바로 번역 역할을 하는 context vector가 fixed size 즉 고정된 사이즈 이기 때문에 입력 문장이 길어지면 모든 정보를 담지 못해 올바른 번역을 해내지 못하는 문제였다.
<br>
<br>
그래서 다음과 같은 Attention Mechanism이 제안되었다. 바로 인코더에서 나온 각각의 state를 모두 활용하는 것이다. 기존에 인코더를 모두 거쳐 하나의 context vector로 나오는 것을 dynamic하게 만들어, 모든 단어가 context vector로서 활용하여 fixed size에서 dynamic size로 그 한계를 극복해낸 것이다. 다른 장점도 있다, 인코더에 있는 모든 state를 활용하며 중요도가 높은 단어에 집중할 수 있도록 설계도 가능해졌다.
</p>
<hr>
### Transformer

<p>
위에서 언급하였듯이 Transformer는 기존 RNN 혹은 LSTM의 순차적 처리 구조가 아닌 병렬식 처리 구조이다.
기존 RNN에서는 문장의 단어의 위치 및 순서 정보를 잘 활용해 자연어처리에서 널리 사용되었으나 Transformer는 Positional Encoding 즉 인코더 및 디코더 입력 값마다 상대적 위치정보를 그대로 더해준다는 것이 그 차이점이다.
</p>
---
