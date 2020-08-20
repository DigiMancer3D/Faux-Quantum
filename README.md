# Faux-Quantum
Starting with building binary fields based on input data, eventually will also entangle the input or data based from the input to the binary field(s).

<a href="https://drive.google.com/uc?export=download&id=16ikTX7KYkfujEsIo-zaDsWEN58IBBKaS" target="_blank">Read more about the concept.</a>

The idea of building a binary field based on other data without containing that data is the first tackle. The working version (<sup><sub>hashlink below</sub></sup>) encodes the input to a Base64 string so this string is reversable back to our input. We also find the dec value of the Base64, character per character, output as a long string. After that it uses the base64 or equivalent dec string to find the a-number then an acceptable vlaue range based off the a-number (low-low | low-high | high-low | high-high). The first binary field (the field core) is generated based on the acceptable value range determinations. The final field (the minable field) is generated based on the end result of the field core. Every 3rd & 4th line in the final field checks for filter pass possiblity based on the previous two lines. 

Not being used nor coded-in yet, there is a programable section in the field core and final field during the filter-passes when a null-string is found. In order to use this section of the fields, the programable section needs be a series of options that's either on or off. The aviable room will differ per build.

Eventually field mining will be added to gain additional programmable sections as well as increase entropy of the field and gain new bit-positions.

The fields should be stored in Base64 or Base128. The Base-versions of the core and final field should be stored in seperate. The field core can be found in a single build final field but in a mined field with entropy will make finding the core much more difficult. A mined field without entropy will not make finding the core harder nor change the difficulty to retrace. 

Not yet coded is the mining of a field. In the concept paper there's two main ways to mine the field but there's room to grow. 

Entropy mining is using the Base64 of any selected sections or just the programmed sections to be used as the input to find another set of the same data as well as second field outputs (core and final). After this the two fields are merged (not yet determined in method for merging) for futhure entropy.

Non-Entropy mining has two methods, the first is entropy mining except the new block is placed either ontop or below the current block, this is switched or not switched per new final field block. 

The second type of non-entropy mining is simply finding missing bit-combinations of the previous block and adding it to the top or bottom of the current block forming a larger new block.

The entropy in mining is through the programming sections of fields and the merging process (zipper | null-swaps | swap-spots | every-Nth | merge-Rebuild). 

Another entropy process not yet coded is a No Knowledge Base Strings to use instead of the direct input. This is better explained in the concept paper.

