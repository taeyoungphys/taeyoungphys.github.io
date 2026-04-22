---
title: "최소 작용의 원리와 해밀턴의 원리에 대해 — Ch.5 해밀턴의 원리와 변분법"
date: 2025-04-22
categories: [series]
tags: [최소작용, 라그랑주, 해밀턴, 라그랑지안, 변분법, 뉴턴역학]
series: "least-action"
toc: true
toc_sticky: true
---

## 1. 라그랑주와 해밀턴

앞선 챕터에서 모페르뒤가 작용이라는 물리량을 정의하고, 오일러가 이를 적분의 형태로 확장한 것까지 살펴보았다. 하지만 아직 몇 가지 과제가 남아 있었다.

- 일반적인 접근 방법의 개발
- 현대적인 표현 방법
- 왜 최소 작용의 원리가 작동하는지에 대한 설명

이 과제를 해결하는 데 기여한 사람이 바로 **조제프루이 라그랑주(Joseph-Louis Lagrange, 1736–1813)**와 **윌리엄 해밀턴(William Rowan Hamilton, 1805–1865)**이다.

해밀턴은 $T - V$를 **라그랑지안(Lagrangian)** $L$로 정의하였고, 경로에 따른 라그랑지안의 시간 적분을 정류(stationary)하게 만드는 원리를 **해밀턴의 원리(Hamilton's Principle)**로 명명하였다. 해밀턴의 원리는 최소 작용 원리의 보다 현대적인 표현 방법이다.

그렇다면 모페르뒤의 원리에서 해밀턴의 원리가 어떻게 유도되는지 살펴보자.

---

## 2. 모페르뒤의 원리에서 해밀턴의 원리로

![모페르뒤에서 해밀턴으로의 유도](/assets/images/least-action/ch4-maupertuis-to-hamilton.png){: .align-center}
*모페르뒤의 원리에서 해밀턴의 원리로의 유도 과정*
{: .text-center}

모페르뒤의 원리로부터 출발한다.

$$\delta S_0 = 0 \quad \Rightarrow \quad \delta \int mvds = 0$$

속도의 정의 $v = \dfrac{ds}{dt}$로부터 $ds = vdt$를 대입하면,

$$\delta \int mv^2 dt = 0$$

운동에너지 $T = \dfrac{1}{2}mv^2$이므로 $mv^2 = 2T$를 대입하면,

$$\delta \int 2T\, dt = 0 \quad \Rightarrow \quad \delta \int (T + T)\, dt = 0$$

여기서 역학적 에너지 보존 $E = T + V$로부터 $T = E - V$를 대입하면,

$$\delta \int (T + E - V)\, dt = 0$$

이를 정리하면,

$$\delta \int (T - V)\, dt + \delta \int E\, dt = 0$$

$\delta \int E\, dt = \delta(Et)$이고, 곱의 변분 규칙에 의해 $\delta(Et) = E\delta t + t\delta E$이다. 오일러가 발견한 조건에 의해 에너지가 보존되므로 $\delta E = 0$이다. 따라서,

$$\delta \int (T - V)\, dt + E\delta t = 0$$

양 끝점이 고정되어 있으면 $\delta t = 0$이므로,

$$\boxed{\delta \int (T - V)\, dt = \delta \int L\, dt = 0}$$

이것이 바로 **해밀턴의 원리(Hamilton's Principle)**이다. 라그랑지안 $L = T - V$의 시간 적분을 **작용(Action)** $S$라 부르며, 이 작용이 정류(stationary)하는 경로가 실제 물체가 따르는 경로이다.

모페르뒤의 원리와 해밀턴의 원리의 차이를 정리하면 다음과 같다.

| | 모페르뒤의 원리 | 해밀턴의 원리 |
|---|---|---|
| 작용의 정의 | $S_0 = \int mvds$ | $S = \int (T - V)\, dt = \int L\, dt$ |
| 변분 대상 | 경로 (공간) | 경로 (시간) |
| 조건 | 에너지 보존 필요 | 양 끝점 고정 |

해밀턴의 원리가 보다 일반적인 이유는, 에너지 보존을 별도의 조건으로 요구하지 않고도 양 끝점만 고정하면 성립하기 때문이다.

---

## 3. 변분법 — 진짜 경로와 벗어난 경로

이제 해밀턴의 원리 $\delta S = 0$으로부터 어떤 물리가 나오는지 살펴보자. 이를 위해 라그랑주가 발전시킨 **변분법(Calculus of Variations)**을 사용한다.

라그랑주는 진짜 물체가 이동하는 경로를 **진짜 경로(true path)** $y(t)$로 생각하고, 그 이외의 경로를 진짜 경로에서 벗어난 경로 $q(t)$로 생각하였다.

![변분법 — 진짜 경로와 벗어난 경로](/assets/images/least-action/ch4-variational-path.png){: .align-center}
*진짜 경로 $y(t)$와 변분 경로 $q(t) = y(t) + \eta(t)$*
{: .text-center}

벗어난 경로 $q(t)$를 다음과 같이 쓸 수 있다.

$$q(t) = y(t) + \eta(t)$$

여기서 $\eta(t)$는 진짜 경로로부터의 편차이며, 양 끝점에서 $\eta(t_1) = \eta(t_2) = 0$이다. 즉, 출발점과 도착점은 고정되어 있으므로 편차 함수 $\eta(t)$는 양 끝에서 반드시 0이어야 한다.

---

## 4. 뉴턴의 제2법칙 유도

진짜 경로 $y(t)$에서의 작용 $S[y(t)]$와 벗어난 경로 $q(t)$에서의 작용 $S[q(t)]$의 차이를 생각해보자.

$$\delta S = S[q(t)] - S[y(t)] = 0$$

작용의 정의 $S = \int_{t_1}^{t_2} L\, dt = \int_{t_1}^{t_2} (T - V)\, dt$를 이용하여 전개하면,

$$S[q(t)] = \int_{t_1}^{t_2} \left( \frac{1}{2}m\left(\frac{dq}{dt}\right)^2 - V(q) \right) dt$$

$$S[y(t)] = \int_{t_1}^{t_2} \left( \frac{1}{2}m\left(\frac{dy}{dt}\right)^2 - V(y) \right) dt$$

$q = y + \eta$를 대입하고 $\eta$에 대해 1차까지만 전개하면,

$$\delta S = \int_{t_1}^{t_2} \left( m\frac{dy}{dt}\frac{d\eta}{dt} - \eta V'(y) \right) dt = 0$$

첫째 항에 **부분적분(integration by parts)**을 적용해보자.

$$\int_{t_1}^{t_2} m\frac{dy}{dt}\frac{d\eta}{dt}\, dt = \left[ m\frac{dy}{dt}\eta \right]_{t_1}^{t_2} - \int_{t_1}^{t_2} m\frac{d^2 y}{dt^2}\eta\, dt$$

경계 조건 $\eta(t_1) = \eta(t_2) = 0$에 의해 경계항은 사라진다. 따라서,

$$\int_{t_1}^{t_2} m\frac{dy}{dt}\frac{d\eta}{dt}\, dt = -\int_{t_1}^{t_2} m\frac{d^2 y}{dt^2}\eta\, dt$$

이를 대입하면,

$$\delta S = \int_{t_1}^{t_2} \left( -m\frac{d^2 y}{dt^2} - V'(y) \right) \eta\, dt = 0$$

$\eta(t)$는 임의의 함수이므로, 위 식이 모든 $\eta(t)$에 대해 성립하려면 괄호 안의 항이 0이어야 한다. 이를 **변분법의 기본 보조정리(Fundamental Lemma of Calculus of Variations)**라고 한다.

$$-m\frac{d^2 y}{dt^2} - V'(y) = 0$$

$F(y) = -V'(y)$ (힘은 퍼텐셜 에너지의 음의 기울기)이므로,

$$\boxed{F = ma}$$

이것은 바로 **뉴턴의 제2법칙(Newton's Second Law)**이다! 즉, 해밀턴의 원리(최소 작용의 원리)로부터 뉴턴 역학이 자연스럽게 유도된다.

---

이 결과가 의미하는 바를 생각해보자. 뉴턴은 $F = ma$라는 법칙을 **출발점**으로 삼아 역학을 구축하였다. 그런데 해밀턴의 원리에서 출발하면, $F = ma$가 출발점이 아니라 **결과**로 나타난다. 이는 곧 해밀턴의 원리가 뉴턴 역학보다 더 근본적인 원리일 수 있음을 시사한다.

실제로 해밀턴의 원리는 뉴턴 역학뿐만 아니라 전자기학, 일반상대성이론, 양자역학 등 현대 물리학의 거의 모든 분야에서 핵심적인 역할을 하고 있다. 이 시리즈에서 헤론의 반사 법칙으로부터 시작하여, 페르마의 원리, 베르누이의 아이디어, 모페르뒤의 작용을 거쳐 해밀턴의 원리까지 도달한 여정은, 물리학이 어떻게 점진적으로 더 일반적이고 근본적인 원리를 향해 나아가는지를 잘 보여준다.

---

> **챕터 이동**
>
> [이전 챕터: Ch.4 — 모페르뒤의 원리와 작용](/series/least-action-ch4/) \| 다음 챕터: 준비 중
