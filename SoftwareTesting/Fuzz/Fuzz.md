# Fuzzing
### **Definition**
Inject random or invalid data into the software to find implementation bugs.

<br>

### **Fuzzer**
(Fuzzer is a program that injects data into program or stack.)<br>

- Mutation-Based Fuzzers
    - Alert original datasets to create new testing datasets.

<br>

- Generation-Based Fuzzers
    - Create datasets from scratch based on inputs.

<br>

- Protocol-Based Fuzzers
    - Find irregularity based on the protocol.
        - e.g. grammar check

<br>

### **Implementation**
(Steps to implement fuzz testing.)

1) Prepare the target system.

2) Prepare the inputs.

3) Use the Fuzzer to generate datasets.  ||  Prepare the datasets.

4) Use datasets to do the testing.

5) Monitor system's behavior.

6) Defect Logging

<br>

### **Tools**
[American Fuzzy Lop plus plus (afl++)](https://aflplus.plus)<br>

[Honggfuzz](https://honggfuzz.dev/)

<br>

### **Papers**
[research gate](https://www.researchgate.net/search/publication?q=black-box%2Btesting%2B)<br>

[A Survey of Methods for Explaining Black Box Models](https://www.researchgate.net/publication/322976218_A_Survey_of_Methods_for_Explaining_Black_Box_Models)<br>

[Software testing: A survey and tutorial on white and black-box testing of C/C++ programs](https://www.researchgate.net/publication/305649292_Software_testing_A_survey_and_tutorial_on_white_and_black-box_testing_of_CC_programs)