A working early version of the Faux-Quantum Bits. <a href="https://itty.bitty.site/#/data:text/html;charset=utf-8;bxze64,XQAAAALyWgAAAAAAAAAeHMqHyTY4PyKmqfkwr6ooCXSIMxPQ7ojnoHG+l0DNJitIMjjLGB16qpP/XaxDaCrfB5mUyay5ezuja/nwmp2aMA8SS2jGrX5PlFhwj7ml570SmS4GBQaUvOv55Mg61ViW1zYEQT4HXJyU3yjNYfnU6i/8mjLLPK5tc4AVvRzDPjcKjBMeyuyuZ44iHp+pSOuzGQKbTuD2jWFqlvOHMWb+kiMwVTP1JayXfSatAZ5UTv61WrNq854otpfYJvR1AgxVUsCEaw6O+E6wMDuhY/JxwDEacYYJHSa4WBJ1md1tqAHEhBx+oSmfJVbcYbCAdI0unf5URQGBad8z4KeLOEt34BrkXHtqhlQhzu1mabIrqjhMAM14QuejxrxxvuVbnIyxLDzVqbGw0u50Z97jkzsAjvoW5EIn5TQhGOPqm0f0rlIY4dpJRsXXEZjp9MFkI/jm6DGPo2aMANizDghb922L2DD6JYgI99cezrB6lrdQXxYrdulB0ZjrSr6KcV36dUgtf9Eotox7X8R+ylwJIQMej0GFN5gPZvzxxYX8Fim1YPRizaEbEdLSydlUV9mms/Xk10mLdhShp8+q5XkxsfftYYcG5hUlpaz9a/RA/x4MNI1FVxBEBRZA71NCqWPNoCj+uB5ViJ4U+pTjl3//0fipHllQ4/cwF8nPElPo4JPPrp9+0qoK4nNnCfbTkM6BZj8oU57GG4bOeZ6TaWXtRa6azGXfZE81kXW1pzZgsUBc9ZconR12ZwHcDjBm+nVNCXDKdzmam155+mrQk11G5iyCjHlwI1PhVJoF7acIPKUURCaXwv0kjxn1in6dcmL5r1BH9UdXeFx4+xBGP4h/Ij0pwKd6p2FfA1ZLulHj7/Rr2i3pLgG8Qh3uU/8Ne+Xkb6O8YCMkSWYjp2rN3joMWr+7uq7ETJa9F9DHdLZJOIumwk5D7ZZNf8sWKWi4xhTM/qiYHhYwiF8h3j0iXX5Om2iiSGkmjpK/dN3jakTdag3WFxQk3ZwHI+h3AOC7FvZ9yxc9cfkhpKfB3/53H54tmq0f6NF3QX3GsZou7/V1iAgVTkCeZVV8kEbq0Jpxj5Nle4q2TENLr3dDZgO0OpFOe+fj8a/qrjKSVeEuCKwNwWs9A+3nDW1ByNyZLqjTI/O9NGGx76mb47QycKuxmEINaAcdRmRBQ/JJGYc4T5aVIyrb2rBUEaaIebymj5dGPcl+3qBt2HpdFcP2mMMlHMYXIfYI8s9pdDItfPqBMB9hQVH7ij/kkCpqPyRNCmOTl8i0fzxJjzk9BBmofQxsj/CRLB8pFE6iKG0Ugai8Qo/oMSXmJM1vhfjVdmvg+GSz1qhdqjhsD0u+sNJ0JwinIi25A93lJ2c4xCLqSdlADCabrTCYAUfMV0mllsQAujY4+FjRe4p6l48+vhSZPyyXObGVfqijSiBXAoLJA34GGL8YHrpXdaNfI2nH7n3q3yW0v971qJ5jygUqWJxfP8NeYpJfSNhrF2UPo3+ehNPQy4QW4UESfgFRYkgwhpjRGJKYnAfxICq5/fAP5NPENjiACYLM/RR2ugmeHVNnud8MK/zHo0jbDKWv7r24gql7jvJPUt4/dU6JZSqPbVFWYUhH6M/PQqovxHv7d2xItWxVi34iHFsbtIPR7+cJt6faaf/ByXhE0M9xNmInqcagEySyjGSHndyWYj8Z/gt4G3EHcYUuCKEcTd2sSAgeH/owaFBmnz1DmhCiJNEZc8wddtML0eqppHFTQ/Z+0d6oOEiM+H0RHi+BN4FBQqXRRrlOP64QXix5HGXMvuB3nhudk7jljXCUbMVa7DClX0vN/G0pmNRGpCpIJWLYfpBTtps/4D7MDKdpxQs6kaEPKd4E/5oX+GulnMGDHJL4HbqvN8XizgGbFuiFgMcllgjs2T4c6hjRwMftEvzJU3ai93h2O9lgNj+gkMDLSMIxdmEuwnBrc0NoHFbUtLvGQlX+mkATHuU1P2Zec8tGol5mNjM1OHZ2jOSHxNFQgjkT0Pvb79881PDb6EY1uaZytBPbWEf62GcrMMadkJEMwmdgGcnl63/NLATAB4w52i+R8VpLV8/dxvn3yJgC1v1VOaP/Lf34RovPRQPdH+4gNfd0omd0tiXCPtG15bogGllg1t9vlS2PEsuAWCLa1W44DgCFc+X9SWbWSVUzqi3UhAh7QKbWI1KnZdGBuaESB3QJrCAhawmoIq1a18CQ5SjI4LP5/8KIIPxMEIveRyVAu+e/VVdkiNSk3+J+REEp4UjOw6GVWb/kATQgjTFMn1vQWcG1i8+HIMSrVVg/Are27fdXRqiwICbdZQeucO6KsVjobgauY/Bn6qRAPE59WikaxHmqzzvzwAGW2xr6AdQ91x/bUS/1Ed54FsTHPI2KqTsGX71ywVxj5H9Ti7ajJJ5qVhrjw89ZXfJNFwMWc0jTNquaKLluahhPgIsd+QffTmizaT1W6xWF/OE2Yx45DLJcQAExc95NlSvLViRB9qULZQF/Vovh0TPmdpuCMTwgixEBQUSU8t8H/MIPGygtvkfK9oLwapzAPOqobHyqUxuMzh7iWqIQE6DZkB7AgURUBlwV/c8HkJ1YdaEkYmeR71FS5YAjignhSSfAB+ks40zbjXbDlaIPRwpQPFTjhh/t0r9PO237gNkBZ6sS89BpmARQ0L+wg68J6//Sm5VG+bMRknnoym8kGp7JniXnYOVcOHuMb/g7z79L2aStzamN4OZWE49xGY9Vm+YABDhbhfLciCLo2YZAkVVL/rn7LkwEFX+ZEESn4zE1cgy5Xt7fyqSyDYEvNICeX77TtGfLdFNyb8vgHFgjKvnp4JmO54mFgpmObUN6u0VzSkPkuxu/eWRONObzjXVQvacJcg1R4KNkucm0gmDNgdjY6SxPFUbs7EgBi3I2vpgYgWEcAHVi/rNI8wEi31p6EAviB4Kb08refPlwXYoUj2sa8qthFfb8Mb/1QMmuVScMpgMi6HIEqJNEKyLuMpjM8V5YVIPAstVoL0DWNiCubAbrq3KiKoGHsL8SoRyMvyu1XiQdBo6q3Wz0IYhZTLLrpdhS8ysHUbYweRbYjEyVzeBIT4PGh4TcbX5g4pp8VZ4eyesd046NIWQlx4+m5WTQhhWtpT49v0pDxiivlxKucjJjCW1io+AaQUnamF4fkPCBdFXogdYjZBAo/2rv95dDBKzRWZtSmQGc8fI5d7omYaYPltEBkb9aTOgfqzH6wFVkgELP0qE7jQZ8bgYTJbxc/QrtWkbyZzJ2itISE/QGfVk6/k5IcdiCcqA2aE+PWq2cq8lnh1nBDlj5G2Kl78NkqwO9T38tEiLF6wVk4Tk38vnyili4DRtE/UjfEEIn+VC3loqmzW9EZFFnziwppK2pjbFY/EfdZxPIw+cj+rFBzC8pj+b7TVvzRv8ZIXnKOmPvEtvzmhbesnNZ02LQqh6d2sllaWN7nhhLF4JDk4fs1kZyhATxbv5rV4rSJiK8a1dN2twi8MLunNry0Ajo8ZHoLvbGx54nh1pXtu5D8al2GXPWjtVIVPtaVnNprf1EuYd7PCpH9mJPJo1019nL2dZFFdJbIHg7tKXBTnByBeG8/yhsrxPjSDCdwOF1Ytu2OfPNEE77u0Fkn/269Dkj56Ju3EvFC9VNHHXNj+5MZ64WGmh8t3lTh4vKm/tWFjGxfgL7h0eR3Uiw05dnyuMXfAQg+9vz6iTBQVp2rLlXek4T10AX0YlNQ5PG8iPlfy0OVMThMr9TGnTamXnIsUJzgFV/5tGX59ptjRX74CdaUzt+aISIiZLLiesa67YntyRUpWd3qGx+mEHfvWhy6nUI38bmK5YYQt0Ho5JO2hSQxNuxTm+vGIJ1lS3YYpwOyxCaq6gUezvjjSW5ZcO/yMe5XJKIVs1Zd2zG6LcQW5L6A9jbmiZdLUUrqXIBxdldHGxsfxTTQdPPhSveC1WA2qkg0RghNZM9uMxS5q78fJ6tsFeM/uvfFjxRVia+nnkwqbdhE5H9JgqqNM37tJUDPo+1tAmpY2JMBVcxCCu434ix9fOT8bSDAv1CNlbMJ2tcQhYYK4lLe2knNL3RR+CTLcftbAhgp/yFkQjohJLidckN8uEM9LSRIktGDgSBcwj6WtnF+IoZHmFfWIwxCXFkqjFQthbv7HFX/sky1dPn+qwkW63u15mNecrVK2KcoEPbjXnHwXR8ncumbpAAy47hyekYb7pshSleMBu7ptVmqBQaApz5hMUZwF0sFcyDtBUJWFqbDDM/9f7hg2pcomPdBip8g6q3m1VvYxRHU/gWHc7bgQwx2faFGekIFnu9acTw/cDcUsGbdgzPdCE7t7bBUsYxKKuQhAn4RVqtKLC9PU8cJ4QEsMw2GN6xF5Q6Hvmp90hMI6bQH0qI923dwi050DI7/i3mZNHQ2d+wEGlnpQuUtrzxmVCz3kAr4Q3ND0AnTGxnunCMxcvNiUPhGGrt/tAOMgzH0WUnjy64P6QJbaB4UVWL8RmlWYwJS4vRStQzCZJ5gfcA023UK004e4PXXrDRCBRUyqJZ4Lg5LnD8nRSMb2TOMiEyGj1hHW/STbIgLaMVRxAS/o0Lr7Y4mRaS3ln0PC/zKLgLHDDxabdgyRdasfRUZdZoUCLBM6PgQRnVOXyfFxCVnT9P5dr1E3M7OxezrZoIgW/VO91vp+52snrIWuoyumRSnQo7gK4VZZI5XRC+S4IunBq+al01nz8mLcCHZZsZu5VeJzH9wOHg9rUwoHQnBArL29q8HFiUq3yXPTaybCpDOSu8C6kVI1GcxdBvLupZCeJ/Xwxf2Z/tsYA50Syrhzq/WNgrI7I8dcLooFReTez6vlFm7mj6BZ1e7G79E/RTdjNO57ROrI/2Za+gHeDjG/pgxXBK0e59LKzTCCtX3Bw1qTbMRz583wQtODWHhymD5vATi8gSom3qUD7RSJ1VfXuqtoKb1ucYO+1IjkZGhlZSG2us6ZvQPiGb/Xm6TBhQqngGyvlR18covhPJzfwyBO79KX0jOVkwyY2ikwRjHfjhHRqLzerHLPwwTFS0thXTvpBkBzBebfsRmpYpQmKTwb9MMzaKsPTqGYPYFLwQxNTht/Y5C5tJCgqsxP02jdcHcbVnWs2NtfiSowqsMQNZLrzb9hm8MHeM/bvYBJvDsMeNs/+27LmC" target="_blank" rel="noopener noreferrer">Just click here. </a>

