Two's complement is a binary representation scheme used to represent signed integers in computers. It's the most common method for representing signed integers because it simplifies arithmetic operations and allows addition and subtraction to be performed using the same circuitry as for unsigned integers. Here's how the two's complement representation works:

1. **Positive Numbers**:
   - Positive integers are represented in binary as usual, with the most significant bit (MSB) as 0.
   - For example, decimal 7 is represented as `0111` in four bits.

2. **Negative Numbers**:
   - To represent negative numbers, two's complement is used. The process involves inverting all the bits (changing 0s to 1s and vice versa) and then adding 1 to the result.
   - For example, to represent decimal -7:
     1. Invert the bits of `0111` to get `1000`.
     2. Add 1 to `1000` to get `1001`.
     - So, -7 is represented as `1001` in four bits using two's complement.

3. **Zero**:
   - Zero is represented with all bits set to 0, which is the same as its positive counterpart.

4. **Range of Representable Values**:
   - An n-bit two's complement representation can represent integers in the range from -2^(n-1) to 2^(n-1) - 1.

Here's an example of two's complement representation using 8 bits:

| Decimal | Binary (8-bit) | Two's Complement |
|---------|---------------|------------------|
| 7       | 00000111      | 00000111         |
| -7      | -             | 11111001         |

Keep in mind that performing arithmetic operations in two's complement representation simplifies the logic for the computer's hardware. Addition and subtraction can be performed using the same logic circuitry as for unsigned integers, which makes the design more efficient.

When working with programming languages like C and C++, the underlying hardware usually handles the two's complement representation transparently. You typically work with signed integers (`int`, `short`, `long`, etc.) and the language and compiler handle the conversion between binary and two's complement for you.