# vulnerabilitydataset

C/C++ test cases formatted for input to an LSTM for natural language processing. All test cases originally come from the SARD database at https://samate.nist.gov/SARD/

finaltestcaselabels.csv holds the filename of each test case. filenames ending in 1 are vulnerable, 0 nonvulnerable. The first number corresponds to the array position of the vulnerability label in cwelabels.txt, and the second number the false positive vulnerability of the testcase.

ie, in the row: cpp\CWE-079\000001973_1.txt,10,0

cpp\CWE-079\000001973_1.txt is the filepath of the testcase.

10 is the 10th array position in cwelabels = "CWE-079: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')" which is the vulnerability of this testcase.

0 is the 0 position in the cwelabels array = "No Vulnerability" which is the possible false positive vulnerability of the testcase, in this example being none

In the nonvulnerable counterpart testcase "cpp\CWE-079\000001974_0.txt,0,10" the first number being 0 means there is no vulnerability in the testcase, and the second 10 means this case would be a false positive for CWE-079.
