# test md
hyper link를 걸어서 어떻게 보이는지 확인하기 위한 markdown. 만약 해당 부분이 보인다면 아래의 각주[^test_md]를 통해 그림을 넣을 수도 있다.

:::{tip} 수식 인용 확인
:class: dropdown
{ref}`eq:eq_of_motion`
라벨의 이름이 겹치지 않으면 가능하며, 겹치는 경우 오류가 발생한다.
또한 `![](#eq:eq_of_motion)`으로 수식을 보여주는 것도 가능하다.
![](#eq:eq_of_motion)
:::

:::{tip} Table 인용 확인
:class: dropdown
{ref}`tbl:table`
또한 `![](#tbl:table)`으로 테이블을 보여주는 것도 가능하다.
![](#tbl:table)
:::

:::{tip} Fig 인용 확인
:class: dropdown
{ref}`fig-altair-horsepower`와 같이 이전에 사용한 그림을 인용하거나 `![](#그림 라벨)`를 사용해서 해당 문서에 embeding 할 수도 있다.
![](#fig-altair-horsepower)
{ref}`table`
:::

:::{card} 🏷 원래 문서로 돌아가기
:link: ./Intro.md
이 부분을 클릭하면 보고 있던 화면으로 돌아갑니다.
:::


[^test_md]:![](PASTE_IMAGE/2025-11-13-04-40-16.png) **Test Fig**: 해당 화면이 보일것이다. 
