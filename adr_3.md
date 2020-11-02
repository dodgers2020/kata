# ADR #3

![Topology Diagram #1](./topology_v2.png)

In discussing which component is persisting transaction data, we identified that the Inventory Tracker should own that responsibility. As the architecture evolves, the transaction and inventory data will need to remain easily accessible to the Inventory Tracker. Furthermore, the Transaction Retriever does not need the data once it has processed it.

The Transaction Retriever may need to store information about the smart fridges and coffee shop kiosks in order to poll for the transaction data.