# <i>What Can This Do Right Now?</i>

### &nbsp; &nbsp; Build Zero-Knowledge-Proofs with low tech
### &nbsp; &nbsp; Build User Specific Binary Cores <sup>(<sub>up to 6 characters long</sub>)</sup>
### &nbsp; &nbsp; Determine Atomic Value of input <sup>(<sub>up to 28 characters</sub>)</sup>
### &nbsp; &nbsp; Build Corresponding Binary Field based on User's Core
### &nbsp; &nbsp; Define an <i>abse64</i> [<i><b>a - Base64</b></i>], Binary <i>Square</i>, & <i>Base64 Signature</i> of the built User Binare Core
### &nbsp; &nbsp; Perform first wave of field mining, non algorithmic, logical comparision mining

# <i>What's Still Needed?</i>
### &nbsp; &nbsp; Algorithmic Mining <sup>(<sub><i>field mining</i> & <i>entangled mining</i></sub>)</sup>
### &nbsp; &nbsp; Algorithmic Entangling to BIN Field
### &nbsp; &nbsp; Private BIN Core Signature
### &nbsp; &nbsp; Webb Data Storage based on Priv-BIN Core Signature locking
### &nbsp; &nbsp; Programable Field Input to Use During Mining & Core Building

# <i>What are Known Issues?</i>

## Binary Core becomes predictable on output after 7 characters:
### After 7 characters the core output can be guessed based on if input is even or odd.

## <s>Binary Core doesn't output correctly.</s>
### <s>The first line of the binary core build determines some of the remainder and is not always outpting correctly based on input.</s>

## <s>Binary Field doesn't output correctly when binary core isn't outputing correctly.</s>
### <s>Related to other known issue, the Binary field will not output correctly when the binary core isn't outputing correctly.</s>
<hr>
### <s>Striked Out Items are No-Longer Issues or Added Features</s>
