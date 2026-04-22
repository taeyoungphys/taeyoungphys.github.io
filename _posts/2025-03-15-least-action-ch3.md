---
title: "최소 작용의 원리와 해밀턴의 원리에 대해 — Ch.3 광학과 역학을 연결시킨 베르누이의 아이디어"
date: 2025-03-15
categories: [series]
tags: [최소작용, 베르누이, 최속강하곡선, 사이클로이드, 등시곡선]
series: "least-action"
toc: true
toc_sticky: true
---

## 3. 광학과 역학을 연결시킨 베르누이의 아이디어

페르마의 원리는 광학에서만 중요한 원리일 것으로 치부되었다. 하지만 베르누이는 놀랍게도 페르마의 원리를 역학과 연결시켰다. 어떻게 역학의 영역으로 페르마의 원리를 접목시켰을까?

**요한 베르누이(Johann Bernoulli, 1667~1748)**는 스위스의 수학자이다. 라이프니츠, 뉴턴 등의 사람과 동시대의 사람이다. 그의 아들인 다니엘 베르누이도 제법 유명하다. 다니엘 베르누이(Daniel Bernoulli, 1700~1782)는 네덜란드 출생의 스위스인으로 수학, 의학 등 다양한 분야를 연구했다. 특히 요한 베르누이의 아들인 다니엘 베르누이는 유체역학에서 베르누이 방정식(Bernoulli's equation)과 같은 업적을 세웠다.

요한 베르누이는 당대 유명한 두 문제에 대해 고심했다. 바로 최속 강하 곡선(Brachistochrone Curve)와 등시 곡선(Tautochrone Curve)이다. 베르누이는 이 문제를 꽤 놀라는 해결책을 제시했다. 그건 무엇이었을까?

### 최속 강하 곡선(Brachistochrone Curve)

![최속 강하 곡선](/assets/images/least-action/ch3-brachistochrone.png){: .align-center}
*최속 강하 곡선(Brachistochrone Curve) — 사이클로이드가 직선이나 포물선보다 빠르다*
{: .text-center}

최속 강하 곡선은 영어로 Brachistochrone curve라고 하는데, 이는 그리스어로 Brachisto는 shortest를 의미하고 chrone는 time을 의미한다. 최속 강하 곡선 문제는 균일한 중력장 내에서 임의의 두 점 사이를 지날때 이동하는 시간이 가장 작은 곡선을 구하는 문제이다.

먼저, 베르누이는 에너지 보존으로부터 다음과 같은 식을 유도하였다.

$$T + V = E \; (\text{const.})$$

$$\frac{1}{2}mv^2 + mgy = E$$

$$\frac{1}{2}mv^2 = E - mgy$$

이때, 총 에너지 $E$는 상수이므로, 0이라고 가정해보자. 그렇다면,

$$\frac{1}{2}mv^2 = -mgy$$

$v$와 $y$에 대한 식을 작성하려고 하는데, $-$ 부호가 있어 곤란하다. 따라서 $-$부호를 없애주기 위해 $y$ 대신 $-y$를 넣어주면 편리하다. 즉, 좌표축의 기준점을 다음과 같이 변경한다.

그렇다면 $y$ 대신 $-y$를 대입하여 식을 더욱 간편하게 만들 수 있다. 따라서,

$$\frac{1}{2}mv^2 = mgy$$

$$v = \sqrt{2gy}$$

이때, $v$는 속력이므로 0 보다 크거나 같은 만 취하면 된다.

여기에서 베르누이는 최속 강하 곡선 문제를 굴절 문제로 변환하게 된다. 단, 굴절면이 무수히 많게 아래 그림의 예시와 같이 만들었다.

![굴절면 분할](/assets/images/least-action/ch3-refraction-layers.png){: .align-center}
*최속 강하 곡선을 A와 B 사이에 무수히 많은 굴절면을 나눈 것으로 생각했다*
{: .text-center}

또한, 위의 에너지 보존에서 유도된 높이와 속도의 관계를 이용해, 다음과 같이 굴절면을 설정한다.

또한, 각 매질의 속도는 다음과 같이 높이와 다음과 같은 관계가 있다.

$$v_1 = \sqrt{2gy_1}$$

$$v_2 = \sqrt{2gy_2}$$

또한, 베르누이는 스넬의 법칙과 굴절률 관련 식을 통해 다음과 같은 관계를 얻어내었다.

$$n_1 \sin\theta_1 = n_2 \sin\theta_2$$

$$\frac{c}{v_1}\sin\theta_1 = \frac{c}{v_2}\sin\theta_2$$

$$\frac{\sin\theta_1}{\sqrt{y_1}} = \frac{\sin\theta_2}{\sqrt{y_2}}$$

이것을 매질 2와 매질 3에 대해 적용하는 방법으로 나아가면, 다음과 같이,

$$\frac{\sin\theta_1}{\sqrt{y_1}} = \frac{\sin\theta_2}{\sqrt{y_2}} = \cdots = \frac{\sin\theta_i}{\sqrt{y_i}} = \cdots$$

$$\frac{\sin\theta_i}{\sqrt{y_i}} = \text{const.}$$

즉 $y$와 굴절각에 상관없이 이 모두를 만족하기 위해서 위와 같은 상수 관계가 성립해야 한다. 베르누이는 높이와 굴절각에 대한 관계식을 찾아내었고, 이후 이 비율이 바로 **사이클로이드 곡선(cycloid curve)**임이 밝혀졌다.

따라서, 베르누이는 최속 강하 곡선(Brachistochrone Curve)는 사이클로이드 곡선(Cycloid Curve)임을 찾아낸 셈이다.

### 등시 곡선(Tautochrone Curve)

![등시 곡선](/assets/images/least-action/ch3-tautochrone.png){: .align-center}
*등시 곡선(Tautochrone Curve) — 시작점에 관계없이 최저점 도달 시간이 동일하다*
{: .text-center}

베르누이는 더욱 나아가 등시 곡선 문제에 도전했다. 등시 곡선은 영어로 tautochrone curve라고 하는데, 그리스어로 tauto는 same이란 뜻이고, chrone은 time이란 뜻이다.

등시 곡선은 균일한 중력장에서 마찰없이 가장 낮은 점까지 도달하는 물체의 시간이 곡선 위의 시작점과 상관없이 동일한 곡선을 의미한다. 베르누이는 위와 유사한 방법으로 등시 곡선 또한 사이클로이드 곡선이며, 따라서 **등시 곡선(Tautochrone Curve)과 최속 강하 곡선(Brachistochrone Curve)과 동일한 문제**임을 밝혀내었다.

---

베르누이는 등시 곡선과 최속 강하 곡선이 같은 문제임을 밝혀내고 다음과 같이 말하였다.

> *"In this way I have solved at one stroke two important problems — an optical and a mechanical one — and have achieved more than I demanded from others: I have shown that the two problems, taken from entirely separate fields of mathematics, have the same character."*
>
> — Johann Bernoulli

이 글을 보고 있는 여러분은 이제 광학에서의 페르마 원리가 역학 문제로 귀결될 수 있음을 본 것이다. 스넬의 법칙으로 역학적 문제를 다루었다는 뜻은 곧 페르마 원리로 역학적 문제를 다룰 수 있음을 의미한다. 광학적 문제와 기계적 문제는 서로 다른 물리 현상으로 보이지만 **최소 시간의 원리라는 공통된 수학적 원리**를 가지게 된다는 것이다.

여기까지 따라온 여러분에게 어떠한 의문이 들 수 있다. 바로 최소 시간의 원리를 역학 문제에 어떻게 명확히 정의할 수 있는지에 대해서이다. 이에 대해 설명하기에 앞서, 경로에 관한 중요한 물리량에 대해 말하지 않을 수 없다. 바로 모페르튀의 원리(Maupertuis's Principle)과 **작용(Action)**이다.

---

> **챕터 이동**
>
> [이전 챕터: Ch.2 — 페르마의 원리](/series/least-action-ch2/) \| 다음 챕터: *준비 중*
