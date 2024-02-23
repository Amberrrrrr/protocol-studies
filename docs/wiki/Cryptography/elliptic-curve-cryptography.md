# A Brief Introduction to Elliptic Curve Cryptography

Cryptography can often seem like an abstract and theoretical field, but its applications are deeply woven into the fabric of our everyday lives. Let's consider a real-world scenario to understand how cryptography, specifically Elliptic Curve Cryptography (ECC), can be used to safeguard critical interactions.

Alice, a diligent businesswoman, has been abducted and held captive on a remote island. Her captors demand a hefty ransom of $1 million for her release. With limited options for communication, they provide a single postcard for her to instruct her associate, Bob, to transfer the funds.

Alice considers writing the ransom amount and signing the postcard like a check. However, this method poses a significant risk: the kidnappers could easily forge the postcard, inflate the amount, and deceive Bob into sending them more money.

Alice needs a robust approach that allows:

1. Bob to verify that the transfer has be authorized by her, and
2. ensure that postcard's message has not been tampered with.

The goal of this exercise is device a method for Alice to create a **secret key 🔑** known only to her. This key will be crucial for her to prove her identity and ensure the message's authenticity to Bob.

Mathematics, as always, comes to the rescue. Through ingenious use of **Elliptic Curves**, let's explore how Alice can generate the secret key.

# Elliptic curves

An elliptic curve is a curve **described by the equation**:

$$
y^2 = x^3 + ax+b
$$

Examples:

<img src="images/elliptic-curves/examples.gif" width="500"/>

Ethereum uses a standard curve known as [secp256k1](http://www.secg.org/sec2-v2.pdf) with parameters $a=0$, and $b=7$; which is the curve:
$$y^2=x^3+7$$

<iframe src="https://www.desmos.com/calculator/4yfo6djcyb?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

Observe that elliptic curves are symmetric about the x-axis.

# Further reading

**Elliptic curve cryptography**

- 📝 Standards for Efficient Cryptography Group (SECG), ["SEC 1: Elliptic Curve Cryptography."](http://www.secg.org/sec2-v2.pdf)
- 🎥 Fullstack Academy, ["Understanding ECC through the Diffie-Hellman Key Exchange."](https://www.youtube.com/watch?v=gAtBM06xwaw)
- 📝 Andrea Corbellini, ["Elliptic Curve Cryptography: a gentle introduction."](https://andrea.corbellini.name/2015/05/17/elliptic-curve-cryptography-a-gentle-introduction/)

**Mathematics of Elliptic Curves**

- 📘 Joseph H. Silverman, ["The Arithmetic of Elliptic Curves."](https://books.google.co.in/books?id=6y_SmPc9fh4C&redir_esc=y)
- 📝 Rareskills.io, ["Elliptic Curve Point Addition."](https://www.rareskills.io/post/elliptic-curve-addition)

**Useful tools**

- 🎥 Tommy Occhipinti, ["Elliptic curves in Sage."](https://www.youtube.com/watch?v=-fRWR_QKzuI)
- 🎥 Desmos, ["Introduction to the Desmos Graphing Calculator."](https://www.youtube.com/watch?v=RKbZ3RoA-x4)

# Credits

- Thanks to Michael Driscoll for his work on [animated elliptic curves.](https://github.com/syncsynchalt/animated-curves)
