If you don't understand what this means, see this writeup for an explanation on RSA.

At first glance, this may seem impossible. The modulus N is far too large to factor. However, there is a caveat. c = pow(m,e,n). However, what if m ^ e < n? Then the modulus never comes into play, and c = m ^ e. Not only that, but e in this case is very small: 3. We can clearly see that c is much smaller than n, meaning that it might just be possible that m ^ e < n. If that is the case, we can just take the cube root of c to find m (m ^ 3 = c so c = m ^ (1/3)).

These numbers are very large, so we need to make sure that our cube root is precise enough to list every digit. To do this in python, you can use a binary search.
