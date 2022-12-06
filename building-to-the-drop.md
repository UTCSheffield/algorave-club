---
title: Building to the drop
tags: presentation
slideOptions:
  theme: white
  #transition: 'fade'
  #parallaxBackgroundImage: 'https://s3.amazonaws.com/hakim-static/reveal-js/reveal-parallax-1.jpg'
live: https://hackmd.io/@IvSYepi5QUqOXsQx5s409A/r18HG3ELs#/
---

# Building to the Drop 
## How we learnt to Algorave by hacking on FoxDot

---

## Intro : Who we are?

- UTC Sheffield Olympic Legacy Park
- Mr Eggleton / stretch___beatz @M
- People who like silly numbers, wait, thats just me (@J). nevermind moving on

![image alt](https://utcsheffield.github.io/algorave-club/img/utc-algorave-club-logo.jpg "title" =200x200)


Note: 
  - specialist school for 13-18 year olds
  - Algorave Club members are live coding the soundtrack to this talk as we go


---


## The Start

- @M & UTC Sheffield loosely involved in Alograve / FoxDot for years
- Students (@J + a cameo from @A) ask for a Electronic Music Club
- Tiny after-school group starts with FoxDot

---

## Summer

- Live music
- @M writes first version of soloBars()

```python
d1.soloBars()
```

Note:
- @M sees C.C.A.I. live and Sam does this classic thing of soloing the drums for a few bars before bringing it all back in
- Started playing with foxdot



---

## Algorave Club - Sept 2022

- we start playing with FoxDot
- we tried demoing strudel
- @F suggests soloBars(end=True)

```python
d1.soloBars(end=True)
```

---

# @F Being Clever 

- @F defines his method for drop
- Speeds up a drum in a specified number of bars (the buildup), (from dur = Clock.bar_length() to a target dur) 
- then solos it for another specified number of bars, then optionally ends the player while it un-solos. 

---

```python!
b1.drop(buildup=2, target=1, solo=2, end=False)
```



---

```python!
s1 >> space(P[1,2,2,4,5].palindrome(), dur=PDur(5,8))
d9 >> play("X", sample=2).drop(target=0.25, player=s1)

```

---

## What we've learnt
@F is clever.
Algorythms are hard.
The pattern for drop is like 40 lines long.

## The code

[Our FoxDot](https://github.com/UTCSheffield/FoxDot)

