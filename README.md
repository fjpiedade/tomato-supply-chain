# Project Blockchain 24

### Use Case 3: Tomato Traceability with Blockchain: Transparency from Seed to Shelf

### Description

Implementation of a Traceability system for the entire process from tomato production and consumption using DAML.

### Contract

- **TomatoBatch** -> _all Parties and All information about the tomato batch._

  <!-- ![Screenshot 2024-05-08 at 1 35 07 PM](https://github.com/fjpiedade/tomato-supply-chain/assets/82730685/edf2dff1-7ea6-45a0-bdf3-10f1344e81ab) -->

```daml
type TomatoBatchCID = ContractId TomatoBatch -- Asset
-- Definition of the contract to represent a batch of tomatoes
template TomatoBatch
  with
    batchId: Text
    farmer: Party
    distributor: Optional Party
    retailer: Optional Party
    consumer: Optional Party
    variety: Text
    quantity: Int
    weight: Decimal
    plantingDate: Date
    harvestDate: Date
    harvestLocation: Text
    currentLocation: Text
    certification: Text
    temperature: Decimal
    humidity: Decimal
    hasFertilizer: Bool
    price: Decimal
    status: Text
```

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
