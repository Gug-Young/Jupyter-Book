---
title: Re-usable data
---

시뮬레이션을 하고 결과 그림을 뽑으면 너무 많아서 어디에 있는지 확인이 어려운 경우가 있다.

```{figure}./PASTE_IMAGE/2025-11-14-07-31-10.png
:label: img:too-many-files
:alt: too-many-files
Kuramoto-model을 연구하면서 만들어진 파일들, 어떤 위치에 어떤 그림 혹은 코드가 있는지 확인하기 어렵다.
```
해당 경우 `ipynb`에 `# | label: `을 걸어주면 해당 그림이 어디에서 왔는지 쉽게 확인이 가능하다. `{ref}`나 `@`혹은 `[](#label)`를 해주에서 인용이 가능하다. 추가적으로 `# 그림에 대한 설명`을 해주면 어떤 그림인지도 알 수 있다.

>`@img:kuramoto_mf2_r_time` -> @img:kuramoto_mf2_r_time  
>`[](#img:kuramoto_mf2_r_time)` -> [](#img:kuramoto_mf2_r_time)  
>`{ref}'img:kuramoto_mf2_r_time'` -> {ref}`img:kuramoto_mf2_r_time`

또한 해당 그림을 `{figure}`를 이용해 `markdown`에 입력 할 수 있다.

:::{figure}#img:kuramoto_mf2_r_time
:label: Order parmeter at ($K=6,m=6,N=5000)
다른 파일에 있는 결과 그림
:::

또한 `# | fig-caption:`이나 `# | caption:`을 사용하고, `cell`에 `tag` `remove-input`을 걸어주면 추가적인 설명 없이 그림을 입력할 수 있다.

![](#fig:paper_fig_1)

만약 `{grid}`를 사용하면 여러가지 그림을 배치할 수 있다.

:::{grid} 2
![](#fig:paper_fig_1)

![](#fig:paper_fig_1_ver2)
:::

## 실시간 적용 가능성
다른 파일에서 해당 그림을 편집하는 경우 편집한 결과가 바로 적용된다.
:::{figure}#img:ramdom_walk_hist2d
:label: fig:Random_walk
Random walk를 통해서 얻어진 결과
:::

## Table 인용
다른 파일에 있는 `pandas`등으로 출력된 테이블 데이터를 다른 문서에서 출력이 가능하다.
![](#tbl:airport_data)


## Interactive figure
`Altair`나 `plotly`를 사용하면 결과물로 HTML을 출력하며, `HTML`으로 출력된 이미지를 받아서 출력할 수 있다.
[다른 페이지](./99 test.md)
::::{grid} 2

:::{card}
:header: Altair
:link: https://altair-viz.github.io/
Altair는 ‘선언적(Declarative)’ 시각화 라이브러리로,
시각화를 "무엇을 나타낼지" 중심으로 표현한다.
내부적으로 Vega-Lite 규격을 사용하기 때문에 구조적으로 매우 안정적이다.
:::

:::{card}
:header: Plotly
:link: https://plotly.com/python/
Plotly는 Python 기반의 고급 인터랙티브 시각화 라이브러리로,
줌/팬/툴팁/레이어 조작 등 웹 기반 상호작용을 기본으로 제공한다.
대부분의 차트는 JavaScript 없이 Python 코드로 생성된다.
:::

:::{figure}#img:Altair
:label: fig:Altair-graph
해당 [링크](https://altair-viz.github.io/altair-tutorial/notebooks/06-Selections.html)에 있는 example code를 사용한 interactive graph
:::

:::{figure}#img:plotly
:label: fig:Plotly-go
해당 [링크](https://plotly.com/python/mixed-subplots/)에 있는 example code를 사용한 interactive graph
:::
::::
asdasdadsad


또한 해당 `interactive graph`는 [다른 링크](./99_test.md)에서도 작동한다.
