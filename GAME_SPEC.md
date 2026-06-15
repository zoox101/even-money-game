# Game Specification

The original design spec for Even Money — an HTML-based game used to teach people about investing. It works as follows:

## Setup

1. The program choses a random number `X` from 2-6 (this number is hidden from the user)
2. Depending on the number chosen, the program creates a random deck of cards from 2-10 with `X` copies of each card in the deck
3. Anytime a deck is exhausted, the program regenerates a new deck using the same approach picking a new random number `X`
4. The user starts out with $100 - their goal is to make $1,000,000

## Gameplay

1. The user first selects 1 of four options: (1) Go Long; (2) Go Short; (3) Lever Up; (4) Hold

**Go Long**: If the number is even, double the user's money. If it is odd, half it
**Go Short**: If the number is odd, double the user's money. If it is even, half it
**Lever Up**: If the number is even, quadruple the user's money. If it is odd, set it to zero
**Hold**: Do not change the user's money

2. After the user selects an option, a card is drawn, shown to the user, and their total money amount is modifed depending on the strategy they chose

3. Three months are added to the timer

## Ending the Game

- If the user runs out of money, they instantly lose. Show them how long they survived for
- If the user reaches or surpasses $1,000,000 they instantly win. Show them how many years it took them to turn $100 -> $1,000,000

## Notes

- The user should have the ability to repeat an option some number of times. When that happens, the game should rapid deal that number of cards with the result appearing and the timer incrementing after each card
- The game should show a graph showing the user's "net worth" over time
- The entire game should fit on a standard laptop screen without scroll-bars
- The game should be statically hostable on any static hosting platform like GitLab pages or Google cloud bucket
