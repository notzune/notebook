in [[Trigonometry|trigonometry]], trigonometric identities are [[Equality|equalities]] that involve [[Trigonometric functions|trigonometric functions]] and are true for every value of the occurring [[Variables|variables]] for which both sides of the equality are defined.

they are different from the [[Triangle identities|triangle identities]] which involve angles but also some length of a triangle.

# [[Pythagorean trigonometric identity]]

the basic relationship between the [[Sine and cosine|sine and cosine]] is given by the Pythagorean identity:

$$
\sin^2\theta+\cos^2\theta=1
$$

where $\sin^2\theta$ means $(\sin\theta)^2$ and $\cos^2\theta$ means $(\cos\theta)^2$.

this can be viewed as a person of the [[Pythagorean theorem]] and follows from the equation $x^2+y^2=1$ for the [[Unit circle|unit circle]]. this equation can be solved for either the sine or the cosine:

$$
\begin{align}
\sin\theta=\pm\sqrt{1-\cos^2\theta} \\
\\
\cos\theta=\pm\sqrt{1-\sin^2\theta} \\
\end{align}
$$

where the sign depends on the [[Quadrant|quadrant]] of $\theta$.

dividing this identity by either $\sin^2\theta,\cos^2\theta$, or both yields

$$
\begin{align}
&1+\cot^2\theta=\csc^2\theta \\
\\
&1+\tan^2\theta=\sec^2\theta \\
\\
&\sec^2\theta+\csc^2\theta=\sec^2\theta\csc^2\theta \\
\end{align}
$$

some other identities that are particularly useful especially in [[Partial integration|partial integration]]:

$$
\begin{align}
\sin^{2}x+\cot^{2}x&=1 \\
\\
1+\tan^{2}x&=\sec^{2}x \\
\\
1+\cot^{2}x&=\csc^{2}x \\
\\
\cos^{2}x&=\frac{1+\cos2x}{2} \\
\\
\sin^{2}x&=\frac{1-\cos2x}{2} \\
\end{align}
$$

## Table of trigonometric functions in terms of the other five

| in terms of | $\sin\theta$ | $\csc\theta$ | $\cos\theta$ | $\sec\theta$ | $\tan\theta$ | $\cot\theta$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $\sin\theta=$ | $\sin\theta$ | $\frac{1}{\csc\theta}$ | $\pm\sqrt{1-\cos^2\theta}$ | $\pm\frac{\sqrt{\sec^2\theta-1}}{\sec\theta}$ | $\pm\frac{\tan\theta}{\sqrt{1+\tan^2\theta}}$ | $\pm\frac{1}{\sqrt{1+\cot^2\theta}}$ |
| $\csc\theta=$ | $\frac{1}{\sin\theta}$ | $\csc\theta$ | $\pm\frac{1}{\sqrt{1-\cos^2\theta}}$ | $\pm\frac{\sec\theta}{\sqrt{\sec^2\theta-1}}$ | $\pm\frac{\sqrt{1+\tan^2\theta}}{\tan\theta}$ | $\pm\sqrt{1+\cot^2\theta}$ |
| $\cos\theta=$ | $\pm\sqrt{1-\sin^2\theta}$ | $\pm\frac{\sqrt{\csc^2\theta-1}}{\csc\theta}$ | $\cos\theta$ | $\frac{1}{\sec\theta}$ | $\pm\frac{1}{\sqrt{1+\tan^2\theta}}$ | $\pm\frac{\cot\theta}{\sqrt{1+\cot^2\theta}}$ |
| $\sec\theta=$ | $\pm\frac{1}{\sqrt{1-\sin^2\theta}}$ | $\pm\frac{\csc\theta}{\sqrt{\csc^2\theta-1}}$ | $\frac{1}{\cos\theta}$ | $\sec\theta$ | $\pm\sqrt{1+\tan^2\theta}$ | $\pm\frac{\sqrt{1+\cot^2\theta}}{\cot\theta}$ |
| $\tan\theta=$ | $\pm\frac{\sin\theta}{\sqrt{1-\sin^2\theta}}$ | $\pm\frac{1}{\sqrt{\csc^2\theta-1}}$ | $\pm\frac{\sqrt{1-\cos^2\theta}}{\cos\theta}$ | $\pm\sqrt{sec^2\theta-1}$ | $\tan\theta$ | $\frac{1}{\cot\theta}$ |
| $\cot\theta=$ | $\pm\frac{\sqrt{1-\sin^2\theta}}{\sin\theta}$ | $\pm\sqrt{\csc^2\theta-1}$ | $\pm\frac{\cos\theta}{\sqrt{1-\cos^2\theta}}$ | $\pm\frac{1}{\sqrt{\sec^2\theta-1}}$ | $\frac{1}{\tan\theta}$ | $\cot\theta$ |
## Reflections, shifts, and periodicity

### Reflections

