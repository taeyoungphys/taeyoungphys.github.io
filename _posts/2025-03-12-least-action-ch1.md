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

**헤론(Heron of Alexandria, 10년경~70년경)**은 고대 이집트에서 태어나 알렉산드리아에서 활동한 고대 그리스인 발명가이자 수학자였다. 헤론이 활동한 알렉산드리아는 당시 학문의 중심지였으며, 그 유명한 **알렉산드리아 도서관(Library of Alexandria)**이 위치한 곳이기도 하다.

헤론은 수학, 광학, 역학 등 다양한 분야에서 업적을 남겼다. 역학 분야에서는 증기의 힘으로 회전하는 장치인 **아이올로스의 공(Aeolipile)**을 고안하여, 최초의 증기 기관의 원형을 만든 것으로도 알려져 있다. 수학에서는 **헤론의 공식(Heron's Formula)**이 대표적이고, 광학에서는 **헤론의 반사 법칙(Heron's Principle of Reflection)**이 대표적이다.

삼각형 세변의 길이를 알고 있을때, 삼각형의 넓이를 구하는 헤론의 공식

$$S = \sqrt{s(s-a)(s-b)(s-c)}$$

$$\text{where } s = \frac{a+b+c}{2}$$

헤론은 특히 광학에서 중요한 원리를 제안하였는데, 바로 **헤론의 반사 법칙(Heron's Principle of Reflection)**이다. 이 법칙은 빛의 경로를 최소화하는 방향으로 반사가 일어난다는 것이다. 굴절과 같은 다른 광학 현상까지는 설명하지 못했으나, 반사 법칙에 대해서는 훌륭하게 설명되었다.

헤론의 반사 법칙은 단순히 반사 현상을 기술하는 것을 넘어, **자연이 어떤 물리량을 최소화하는 방향으로 작동한다**는 아이디어의 씨앗이 되었다. 이 아이디어는 이후 약 1600년이 지나서야 페르마에 의해 다시 발전하게 된다.

### 헤론의 반사 법칙의 증명

![헤론의 반사 법칙](/assets/images/least-action/ch1-heron-reflection.png){: .align-center}
*헤론의 반사 법칙(Heron's Principle of Reflection)*
{: .text-center}

우리가 알고 있는 반사 법칙은 먼저 입사각과 반사각의 크기는 항상 같다는 것이다. 이것은 **헤론의 반사 법칙(Heron's Principle of Reflection)**으로부터 설명되는데, 어떻게 입사각과 반사각이 같음을 알려주는 것일까?

위의 그림과 같이 빛이 A로부터 출발하여 반사면의 P 지점에 도달하여 반사되고, B에 도달한다고 하자. 그리고 B지점이 반사면에 대칭되어 대응되는 지점을 B'이라고 하자. 그렇다면 경로 $\overline{AP}+\overline{PB}$는 $\overline{AP}+\overline{PB'}$과 같다. 왜냐하면 $\overline{PB} = \overline{PB'}$이기 때문이다.

헤론의 반사 법칙에 의하면, 빛은 빛의 경로를 최소화하는 방향으로 반사가 일어난다고 하였다. 이때 빛의 경로의 길이를 **광학적 경로 길이(Optical Path Length, OPL)**라고 한다. 따라서, OPL을 최소화하는 문제가 되어야 하므로 OPL $\overline{AP}+\overline{PB'}$는 최소가 되어야 한다. 따라서, $\overline{AP}+\overline{PB'}$의 최소 경로는 직선 $\overline{AB'}$과 같다.

즉, 점 P는 직선 AB' 위에 놓여 있으므로, 맞꼭지각에 의해 각도 알파와 감마가 서로 크기 같다. 각도 베타와 감마는 서로 같으므로, 즉, 입사각과 반사각이 같다.

---

이와 같은 **헤론의 반사 법칙(Heron's Principle of Reflection)**은 반사 현상을 잘 설명한다. 하지만 굴절과 같은 광학적 현상을 일반적으로 설명하는데 무리가 있었다. 따라서 굴절과 같은 광학적 현상을 일반적으로 설명하기 위한 **페르마의 원리(Fermat's Principle)**가 등장하게 되었다.

---

> **챕터 이동**
>
> [이전 챕터: Ch.0 — 소개](/series/least-action-ch0/) \| [다음 챕터: Ch.2 — 페르마의 원리](/series/least-action-ch2/)
