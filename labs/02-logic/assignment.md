# Lab 2: YOUR_FIRSTNAME LASTNAMEE

### 2-bit comparator

1. Karnaugh maps for other two functions:
2. Equations of simplified SoP (Sum of the Products) form of the "greater than" function and simplified PoS (Product of the Sums) form of the "less than" function.

   ![](https://github.com/jamo796/-digital-electronics-1/blob/main/labs/02-logic/img/Kmaps.png)

### 4-bit comparator

1. Listing of VHDL stimulus process from testbench file (`testbench.vhd`) with at least one assert (use BCD codes of your student ID digits as input combinations). Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

   Last two digits of my student ID: **xxxx??**

```vhdl


    p_stimulus : process
    begin

-- SEQUENCE IMPUTS

        report "Stimulus process started" severity note;

-- ID = 211539
-- B = 3 = 0011
-- A = 9 = 1001


		s_b <= "0011"; s_a <= "1001"; wait for 100ns;
        assert ((s_B_greater_A = '1') and (s_B_equals_A = '1') and (s_B_less_A = '1'))
        report "Test failed for input combination: 0000, 0000" severity error;

-- ZDE JE SCHVALNE NAPSANA CHYBA
    
        report "Stimulus process finished" severity note;
        wait;
    end process p_stimulus;
```

2. Text console screenshot during your simulation, including reports.

   ![your figure]()

3. Link to your public EDA Playground example:

   [https://www.edaplayground.com/...](https://www.edaplayground.com/...)
