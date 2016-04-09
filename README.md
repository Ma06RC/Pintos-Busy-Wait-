# Pintos-Busy-Wait-
Previous implementation of sleep uses busy wait. Therefore, my objective is to get rid of busy waiting as it waste CPU cycles, which is inefficient.

  - Methods that I re-implemented are timer_sleep() and timer_interrupt() in src/devices/timer.c
  - I also added a comparator method for comparing the sleeping time for two thread's so that they are ordered in the list when they are added
  - I was able to pass every single test cases for this project. 
      - alarm-single
      - alarm-multiple
      - alarm-simultaneous  
      - alarm-zero
      - alarm-negative
  - To compile and run, go to terminal. cd to where pintos file is, then:
      - %>cd src/threads
      - %>make 
      - %>cd build
      - Now you can run the test either you type in %>make check for running automated test or %>make grade for running grading script
