# PasswordChecker.sol
Hard to disagree with this.
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract PasswordChecker {
    string private password = "1234";

    function checkPassword(string memory _pass) public view returns (bool) {
        return keccak256(abi.encodePacked(_pass)) == keccak256(abi.encodePacked(password));
    }
}
Add basic contract structure
