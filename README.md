# BURP

**B**eautiful **U**nique **R**eliable **P**asswords

**BURP** is a reliable password generator. You feed **BURP** a key and your unique passphrase and it will belch back a password that can be reliably regenerated again later so you never have to remember it.

**BURP** is meant to replace the passwords you use for trivial internet accounts. Instead of constantly forgetting your password to the point of writing it down, using a simple and insecure password, or worse [the same insecure password for multiple sites](http://gizmodo.com/5812545/find-out-if-your-passwords-were-leaked-by-lulzsec-right-here). Instead you create a password with **BURP**  that you can regenerate later, the idea is that you don't have to remember your password and there's nothing to lose.

**BURP** is not inherently secure and comes with no warranty, I definitely would not recommend you use it to generate your bank password.

## Usage

**Key** - A unique identifier, the reason for generating the password.

**Passphrase** - Your **BURP**'s secret sauce. This should be a long but memorable sequence of words, numbers and punctuation- the longer the better. Pick something that's both memorable and easy to type accurately and don't use well known phrases, famous quotes, or literature.

$ ./BURP.rb  
Enter your unique key: reddit.com  
Enter your passphrase: (not echoed to terminal)  
Your password is: tower-wigwam-baby-salad

## To Do

* Password restrictions (alphanumeric, uppercase, special characters, maxlength, etc)
* Encrypted custom wordlist

## Security

The default wordlist is 256 words resulting in just over 4 billion (256^4) possible permutations with the default settings (4 words). For added security roll your own custom wordlist with at least 256 words. 

## Notes

Much of the inspiration for **BURP** comes from the [XKCD](http://xkcd.com/936/) password comic and [humanhash](https://github.com/zacharyvoase/humanhash). My friends Tim Burden and Todd Graham helped me come up with the name and brainstorm ways to make passwords more secure, such as possibly encrypting the wordlist.

## Disclaimer

**BURP** comes with no warranty. 

