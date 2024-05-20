# Project Blockchain 24

### Use Case 3: Tomato Traceability with Blockchain: Transparency from Seed to Shelf

### Description

Implementation of a Traceability system for the entire process from tomato production and consumption using DAML.

### Contract

- **TomatoBatch** -> _All information about the tomato batch and all Parties._

![Screenshot 2024-05-20 at 7 56 36 AM](https://github.com/fjpiedade/tomato-supply-chain/assets/82730685/4b0435b2-8b3e-4539-94bb-d93d87565ac8)


### Choices

- **Harvested** -> _When harvested by the producer, initial state;_

- **Packed** -> _Phase that represents being prepared for collection at the distributor;_

- **ReceivedByDistributor** -> _Distributor Reception;_

- **InTransit** -> _When lots are in transit through the distributor, the location and environmental situation, such as temperature and humidity, can be updated;_

- **InTransitToRetailer** -> _When lots are in transit to the store;_

- **ReceivedByRetailer** -> _Reception by the store;_

- **ReadyToSell** -> _Ready to be sold;_

- **PurchasedByConsumer** -> _Purchase process by the consumer;_

- **ReturnedToFarmer** -> _Process that allows the distributor to send a batch of tomatoes back to the Farm;_

- **DeniedByRetailer** -> _Process that allows a retailer or store to reject a batch of tomatoes._

### How to Run

Execute setup script

![Screenshot 2024-05-09 at 1 20 12 AM](https://github.com/fjpiedade/tomato-supply-chain/assets/82730685/d4412494-fe1f-4716-b5c8-139394622d13)


### Result

![Screenshot 2024-05-07 at 11 54 43 PM](https://github.com/fjpiedade/tomato-supply-chain/assets/82730685/6a0cf327-1d44-4ef4-be52-3fbb7485562b)
