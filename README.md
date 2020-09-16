


# Smart contracts using solidity
<p align="center">
<img src="./images/smartcontract.jpeg?raw=true" alt="Smart contract"/>
</p>

We used solidity to create three smart contracts as needed by the business users. Solidity code for these smart contracts can be found under folder "code".

1. [AssociateProfitSplitter.sol](code/TieredProfitSplitter.sol) - This contract accepts Ether into the contract and divide the Ether evenly among the associate level employees. This will allow the Human Resources department to pay employees quickly and efficiently.
2. [TieredProfitSplitter.sol](code/TieredProfitSplitter.sol) - This contract distributes different percentages of incoming Ether to employees at different tiers/levels. For example, the CEO gets paid 60%, CTO 25%, and Bob gets 15%.
3. [DeferredEquityPlan.sol](code/DeferredEquityPlan.sol) - This contract models traditional company stock plans. This contract will automatically manage 1000 shares with an annual distribution of 250 over 4 years for a single employee.

<br>
<br>

First we created the solidity code in **Remix** editor. While developing and testing the contracts, we used the **Ganache** development chain, and pointed **MetaMask** to **localhost:8545**
<br>
<br>

## <ins>**Deploying and testing the contracts on the localhost:**</ins>
### **_The AssociateProfitSplitter Contract:_**
After deploying the contract locally, we performed a transaction to confirm that the balance is distributed to all three addresses as expected. Below screenshot confirms the balances after the transaction. The original balance was 100 each and 3.33 eth were added to each address when distribution took place.

<p align="center">
<img src="./images/AssociateProfitSplitter_1.png?raw=true" alt="Smart contract"/>
</p>
<br>

### **_The TieredProfitSplitter Contract:_**
This contract should be distributing different percentages of incoming Ether to employees at different tiers/levels. So we performed a transaction to confirm that the balance is distributed to all three addresses according to the requirements. Below screenshot confirms the balances after the transaction. The original balance shown above was incremented according to the percentage allocation for each employee (address).

<p align="center">
<img src="./images/TieredProfitSplitter _1.png?raw=true" alt="Smart contract"/>
</p>
<br>


### **_The DeferredEquityPlan  Contract:_**
This contract should be  managing an employee's "deferred equity incentive plan" in which 1000 shares will be distributed over 4 years to the employee. After deploying the contract, we performed trasactions using the distribute function and checkd the balance. Below screenshot shows the balance after distribution.

<p align="center">
<img src="./images/DeferredEquityPlan_1.png?raw=true" alt="Smart contract"/>
</p>
<br>
<br>

## <ins>**Deploying and testing the contracts on the Kovan Test Network:**</ins> 
After testing the contracts locally and makign sure they work as expected, we deployed the contracts to Kovan Test Network.  
<p align="center">
<img src="./images/Kovan_account.png?raw=true" alt="Smart contract"/>
</p>
<br>

### **_The TieredProfitSplitter Contract_**
Transaction confirmation and balance of one address after the transaction:
<p align="center">
<img src="./images/AssociateProfitSplitter_2.png?raw=true" alt="Smart contract"/>
</p>
<br>

<p align="center">
<img src="./images/AssociateProfitSplitter_3.png?raw=true" alt="Smart contract"/>
</p>
<br>

### **_The TieredProfitSplitter Contract_**
Transaction confirmation and balance of one address after the transaction:
<p align="center">
<img src="./images/TieredProfitSplitter_3.png?raw=true" alt="Smart contract"/>
</p>
<br>

<p align="center">
<img src="./images/TieredProfitSplitter_2.png?raw=true" alt="Smart contract"/>
</p>
<br>

### **_The DeferredEquityPlan Contract_**
Transaction confirmation and balance of one address after the transaction:
<p align="center">
<img src="./images/DeferredEquityPlan _distribute.png?raw=true" alt="Smart contract"/>
</p>
<br>

<p align="center">
<img src="./images/DeferredEquityPlan_1.png?raw=true" alt="Smart contract"/>
</p>
<br>

 