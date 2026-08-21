
Link: [https://cryptohack.org/courses/modular/course_details/]

## Greatest Common Divisor:
  - I believe this is our introduction into algorithms using Euclidean algorithm as an example. You might recognise or remember this from your days in school, I do.
  - In essence, the way this algorithm works is we can represent larger of the two numbers provided as a multiple of the smaller number plus the difference, and we keep repeating this until the difference (or remainder) becomes zero.
  - For example, if we are given `GCD of 8, 12` we can represent it as `12 = 8*1 + 4`, then `8 = 4*2 + 0`. On the first representation, we have to add 4 and include it in the RHS for the equation to hold true, then further applying the algorithm, we do not need to add anything into the second step for the equation to hold true, thus we know 4 is the GCD. This is how I solved this one.

## Extended GCD:
  - This is quite literally an extension to the Euclidean algorithm, with the addition of Bezout's coefficients which is often used in RSA. While mathematically working out, it is done by working our way back from the last line and substituting values to match the required equation.
  - In implementing with python, you may opt to use recursion as it is very efficient when used correctly here to find the gcd, then work it back up to find u and v.
  - It is worth noting that one of the coefficients will always be negative, and this is the smaller number asked of us.

## Modular Arithmetic 1:
  - A simple but effective introduction to how MOD function or operation is applied. Also helps the learner understand that intuitively, big numbers dont always equal a bigger mod result.
  - Solving it is easy, simply divide then find the remainder, and smaller of the two remainder integers is the flag.

## Modular Arithmetic 2:
  - This is an application of a Fermat's Little Theorem, which can serve as a quick trick to find the answer to what could otherwise be a very long calculation.
  - Basically, if 'a' is any number, and 'p' is a prime, then anything in the format of `a^p-1 (mod p)` is always equal to 1.
  - Funny of them to ask if we needed a calculator, I understand if one decides to use a calculator to compute it themselves though.

## Modular Inverting:
  - Personally, this is where I started to get a good feel of mod notation and working with it in my head. This is my first exposure to it.
  - I didn't compute the answer as I was probably expected to, using the theorem, I simply figured subsituting 'd' with 9 yields the right answer. Oh well.
