---
layout: post
title: First order optimality condition
chapter: "04"
order: 3
---

<script type="text/x-mathjax-config">
MathJax.Hub.Config({
    displayAlign: "center"
});
</script>

> $$
> \text{min}\_{x} \quad f(x) \quad \text{  subject to  } x \in C
> $$

위 convex problem에서 objective function $f$가 미분 가능할 때, 아래의 부등식은 optimal point $x$에 대한 필요충분 조건이 된다.

> $$\nabla f(x)^{T}(y-x) \geq 0 \text{ for all } y \in C$$

우리는 이를 *first-order condition for optimality*라고 부른다. $\nabla f(x)^{T}(y-x) = 0$는 set $C$의 접점 x를 지나는 hyperplane이고, $- \nabla f(x)$는 $x$에서 optimal point로 이동하는 방향이다. 이때 위의 부등식을 만족한다면 set $C$가 $- \nabla f(x)$의 반대방향인 half-space에 포함된다는 것이므로 $x$는 optimal point가 된다.</br>
<center>
![](https://wikidocs.net/images/page/18337/first-order-condition.png)</br>
**[Fig1] geometric interpretation of first-order condition for optimality [3]**
</center>

#### Important special case
$C = R^n$일때(unconstrained optimization일때), optimality condition은 다음과 같이 정의된다.
> $$\nabla f(x) = 0$$

마찬가지로 −∇f(x) 는 x에서 optimal point로 이동하는 방향인데, $\nabla f(x) = 0$라는 것은 $f$를 최소화시키기 위해 $x$에서 더이상 이동할 곳이 없다는 것과 같다.