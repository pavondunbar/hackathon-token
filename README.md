How to Use This Contract

NOTE: This is a crypto-backed stablecoin that has a built in KYC mechanism. This was submitted to Chainlink's Hackathon back in 2023.

CONTRACT OWNER:

1. Deploy this contract to the blockchain of your choice.

2. Call the addKYC() function in the contract to input the user's information to approve the user to get ART Tokens. Pass as parameters:
                    User's wallet address,
                    An ID number to identify the user,
                    User's Full name,
                    User's Residential Address,
                    User's City,
                    User's State,
                    User's Zip,
                    User's Date of Birth (can be in any format ex: mm-dd-yyyy or mm/dd/yyyy or March 16, 1978),
                    User's Driver License or ID number,
                    User's License or ID State of Issuance

3. Run the kycMapping() function to confirm that the user has been added to the smart contract

CONTRACT USER:

1. Once you receive notification that your KYC has been approved, you need to call the approve() function on the USDC contract address to authorize this smart contract to process your USDC tokens.
2. Once you've approved the contract to use the USDC tokens, execute the buy() function and specify how many ART tokens you would like to purchase. ART tokens are set at 6 decimal places to match USDC, so remember to set the appropriate number of zeros. For example, if you want to buy 500 ART tokens, you need to specify 500 as 500000000 (500 with 6 zeroes).
3. Remember, 1 USDC = 1 ART. There is no charge to buy ART tokens.
4. You can sell your ART tokens back to the smart contract at any time to get back USDC tokens. However, there is a fee to sell ART TOKENS back. This fee is in addition to any gas fees charged to you by the blockchain network.

If you have any questions or issues about this contract, feel free to submit an ISSUE here and I will respond as soon as possible.  Thank you.
