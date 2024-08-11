This project shows how to use the TFHE-rs library in Rust to provide efficient arithmetic and comparison operations. The code demonstrates the use of fully homomorphic encryption (FHE) to encrypt, manipulate, and decrypt FheUint8 and FheBool data.

## Features
- **Key Generation:** Generate client and server keys using the TFHE library's ConfigBuilder.
- **Encryption & Decryption:** Encrypt and decrypt unsigned 8-bit integers (u8) and boolean values using FheUint8 and FheBool.
- **Optimized Operations:** Perform optimized arithmetic (addition, subtraction, multiplication, division, remainder) and logical operations (AND, OR, XOR, NOT, shifts) on encrypted data.
- **Comparison Operations:** Evaluate equality, inequality, greater than, and less than comparisons on encrypted data.


## Requirements
- **Rust:** Ensure you have the latest stable version of Rust installed. 
- **TFHE Library:** The project depends on the TFHE library for fully homomorphic encryption. Ensure the library is included in your `Cargo.toml` file. 
## Main Steps
- **Configuration:**  A default configuration is set up using ConfigBuilder::default().build().
- **Key Generation:**  Keys are generated and the server key is set using generate_keys and set_server_key.
- **Encryption:**  Values are encrypted into FheUint8 using the client key.
- **Optimized Operations:**  The code defines various optimized functions to perform arithmetic and logical operations on the encrypted values.
- **Comparison Operations:**  The code also includes optimized functions to compare encrypted values.
- **Verification:**  After performing operations, the results are decrypted and verified against the expected results.

## Code Structure
- main.rs: Contains the core logic for configuring, encrypting, computing, and verifying results.
- optimized_operations.rs: Implements optimized arithmetic and comparison operations on encrypted values.

## Optimized Functions
- optimized_add, optimized_sub, optimized_mul, optimized_div, optimized_rem: Perform arithmetic operations on encrypted data.
- optimized_shl, optimized_shr: Perform bitwise shifts on encrypted data.
- optimized_eq, optimized_ne, optimized_gt, optimized_lt: Perform comparison operations on encrypted data.

git clone https://github.com/cypriansakwa/Implementing_and_Verifying_Optimized_FHE_Operations_in_Rust.git
cd Implementing_and_Verifying_Optimized_FHE_Operations_in_Rust
