# blockchain-and-cryptocurrency
Build a Blockchain and a Cryptocurrency from Scratch using javascript and its libraries.
you will know how blockchains work at the core, and how cryptocurrencies like Bitcoin are implemented.

clone the repo, install all dependency ,start testing

POSTMAN TEST

First run one node

$ HTTP_PORT=3001 P2P_PORT=5001 npm run dev

Run a second node

$ HTTP_PORT=3002 P2P_PORT=5002 PEERS=ws://localhost:5001 npm run dev

$ curl http://localhost:3002/public-key

grab value from ^^

hit_transactions = ?

$ hit_transactions * curl -d '{"address":"0429d6c26410c83f725609426ed63b0b6f8cdfe2a7414deab02bfefa53fa2b30d458bd6901fee6272ff373f1adec6f4f28e57b25c0f1487d39890ab073f80bf5e8", "amount":"50"}' -H "Content-Type: application/json" -X POST http://localhost:3001/transact

$ curl http://localhost:3001/transactions

$ curl http://localhost:3002/transactions

$ curl http://localhost:3001/mine-transactions

$ curl http://localhost:3001/balance

// expect a balance to equal 500 - (hit_transactions * 50) + 50 // for the reward

$ curl http://localhost:3002/blocks

$ curl http://localhost:3001/transactions

$ curl http://localhost:3002/transactions

*/



TODO:

* test the transaction pool
