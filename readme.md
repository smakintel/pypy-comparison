*DISTRIB_DESCRIPTION="Ubuntu 20.04.3 LTS"
*NAME="Ubuntu"
*VERSION="20.04.3 LTS (Focal Fossa)"
*ID=ubuntu
*ID_LIKE=debian
*PRETTY_NAME="Ubuntu 20.04.3 LTS"
*VERSION_ID="20.04"


    *-memory
          description: System memory
          physical id: 0
          size: 8GiB
     *-cpu
          product: Intel(R) Pentium(R) CPU G3250 @ 3.20GHz
          vendor: Intel Corp.
          physical id: 1
          bus info: cpu@0
          size: 2334MHz
          capacity: 3200MHz
          width: 64 bits

# for summing up 1000 numbers
* kenwyn@kenwyn-Lenovo-H30-50:~/repos/pypy-test$ pypy3 test-time.py 
* Sum of 1,000 numbers is :  499500
* Elapsed time is :  0.0002446174621582031  seconds
* kenwyn@kenwyn-Lenovo-H30-50:~/repos/pypy-test$ python3 test-time.py 
* Sum of 1,000 numbers is :  499500
* Elapsed time is :  0.00010323524475097656  seconds
*kenwyn@kenwyn-Lenovo-H30-50:~/repos/pypy-test$ `

cpython interpreter is the winner

# for summing up 10000000 numbers
* kenwyn@kenwyn-Lenovo-H30-50:~/repos/pypy-test$ pypy3 test-time.py 
* Sum of 1,000 numbers is :  49999995000000
* Elapsed time is :  0.019888877868652344  seconds
* kenwyn@kenwyn-Lenovo-H30-50:~/repos/pypy-test$ python3 test-time.py 
* Sum of 1,000 numbers is :  49999995000000
* Elapsed time is :  0.8334991931915283  seconds
* kenwyn@kenwyn-Lenovo-H30-50:~/repos/pypy-test$ 

for long running process pypy is the winner
for short running process cpython is the winner
