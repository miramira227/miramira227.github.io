---
title: "텐서플로우 다운로드"
date: 2019-08-22 04:00:00 -0400
categories: tensorflow install
---
텐서플로우 install을 하는 중이다.. 
텐서플로우 관련 프로젝트를 하나 맡게 되었는데, 
정말 너무 문외한이라서 걱정되는 마음에 오늘부터 커피 2잔 마시고 밤새 열심히 공부해보려고 한다. <br><br>
정말 생으로 처음 접하는 입장에서, 텐서플로우, 아나콘다, 파이썬 세 개의 분류가 어려웠던 관계로
일단은 이 세 가지의 개념을 정리하려고 한다.

그 전에 일단 
https://docs.anaconda.com/anaconda/user-guide/getting-started/
이걸 보면서 아나콘다를 설치하였다. (신기해..)

<strong>1. 텐서플로우란?<strong> <br>  
<strong>2. 아나콘다란?<strong> <br>
<strong>3. 아나콘다 설치방법<strong> <br>
  이제 서서히 깃헙 블로그 관리를 해야하지 싶다. 코드를 올리고 싶은데...
  1. https://www.anaconda.com/distribution/ 
  이 사이트에서 Windows용 Python 3.7을 다운로드 받았다. 그 전에 
  python --version
코드를 통해 자신이 사용 중인 파이썬의 버전을 확인하자! 그리고 그 뒤로 전부 Next 버튼을 누른다. 
  2. 파이썬을 활성화하고, 주피터 노트북을 install한다. 
  여러 사이트들을 참고하느라 뒤죽박죽으로 봐버렸는데, 
  <div class="colorscripter-code" style="color:#010101;font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important; position:relative !important;overflow:auto"><table class="colorscripter-code-table" style="margin:0;padding:0;border:none;background-color:#fafafa;border-radius:4px;" cellspacing="0" cellpadding="0"><tr><td style="padding:6px;border-right:2px solid #e5e5e5"><div style="margin:0;padding:0;word-break:normal;text-align:right;color:#666;font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important;line-height:130%"><div style="line-height:130%">1</div><div style="line-height:130%">2</div><div style="line-height:130%">3</div><div style="line-height:130%">4</div><div style="line-height:130%">5</div><div style="line-height:130%">6</div><div style="line-height:130%">7</div><div style="line-height:130%">8</div><div style="line-height:130%">9</div></div></td><td style="padding:6px 0;text-align:left"><div style="margin:0;padding:0;color:#010101;font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important;line-height:130%"><div style="padding:0 6px; white-space:pre; line-height:130%">#&nbsp;And</div><div style="padding:0 6px; white-space:pre; line-height:130%">x_data&nbsp;=&nbsp;np.array([[0,&nbsp;0],&nbsp;</div><div style="padding:0 6px; white-space:pre; line-height:130%">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[0,&nbsp;1],</div><div style="padding:0 6px; white-space:pre; line-height:130%">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[1,&nbsp;0],&nbsp;</div><div style="padding:0 6px; white-space:pre; line-height:130%">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[1,&nbsp;1]],&nbsp;dtype=np.float32)</div><div style="padding:0 6px; white-space:pre; line-height:130%">y_data&nbsp;=&nbsp;np.array([[0],</div><div style="padding:0 6px; white-space:pre; line-height:130%">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[0],</div><div style="padding:0 6px; white-space:pre; line-height:130%">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[0],</div><div style="padding:0 6px; white-space:pre; line-height:130%">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[1]],&nbsp;dtype=np.float32)</div></div></td><td style="vertical-align:bottom;padding:0 2px 4px 0"><a href="http://colorscripter.com/info#e" target="_blank" style="text-decoration:none;color:white"><span style="font-size:9px;word-break:normal;background-color:#e5e5e5;color:white;border-radius:10px;padding:1px">cs</span></a></td></tr></table></div>
