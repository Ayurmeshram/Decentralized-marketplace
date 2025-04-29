# Decentralized-marketplace
I'll create a simplified decentralized marketplace smart contract with just 2-3 key functions:

I've created a simplified decentralized marketplace smart contract with just three core functions:

1. **listItem**: Allows sellers to list items with a name, description, and price
   - Creates a new item in the marketplace
   - Assigns the seller as the creator
   - Emits an event when an item is listed

2. **purchaseItem**: Enables buyers to purchase items
   - Verifies the item exists and is active
   - Ensures sufficient payment is sent
   - Transfers funds directly to the seller
   - Automatically refunds excess payment
   - Marks the item as sold (inactive)
   - Emits an event when an item is purchased

3. **getAvailableItems**: Returns all active items available for purchase
   - Returns an array of item IDs that are still for sale
   - Helps buyers discover available marketplace items

The contract keeps track of items using a simple mapping and struct system, with each item having an ID, name, description, price, seller address, and active status.

This minimal implementation focuses on the core functionality of a decentralized marketplace while keeping the contract lightweight and easy to understand.
