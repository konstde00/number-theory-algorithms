# Number theory algorithms

Implementations of the algorithms underlying public-key cryptography, written from scratch in
Java against a test suite. University coursework, 2023.

| Class | Algorithm |
|---|---|
| `EulerMobius` | Euler's totient and Mobius functions, least common multiple of a set |
| `ChineseRemainderTheorem` | systems of linear congruences |
| `LegendreJacobi` | Legendre and Jacobi symbols |
| `MillerRabin` | probabilistic primality testing |
| `PollardsRhoAlgorithm` | integer factorisation |
| `Cipolla` | square roots modulo a prime |
| `BigStepSmallStep` | baby-step giant-step, discrete logarithm |
| `EllipticCurve` | arithmetic over elliptic curves |
| `RSA` | key generation, encryption, decryption |

Together these are what a public-key scheme is built from: primality testing to find the
primes, factorisation and discrete logarithm as the problems whose hardness the schemes rest
on, Jacobi symbols and modular square roots as the primitives, and RSA as one construction
that uses them.

## Running

```bash
mvn test
mvn exec:java -Dexec.mainClass=com.konstde00.App
```

The original problem statements are in Ukrainian in `Readme.md`.
