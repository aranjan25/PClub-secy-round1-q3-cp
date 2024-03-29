# Gotta Catch 'em all
## Problem Statement
You are Ash, a young pokémon trainer. You have recently encountered upon a new location which offers a huge amount of exotic pokémons, and you do not want to miss this golden opportunity to catch them. You decide to take the help of Professor Oak, a well known pokémon researcher. Each of your and Prof. Oak's pokémon has its own power, which is a positive integer. You have **n** pokémons in your current team, where the **i***th* pokémon has power **A_i**.

Prof. Oak gives you **q** instructions. Each instruction is of 2 types, either an instruction to change, or to fight. If the instruction is to change, then Prof. Oak gives you 2 positive integers, **i** and **p**, and you replace your **i***th* pokémon by a new pokémon having power **p**.  If the instruction is to fight, Prof. Oak again gives you 2 positive integers **l** and **r**, and you have to fight with your team which consists of the **l***th* pokémon till the **r***th* pokémon (both inclusive). The raw power is given by the **GCD** of all the powers of pokémons in your team. In each fight, Prof. Oak then allows you to choose a legendary pokémon, and and you can choose a pokémon with any power between **1** and **m** (both inclusive). The total team power is then the **LCM** of the raw team power and the power of the legendary pokémon.

Since Ash is not good at maths, he needs your help to find the maximum team power he can achieve after adding the legendary pokémon.

## Input
The first line of input consists of 3 positive integers `n`, `m` and `q`, where **n** is the total number of pokémons Ash has, **m** is the maximum power of the legendary pokémon, and **q** is the number of instructions. The next line consists of **n** space separated positive integers **A_1, A_2, ... A_n**. Then each of the next **q** lines of inupt is either of the form `c i p` (change instruction) or `f l r` (fight instruction).

## Output
For each fight instruction, output the maximum team power Ash can achieve for that instruction in a new line.

## Constraints

**1** <= **l** <= **r** <= **n** <= **10^7**

**1** <= **q** <= **10^3**

**1** <= **m** <= **10^4**

**1** <= **i** << **n**

**1** <= **A_i, p** <= **10^9**

## Sample test cases

### Input

`5 10 3`

`1 2 4 8 16`

`f 3 4`

`c 3 8`

`f 3 4`

## Output

`36`

`72`

## Input

`1 59 1`

`40`

`f 1 1`

## Output

`2360`
