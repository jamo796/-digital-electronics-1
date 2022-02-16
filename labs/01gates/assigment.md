# Lab 1: YOUR_FIRSTNAME LASTNAME

### De Morgan's laws

1. Equations of all three versions of logic function f(c,b,a):

   ![Logic function](https://github.com/jamo796/-digital-electronics-1/blob/main/labs/01gates/img/demorgan.png)

2. Listing of VHDL architecture from design file (`design.vhd`) for all three functions. Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

```vhdl
architecture dataflow of gates is
begin
	-- necht je A = X , B = Y , C = Z
    f_org_o  <= (not(b_i) and a_i) or (not(c_i) and not(b_i));
    f_nand_o <= ( a_i nand ( b_i nand b_i ) )   nand ( ( b_i nand b_i ) nand (c_i nand c_i) );
	f_nor_o <= ((((a_i nor a_i) nor b_i) nor (b_i nor c_i))   nor  (((a_i nor a_i) nor b_i) nor (b_i nor c_i))); 
	f_firl_o <= (a_i and b_i) or (a_i and c_i);
    f_firr_o <= a_i and (b_i or c_i);
    f_secl_o <= (a_i or b_i) and (a_i or c_i);
    f_secr_o <= a_i or (b_i and c_i);

end architecture dataflow;
```

3. Complete table with logic functions' values:

| **c** | **b** |**a** | **f(c,b,a)_ORG** | **f(c,b,a)_NAND** | **f(c,b,a)_NOR** | **f(c,b,a)_FIRL** | **f(c,b,a)_FIRR** | **f(c,b,a)_SECR** | **f(c,b,a)_SECL** |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| 0 | 0 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1 |  
| 0 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 |
| 0 | 1 | 0 | 0 | 0 | 0 | 1 | 1 | 1 | 1 |
| 0 | 1 | 1 | 0 | 0 | 0 | 1 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 | 0 | 0 | 1 | 1 | 1 | 1 |
| 1 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 |
| 1 | 1 | 0 | 0 | 0 | 0 | 1 | 1 | 1 | 1 |
| 1 | 1 | 1 | 0 | 0 | 0 | 1 | 1 | 1 | 1 |

### Distributive laws

1. Screenshot with simulated time waveforms. Always display all inputs and outputs (display the inputs at the top of the image, the outputs below them) at the appropriate time scale!

   ![your figure](https://github.com/jamo796/-digital-electronics-1/blob/main/labs/01gates/img/prubehy2.png)

2. Link to your public EDA Playground example:

   [https://www.edaplayground.com/x/b3ew](https://www.edaplayground.com/x/b3ew)      