when the direction of a [[Euclidian vector]] is represented by an angle $\theta$, this is the angle determined by the free vector (starting at the origin) and the positive $x$-unit vector. the same concept may also be applied to lines in a [[Euclidean space]], where the angle is determined by a parallel to the given line through the origin and the positive $x$-axis. if a line (vector) with direction $\theta$ is reflected about a line with direction $\alpha$, then the direction angle $\theta\prime$ of this reflected line (vector) has the value

$$
\theta\prime=2\alpha-\theta
$$

the values of the trig functions of these angles $\theta,\theta\prime$ for specific angles $\alpha$ satisfy simple identities: either they are equal, have opposite signs, or employ the complementary trig function. these are also known as reduction formulae.

| $\theta$ reflected in $\alpha=0$ ([[Even and odd functions\|odd/even]] identities) | $\theta$ reflected in $\alpha=\frac{\pi}{4}$ | $\theta$ reflected in $\alpha=\frac{\pi}{2}$ | $\theta$ reflected in $\alpha=\frac{3\pi}{4}$ | $\theta$ reflected in $\alpha=\pi$ (compare to $\alpha=0$) |
| ---- | ---- | ---- | ---- | ---- |
| $\sin(-\theta)=-\sin\theta$ | $\sin(\frac{\pi}{2}-\theta)=\cos\theta$ | $\sin(\pi-\theta)=+\sin\theta$ | $\sin(\frac{3\pi}{2}-\theta)=-\cos\theta$ | $\sin(2\pi-\theta)=-\sin(\theta)=\sin(-\theta)$ |
| $\cot(-\theta)=+\cos\theta$ | $\cos(\frac{\pi}{2}-\theta)=\sin\theta$ | $\cos(\pi-\theta)=-\cos\theta$ | $\cos(\frac{3\pi}{2}-\theta)=-\sin\theta$ | $\cos(2\pi-\theta)=+\cos(\theta)=\cos(-\theta)$ |
| $\tan(-\theta)=-\tan\theta$ | $\tan(\frac{\pi}{2}-\theta)=\cot\theta$ | $\tan(\pi-\theta)=-\tan\theta$ | $\tan(\frac{3\pi}{2}-\theta)=+\cot\theta$ | $\tan(2\pi-\theta)=-\tan(\theta)=\tan(-\theta)$ |
| $\csc(-\theta)=-\csc\theta$ | $\csc(\frac{\pi}{2}-\theta)=\sec\theta$ | $\csc(\pi-\theta)=+\csc\theta$ | $\csc(\frac{3\pi}{2}-\theta)=-\sec\theta$ | $\csc(2\pi-\theta)=-\csc(\theta)=\csc(-\theta)$ |
| $\sec(-\theta)=+\sec\theta$ | $\sec(\frac{\pi}{2}-\theta)=\csc\theta$ | $\sec(\pi-\theta)=-\sec\theta$ | $\sec(\frac{3\pi}{2}-\theta)=-\csc\theta$ | $\sec(2\pi-\theta)=+\sec(\theta)=\sec(-\theta)$ |
| $\cot(-\theta)=-\cot\theta$ | $\cot(\frac{\pi}{2}-\theta)=\tan\theta$ | $\cot(\pi-\theta)=-\cot\theta$ | $\cot(\frac{3\pi}{2}-\theta)=+\tan\theta$ | $\cot(2\pi-\theta)=-\cot(\theta)=\cot(-\theta)$ |

### Shifts and periodicity

| Shift by one quarter period | Shift by one half period | Shift by full periods | Period |
| ---- | ---- | ---- | ---- |
| $\sin(\theta\pm\frac{\pi}{2})=\pm\cos\theta$ | $\sin(\theta+\pi)=-\sin\theta$ | $\sin(\theta+k\cdot2\pi)=+\sin\theta$ | $2\pi$ |
| $\cos(\theta\pm\frac{\pi}{2})=\mp\sin\theta$ | $\cos(\theta+\pi)=-\cos\theta$ | $\cos(\theta+k\cdot2\pi)=+\cos\theta$ | $2\pi$ |
| $\csc(\theta\pm\frac{\pi}{2})=\pm\sec\theta$ | $\csc(\theta+\pi)=-\csc\theta$ | $\csc(\theta+k\cdot2\pi)=+\csc\theta$ | $2\pi$ |
| $\sec(\theta\pm\frac{\pi}{2})=\mp\csc\theta$ | $\sec(\theta+\pi)=-\sec\theta$ | $\sec(\theta+k\cdot2\pi)=+\sec\theta$ | $2\pi$ |
| $\tan(\theta\pm\frac{\pi}{4})=\frac{\tan\theta\pm1}{1\mp\tan\theta}$ | $\tan(\theta+\frac{pi}{2})=-\cot\theta$ | $\tan(\theta+k\cdot\pi)=+\tan\theta$ | $\pi$ |
| $\cot(\theta\pm\frac{\pi}{4})=\frac{\cot\theta\mp1}{1\pm\cot\theta}$ | $\cot(\theta+\frac{pi}{2})=-\tan\theta$ | $\cot(\theta+k\cdot\pi)=+\cot\theta$ | $\pi$ |
