---
title: "최소 작용의 원리와 해밀턴의 원리에 대해 — Ch.1 헤론의 반사 법칙"
date: 2025-03-12
categories: [series]
tags: [최소작용, 광학, 헤론, 반사법칙]
series: "least-action"
toc: true
toc_sticky: true
---

## 1. 헤론의 반사 법칙(Heron's Principle of Reflection)

헤론(10년경 ~ 70년경)은 고대 이집트에서 태어나 알렉산드리아에서 태어난 고대 그리스인 발명가이자 수학자였다. 헤론은 기하학과 광학에서 많은 업적을 남겼는데, 헤론의 공식(Heron's formula)과 헤론의 반사 법칙(Heron's Principle of Reflection)이 그 예이다.

삼각형 세변의 길이를 알고 있을때, 삼각형의 넓이를 구하는 헤론의 공식

$$S = \sqrt{s(s-a)(s-b)(s-c)}$$

$$\text{where } s = \frac{a+b+c}{2}$$

헤론은 특히 광학에 있어 중요한 소식이 된 **헤론의 반사 법칙(Heron's principle of reflection)**을 만들었는데, 한번 살펴보도록 하자.

**헤론의 반사 법칙(Heron's Principle of Reflection)**은 빛의 경로를 최소화하는 방향으로 반사가 일어난다는 것이다. 이 법칙은 굴절과 같은 다른 광학 현상에서 설명되지 않았으나 반사 법칙에 대해 잘 설명되었다.

### 헤론의 반사 법칙의 증명

![헤론의 반사 법칙](/assets/images/least-action/ch1-heron-reflection.png){: .align-center}
*헤론의 반사 법칙(Heron's Principle of Reflection)*
{: .text-center}

우리가 알고 있는 반사 법칙은 먼저 입사각과 반사각의 크기는 항상 같다는 것이다. 이것은 헤론의 반사 법칙(Heron's Principle of Reflection)으로 부터 설명되는데, 어떻게 입사각과 반사각이 같음을 알려주는 것일까?

위의 그림과 같이 빛이 A로부터 출발하여 반사면의 P 지점에 도달하여 반사되고, B에 도달한다고 하자. 그리고 B지점이 반사면에 대칭되어 대응되는 지점을 B'이라고 하자. 그렇다면 경로 AP+PB는 AP+PB'과 같다. 왜냐하면 PB = PB'이기 때문이다.

헤론의 반사 법칙(Heron's Principle of Reflection)에 의하면, 빛은 빛의 경로를 최소화하는 방향으로 반사가 일어난다고 하였다. 이때 빛의 경로의 길이를 **광학적 경로 길이(Optical Path Length, OPL)**라고 한다. 따라서, OPL을 최소화하는 문제가 되어야 하므로 OPL $\overline{AP}+\overline{PB'}$는 최소가 되어야 한다. 따라서, $\overline{AP}+\overline{PB'}$의 최소 경로는 직선 $\overline{AB'}$과 같다.

즉, 점 P는 직선 AB' 위에 놓여 있으므로, 맞꼭지각에 의해 각도 알파와 감마가 서로 크기 같다. 각도 베타와 감마는 서로 같으므로, 즉, 입사각과 반사각이 같다.

---

이와 같은 헤론의 반사 법칙(Heron's Principle of Reflection)은 반사 현상을 잘 설명한다. 하지만 굴절과 같은 광학적 현상을 일반적으로 설명하는데 무리가 있었다. 따라서 굴절과 같은 광학적 현상을 일반적으로 설명하기 위한 **페르마 원리(Fermat's Principle)**이 등장하게 되었다.

---

> **챕터 이동**
>
> [이전 챕터: Ch.0 — 소개](/series/least-action-ch0/) \| [다음 챕터: Ch.2 — 페르마의 원리](/series/least-action-ch2/)
