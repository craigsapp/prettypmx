

all: output1 output1b output2

output1:
	../prettypmx input1.pmx > output1.pmx

output1b:
	../prettypmx -s "   " input1.pmx > output1b.pmx

output2:
	../prettypmx -s "  " input2.pmx > output2.pmx

clean:
	rm output*.pmx
