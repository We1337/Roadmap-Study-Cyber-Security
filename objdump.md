`objdump` is a powerful command-line utility that comes with the GNU Binutils suite. It is used for displaying information about object files, executable files, and shared libraries. `objdump` can provide a wide range of details about the binary file, including disassembled machine code, header information, symbol tables, and more.

Here are some common uses of `objdump`:

1. **Disassemble Executable:**
   ```bash
   objdump -d <executable>
   ```
   This command disassembles the machine code of the specified executable file, showing the assembly instructions.

2. **Display Sections:**
   ```bash
   objdump -h <executable>
   ```
   This command displays information about the sections in the specified executable, including their sizes, offsets, and attributes.

3. **Print Symbol Table:**
   ```bash
   objdump -t <executable>
   ```
   This command prints the symbol table of the executable, showing the addresses and names of symbols.

4. **Display Dynamic Sections:**
   ```bash
   objdump -x <executable>
   ```
   This command displays the dynamic sections of the executable, providing information about shared library dependencies and other runtime details.

5. **Print Relocation Entries:**
   ```bash
   objdump -r <executable>
   ```
   This command prints the relocation entries in the executable, showing how addresses are adjusted during linking.

6. **Display Header Information:**
   ```bash
   objdump -f <executable>
   ```
   This command displays the file header information, including the architecture, entry point, and other details.

7. **Disassemble a Specific Section:**
   ```bash
   objdump -d --section=.text <executable>
   ```
   This command disassembles a specific section of the executable, such as the ".text" section.

8. **Display Source Code alongside Assembly:**
   ```bash
   objdump -S <executable>
   ```
   This command displays the source code interleaved with the assembly code, if the executable contains debug information.

`objdump` is a versatile tool commonly used for reverse engineering, debugging, and analyzing binary files. It provides a wealth of information about the structure and content of executable files, making it a valuable resource for understanding the internals of compiled programs.