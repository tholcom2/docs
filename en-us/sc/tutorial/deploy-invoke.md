# Deploying a Smart Contract with Parameters

## 1 - Introduction
 What this tutorial will cover
 
## 2 - Useful Resources

* [Lock2](https://github.com/CityOfZion/docs/blob/develop/en-us/sc/tutorial/Lock2.md)
* [Parameter](https://github.com/CityOfZion/docs/blob/develop/en-us/sc/tutorial/Parameter.md)
   
## 3 - SC Code
 
## 4 - Deploying a Smart Contract with Parameters
 
1. To deploy the smart contract (.avm) on the blockchain, click on the **Advanced** menu option on the NEO desktop wallet and select **Deploy Contract**.
2. Populate all of the fields in the **Information** section of the window that appears.  All fields must be populated to deploy the contract.
3. Load the .avm file using the **Load** buttton.  The Code field will be populated with the script hash.  Copy the contents of the **Code** field for use in a later step.
4. Populate the **Metadata** fields referencing the **Parameter** documentation.
  ```Example:
    A smart contract defined as:
    public static bool Main( (byte[]) publicKey, (byte[]) Sig, int value ){}
 
    Has a Parameter list: 020001
    and Return Type: 01	
  ```
  
5. If the contract requires storage (uses the Storage methods), check the **Need Storage** box.
6. Click the **Deploy** button.


## 5 - Watching the Smart Contract   
 
1. On the main NEO wallet window, right click on the address area and select (Create Contract Add > Custom)
2. Select the Account that you want to associate the Contract with from the 'Related Account' dropdown
3. In the 'Parameter List' field, populate the 'Parameter List' values used in Step 4 of the **Deploy Smart Contract w/ Parameters** sections.
4. Populate the 'Script' field with the value provided in Step 3 of **Deploy Smart Contract w/ Parameters**.
5. Click 'Confirm' to load the contract into the wallet window.
 
  
 
## 6 - Invoking the Smart Contract
 
To invoke a smart contract on the NEO blockchain, you will need the smart contract script hash. 
1. To acquire the contract hash, right click on the contract account populated in the address window as a result of the **Watching the Smart Contract** window.
2. Select 'View Contract' to open a window containing information about the smart contract.  Copy the value in the 'Script Hash' field.
3. Click on the 'Advanced' menu option and select 'Invoke Contract'.
4. Populate the 'Script Hash' field with the value copied in Step 2.
5. The Smart Contract information should automatically populate in the remaining 'Invoke Function' fields.
6. To populate the input parameters, click on the '...' button next the the Parameters field to open the parameter population menu.
7. Select the parameters on the left field and populate the variable values in the lower right field.
8. Click 'OK' to close the parameter input window.
9. Click the 'Invoke' button to invoke the smart contract.
 
 
