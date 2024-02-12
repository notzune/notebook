a technical standard for [[Floating-point arithmetic|floating-point arithmetic]] that addresses many problems found in the early implementation of floating-point. most hardware [[Floating-point unit (FPU)|floating-point units]] use this standard.

- _arithmetic formats:_ sets of [[Binary code|binary]] and decimal floating-point data, which consist of finite numbers (including signed zeroes, infinities, and special "not a number" values ([[NaN]]))
- _interchange formats:_ encodings (bit strings) that may be used to exchange floating-point data in an efficient and compact form
- _rounding rules:_ properties to be satisfied when rounding numbers during arithmetic and conversions
- _operations:_ arithmetic and other operations (such as [[Trigonometric functions|trig functions]]) on arithmetic formats
- _exception handling:_ indications of exceptional conditions (such as division by zero, overflow, _etc._)