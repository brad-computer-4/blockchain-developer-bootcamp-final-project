# blockchain-developer-bootcamp-final-project

My idea is to publish relationships between accounts to the blockchain.  Let's say there is entity A, entity B, and entity C and the relationship between these entities (accounts) is in the public interest.  I want to find a way to publish information on the relationship between these accounts to the blockchain, and build an interface that can show balances, at the minimum.

I don't know enough about the space to know if this is something that is possible or needed.  I know about Etherscan and I know about The Graph.  With Etherscan, it seems like I can type in an address and view all of the transactions for any account.  Going back to my example, entity A might have also transacted with Z, Y, and X, but those transactions might be considered out of scope for our exercise.  I could probably put the in-scope information together through an Etherscan API call, or something, but I am wondering if I could provide an interface for no-code contract deployments.  This is all for the sake of learning, so I am not too worried about the use case making complete sense.  The benefit of publishing a contract is that the signer is acknowledging that the relationship between accounts exists, and they can publish it themselves to a decentralized ledger.

I am also thinking that what I want might be similar to publishing a contract to The Graph.  I will research that as well, and the potential benefits of integrating that, but here is what I am thinking for basic functionality:

1. User inputs accounts A, B, and C into form fields
2. Contract is created, which stores the in-scope accounts
3. User visits page, request is sent to the contract, which returns the balances of A, B, C --- derived only from their interactions within the scope of accounts A, B, and C.
