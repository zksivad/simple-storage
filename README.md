# Simple Storage Contract 

A Solidity smart contract that demonstrates state variable storage along with structs, dynamic arrays, and mappings.

This contract allows users to:
- Store a favorite number
- Retrieve the stored value
- Add people with names and favorite numbers
- Map names to their favorite numbers

---

##  Features

### 1. Store & Retrieve a Number
- `store(uint256 _favoriteNumber)` — updates the stored number  
- `retrieve()` — returns the current stored number  

### 2. Struct-Based Storage
The contract includes a Person struct:
struct Person {
uint256 favoriteNumber;
string name;
}

An array of these structs is stored in:
Person[] public listOfPeople;

### 3. Mapping Support
Maps a person's name to their favorite number:
mapping(string => uint256) public nameToFavoriteNumber;


### 4. Add People
Adds a new person to the array and mapping:
addPerson(string memory _name, uint256 _favoriteNumber)



---

##  Tools Used
- Solidity 0.8.19
- Remix IDE
- GitHub for version control

---

##  Key Concepts Demonstrated
- State variables  
- Structs  
- Dynamic arrays  
- Mappings  
- Public getters  
- Basic storage & retrieval  

---

##  Future Improvements
- Add an event when a person is added  
- Emit an event when the favorite number changes  
- Prevent duplicate name inserts  
- Add access control (owner-only functions)  

---
