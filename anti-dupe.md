
## Anti-Duplication

### How can we ensure that each card is received once and only once?

We can include the time of when each card was sent, followed by a number of minutes in which the card should be destroyed (14:53, 1). Each card in a single message should include the same number of minutes to live. So, at 14:54, if a node still had the card, then it should be destroyed. 

Once Bob sends a message back to Alice about a missing card, Bob should include the card number (card 4/9) as well as the times in which the card before and the card after were sent and the number of minutes to live. By including the times, this allows Alice to see if the card has gone past its time to live, and send another to Bob. 
