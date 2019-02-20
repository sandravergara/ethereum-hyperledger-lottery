# Ethereum-Hyperledger-Lottery

This repository contains Ethereum and Hyperledger design in process diagram. 

# Contents

**Ethereum Lottery**

Simple Lottery

Recurring Lottery

RNG Lottery

Powerball

**Hyperledger Lottery**

Simple Lottery

Recurring Lottery

RNG Lottery

Powerball

# Steps

1. Clone this repository git clone https://github.com/ssvergara/ethereum-hyperledger-lottery.git
2. Go to this link https://www.draw.io/ 
3. Drag the XML file to draw.io to view the process diagram.

# ReadMe Ethereum Lottery

**Simple Lottery Ethereum**

1. The user will initiate the contract.
2. The System will Set lottery duration and save to world state the total duration.
3. The user will load contract address.
4. The user will buy ticket.
5. When user successfully bought a ticket, System add user's addresss to ticket list in world state.
6. When duration will lapsed,
7. User will draw the winner if he/she will be the winner.
8. When user draw the winner, the system will generate random unsigned integer.
9. After that, system will Use the generated integer to select an adress to Ticket list in world state.
10. After that, system will Assign winner's address that will retrieved in world state.
11. When the address verified successfully, the user will withdraw the prize.
12. When withdrawing the prize the system will transfer balance to winner's address.
END

**Recurring Lottery Ethereum**

1. The user will initiate the contract
2. System will provide new round
3. The System will Set lottery duration and save to world state the total duration
4. The user will load contract address
5. The user will buy ticket
6. The System will end the time or duration lapsed
7. User will draw the winner
8. When user draw the winner, the system will generate random unsigned integer
9. After that, system will Use the generated integer to select an adress to Ticket list in world state
10. After that, system will Assign winner's address that will retrieved in world state
11. When the address verified successfully, the user will withdraw the prize.
12. When withdrawing the prize the system will transfer balance to winner's address
13. Add 1 to round counts
14. The system will initiate new rounds
15. If the round counts is less than or equal to 100, the system will be deleted 1 round

**RNG Lottery Ethereum**

1. Every buyer submits a commitment hash when they buy a ticket.
2. User’s is generating their number which they want to submit.
3. User’s secret number and address will be added to ticket list.
4. Ticketing period is over. Tickets cannot be purchased after this period.
5. User’s must reveal their own secret number.  All reveals must occur after the ticket deadline and before the reveal deadline.
6. Verifying of commitment hash and must match the commitment submitted with the ticket.
7. If failed to submit their own number and address, dropped from the lottery.
8. Draw winner and Withdraw are nearly identical to SimpleLottery.
9. Draw winner 
10. Generate random number, it will enable to select the user’s address to ticketlist.
11.Generate random seed for picking a winner, this is random seed to determine the winner. Each time a secret number is revealed, the seed is modified to incorporate the reveal.
12. Withdraw 	
13. Balance will be added to user’s address and will added to world state to verify the address of the user.

**Powerball Ethereum**

______________________________________________________________________________________________________

# ReadMe Hyperledger Lottery

**Simple Lottery Hyperledger**



**Recurring Lottery Hyperledger**




**RNG Lottery Hyperledger**

1. User’s must register first and run the application.
2. Every buyer submits a commitment hash when they buy a ticket.
3. User’s is generating their number which they want to submit.
4. User’s secret number and address will be added to ID list..
5. Ticketing period is over. Tickets cannot be purchased after this period.
6. User’s must reveal their own secret number.  All reveals must occur after the ticket deadline and before the reveal deadline.
7. Verifying of commitment hash and must match the commitment submitted with the ID.
8. If failed to submit their own number and address, dropped from the lottery.

**Draw winner** and **Withdraw** are nearly identical to Simple Lottery.

10. Draw winner 
11. Generate new hash from block hash, it will enable to select the user’s address to ID list.
12. Generate random seed for picking a winner, this is random seed to determine the winner. Each time a secret number is revealed, the seed is modified to incorporate the reveal.
13. Withdraw 	
14. Balance will be added to user’s ID and will added to world state to verify the address of the user.
15. User’s wallet will be updated.

**Powerball Hyperledger**


