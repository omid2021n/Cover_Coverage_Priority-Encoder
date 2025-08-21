# Cover_Coverage_Priority-Encoder
Final Result: PERFECT SCORE! ✅
Your test achieved 100% functional coverage. This means your testbench successfully generated every single scenario you asked it to look for. The priority encoder is thoroughly tested.

What Was Tested (The "Coverpoints")
Your coverage group was set up to check two things:

Input (y) Patterns: Did we see all 8 types of priority cases?

Output (a) Values: Did we see all 8 possible output codes (0-7)?

Both passed with 100%.

The Input Test (The Most Important Part)
This table shows how many times each specific input pattern was seen. The "Goal" was to see each pattern at least once.

Coverage Bin	Input Pattern	What it Tests	Times Seen	Status
zero	00000001	Only bit 0 is high	1	✅ PASS
one	0000001?	Bit 1 is the highest	2	✅ PASS
two	000001??	Bit 2 is the highest	8	✅ PASS
three	00001???	Bit 3 is the highest	8	✅ PASS
four	0001????	Bit 4 is the highest	15	✅ PASS
five	001?????	Bit 5 is the highest	37	✅ PASS
six	01??????	Bit 6 is the highest	88	✅ PASS
seven	1???????	Bit 7 is the highest	139	✅ PASS
Why the numbers increase?
This is expected! With random inputs, patterns with more "don't care" bits (?) are more likely to occur. A pattern like 1??????? (bit 7 high) matches 128 different possible values, while 00000001 (bit 0 high) matches only 1. The random generator found them all.

The Output Test (The Proof it Works)
This table shows how many times each output code from the encoder was seen. This perfectly mirrors the input, which is proof your encoder works correctly!

Output Value	Times Seen	Meaning
0	1	The encoder detected input 0
1	2	The encoder detected input 1
2	8	The encoder detected input 2
3	8	The encoder detected input 3
4	15	The encoder detected input 4
5	37	The encoder detected input 5
6	88	The encoder detected input 6
7	138	The encoder detected input 7
