Google 2021 CTF BeginnerQuest

Website: https://capturetheflag.withgoogle.com/beginners-quest

*(Warning: this contains spoilers for an active CTF (obviously), so if you haven't done these challenges and want to then you should go ahead and go to the CTF site instead)*

# Flags & Solutions

## Chal 1

Flag: `CTF{IJustHopeThisIsNotOnShodan}`

Solution:
- View source of webpage
- Convert the hex integer `0xCafe` to denary
- Sort the `p[i]` into order
- Subtract `0xCafe` from each `p[i]`
- Convert to text
- Enter password `GoodPassword`
- Flag is at the bottom of the page

## Chal 2

Flag: `CTF{BCFIJ}`

Solution:
- Decode the logic gates to find combination of inputs is necessary to make the output a 1
- Flag is a string of the inputs that need to be 1

## Chal 3

Flag: `CTF{cbe138a2cd7bd97ab726ebd67e3b7126707f3e7f}`

Solution:
- Solve the problem in javascript
  - Solution by catdotjs#1110: https://pastebin.com/7UhCPQJH
- Flag is given after submitting your code solution

## Chal 4

Flag: *Unsolved*

Theories:
- Requires RaspberryPi to solve
- Involves pins

## Chal 5

Flag: `CTF{n3v3r_3ver_ev3r_use_r4nd0m}`

Solution:
- Python's `random` module uses Marsenne Twister algorithm
- Marsenne Twister repeats after exactly 624 iterations, which is the length of the random phone numbers text file
- Reverse engineer the encoding and encryption software
- Extract original 624 random numbers from robo call numbers
- Use numbers in Marsenne Twister predictor to decode secret.enc
  - Solution by mental#5985: https://pastebin.com/2UUUpkxa

## Chal 6

*Not visible yet*

## Chal 7

Flag: *Unsolved*

Theories:
- Uses python
- There's a `__pycache__` folder in the zip, doesn't include the flag or anything else interesting except the filepath: `/usr/local/google/home/jbuff/Documents/KCTF/2021-challenges-quals/beginners/crypto-babyrsa/attachments/chall.py`

## Chal 8

Flag: *Unsolved*
Theories:
- Involves PNG
