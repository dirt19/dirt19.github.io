---
layout: post
title:  "Vigenere Cipher"
date:   2023-09-10 21:53:00 -0600
categories: cryptography cipher vigenere
permalink: /cipher
excerpt: "Kryptos"
---
## Summary
Several years ago, I encountered the "KRYPTOS" sculpture and mysteries surrounding the messages. The Vigenere Cipher was intriguing.

## Some code
{% highlight python %}
def encipher(plaintext, key):
    ciphertext = ""
    key = key.upper()
    key_index = 0

    for char in plaintext:
        if char.isalpha():
            # Determine the shift value based on the current key character
            shift = ord(key[key_index % len(key)]) - ord('A')

            if char.isupper():
                new_char = chr((ord(char) - ord('A') + shift) % 26 + ord('A'))
            else:
                new_char = chr((ord(char) - ord('a') + shift) % 26 + ord('a'))

            ciphertext += new_char

            # Move to the next key character
            key_index += 1
        else:
            ciphertext += char

    return ciphertext


def decipher(ciphertext, key):
    plaintext = ""
    key = key.upper()
    key_index = 0

    for char in ciphertext:
        if char.isalpha():
            # Determine the shift value based on the current key character
            shift = ord(key[key_index % len(key)]) - ord('A')

            if char.isupper():
                new_char = chr((ord(char) - ord('A') - shift) % 26 + ord('A'))
            else:
                new_char = chr((ord(char) - ord('a') - shift) % 26 + ord('a'))

            plaintext += new_char

            # Move to the next key character
            key_index += 1
        else:
            plaintext += char

    return plaintext


# Example usage:
key = "How can I, unless someone show me?"
plaintext = """Temporary virtual credit cards have a number of uses for the consumer: Free trial signups, separation of concerns, and similar to fin-tokens - cut off without changing primary card."""

# Encipher the plaintext
ciphertext = encipher(plaintext, key)
print("Ciphertext:", ciphertext)

# Decipher the ciphertext
decrypted_text = decipher(ciphertext, key)
print("Decrypted Text:", decrypted_text)

{% endhighlight %}
