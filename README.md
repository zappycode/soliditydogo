Woof!

![woof](https://i.stack.imgur.com/DskhO.png)

```
pragma solidity ^0.5.1;

contract Dogo {
  bytes32[16] public woofs;

  function woof(bytes32 bark, uint spotNumber) public returns (uint) {
    require(spotNumber >= 0 && spotNumber <= 15);

    woofs[spotNumber] = bark;

    return spotNumber;
  }
}
```
