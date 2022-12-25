# Equity-Crowdfunding
Crowdfunding Smart-Contract oversees that people who fund a company don't get cheated.
It starts with people sending their funds to smart contract instead to actual company manager's personal account .
Manager will set a deadline and target amount in order to enable the contract .

#sendEth():
    If a person wants to send fund to the contract than these condition must satisfy:
    1)block timestamp must be less than deadline.
    2)Should send minimum amount that has set by the manager.


#getContractBalance():
    This returns the total funded amount to the contract .
    This function can be called by any person who contributed the amount .

#refund():
    A Contributer gets refund only if these conditions satisfy:
     1)Block timestamp should be greater than deadline.
     2)Contract balance should be less than the target amount.

#createRequest():
    This function can be called by manager only.
    Manager can access the amount in contract only if more than half contributers permit him.
#makePayment():
    If majority of contributers support than the funds will be transferred to the managers account .
