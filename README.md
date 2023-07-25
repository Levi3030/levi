CREATE A TOKEN
This SOLIDITY assessment aims to create an nft token in a simple and easy way in order for newbie students can understand with ease.
Description
It's important to note that this code is a minimal implementation and does not include crucial features such as access control, security checks. In a real-world scenario, you would need to consider additional functionality and best practices to ensure the contract's security and usability.

Getting Started
Installing
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.
Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., johnlevi.sol). Copy and paste the following code into the file:
Executing program
- First you need to create string variables.
- Use a function called mapping address and make it public.
- Create a mint function that both parameters has an address and uint.
- Create a burn function, it is nearly the same as the mint function but replace the "+" with a "-" and add a if statement.
- Deploy your NFT and try its features.

contract MyToken {

    // public variables here
    string public name = "REMIX";
    string public abbrv = "RNB";
    uint public supply = 0;

    // mapping variable here
         mapping(address => uint) public blnc;

    // mint function 
        function mint (address add, uint val) public{
           supply += val;
           blnc [add] += val;
        }

    // burn function
        function burn(address add, uint val) public{
           if(blnc[add] >= val){
              blnc[add] -= val;
           }
        }
}
Authors
Contributors names and contact info
Viñas John Levi M. 8202689@ntc.edu.ph
Johm Vinas
https://www.facebook.com/johnlevi30/

License
This project is licensed under the [John Levi M. Viñas] License - see the LICENSE.md file for details
