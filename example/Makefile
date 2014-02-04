

all: output1 output1b output1c output2

output1:
	../prettypmx input1.pmx > output1.pmx

# Example adding "   " space between columns:
output1b:
	../prettypmx -s "   " input1.pmx > output1b.pmx

# Example giving minimal spacing between numbers on each line
# (columns may not line up when -m is used).
output1c:
	../prettypmx -m input1.pmx > output1c.pmx

output2:
	../prettypmx -s "  " input2.pmx > output2.pmx

clean:
	rm output*.pmx
