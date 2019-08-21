---
title: "Tensorflow 예제 1 연습!"
date: 2019-08-22 04:56:00 -0400
categories: tensorflow exercise 
---
드.디.어. 텐서플로우 예제를 돌려보았다.
참고한 링크는 https://pinkwink.kr/1080 이다.
텐서플로우를 사용하는 것에 의의를 두었기 때문에 train set과 test set을 구별하지 않은, 정말 기본적인 예제이다.
링크에 자세한 설명이 나와있지만, 생초보인 나는 나를 위한 설명을 해보겠다. 
저랑 비슷한 왕왕왕초보님덜 두눈뜨고 잘 따라오세유 노빠꾸예유~~

<h3>1. tensorflow랑 numpy 두 개 import하기 </h3>
<div class="colorscripter-code" style="color:#010101;font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important; position:relative !important;overflow:auto"><table class="colorscripter-code-table" style="margin:0;padding:0;border:none;background-color:#fafafa;border-radius:4px;" cellspacing="0" cellpadding="0"><tr><td style="padding:6px;border-right:2px solid #e5e5e5"><div style="margin:0;padding:0;word-break:normal;text-align:right;color:#666;font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important;line-height:130%"><div style="line-height:130%">1</div><div style="line-height:130%">2</div><div style="line-height:130%">3</div><div style="line-height:130%">4</div><div style="line-height:130%">5</div><div style="line-height:130%">6</div></div></td><td style="padding:6px 0;text-align:left"><div style="margin:0;padding:0;color:#010101;font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important;line-height:130%"><div style="padding:0 6px; white-space:pre; line-height:130%"><span style="color:#a71d5d">import</span>&nbsp;tensorflow&nbsp;as&nbsp;tf</div><div style="padding:0 6px; white-space:pre; line-height:130%"><span style="color:#a71d5d">import</span>&nbsp;numpy&nbsp;as&nbsp;np</div><div style="padding:0 6px; white-space:pre; line-height:130%">&nbsp;</div><div style="padding:0 6px; white-space:pre; line-height:130%">tf.set_random_seed(<span style="color:#0099cc">777</span>)</div><div style="padding:0 6px; white-space:pre; line-height:130%"><span style="color:#066de2">print</span>(tf.__version__)</div><div style="padding:0 6px; white-space:pre; line-height:130%"><span style="color:#066de2">print</span>(<span style="color:#63a35c">"Hello"</span>)</div></div></td><td style="vertical-align:bottom;padding:0 2px 4px 0"><a href="http://colorscripter.com/info#e" target="_blank" style="text-decoration:none;color:white"><span style="font-size:9px;word-break:normal;background-color:#e5e5e5;color:white;border-radius:10px;padding:1px">cs</span></a></td></tr></table></div>
tensorflow랑 numpy를 사용하기 위해 가져왔다. 
<strong>Numpy란?</strong> (C언어로 구현된) 파이썬 라이브러리로, Numerical Python의 줄임말이다. 즉, 벡터 및 행렬 연산 등 고성능의 수치계산을 위해 제작되었다. 근데 주로 array(행렬) 단위의 연산을 수행한다. 
Numpy를 사용하기 위해서는 import numpy를 써야한다. 근데 코드에서 편의를 위해 좀더 짧게 줄여서 쓰기 위해서 as np를 덧붙인다. 즉, numpy를 가져오는데 np라는 이름으로 가져온다는 것이다.
<strong>Numpy의 함수들</strong>에 대해서는 이번주 내로 정리해서 올릴 예정이다. <br>

과연 tf.set_random_seed(777)은 무엇을 의미하는 걸까.. 
seed는 난수값(랜덤값)이라고 한다. 이때 seed안에 일정한 숫자(이 경우 777)를 넣으면, 일정한 패턴의 숫자들만 계속 나온다고 한다. 
예를 들어 이 코드를 한번 돌리면 234, 341, 61, 234, ... 다시 한번 돌려도 234, 341, 61, 234, ... 이런 식으로. 
(보충설명이 필요하다)

tf의 버전을 확인하기 위해서 tf.__version__을 print해보았고, 1.14버전임을 알았다. 

<h3>2. 입출력데이터를 설정해주기 </h3>

