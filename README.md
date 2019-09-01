# rpispeed

This program displays the cpu speed of the processor cores of your Pi in BogoMIPS in real time.

Rpispeed, written in Java, uses Tkinter to display the realtime cpu speed of your Raspberry Pi. It uses the system file /proc/cpuinfo to capture the speed in BogoMIPS. It first captures the model information, such as ARMv7 and the revision details, then counts the number of cpu cores. Once the line for the cpeed count of each core is identified it drops into a continuous loop that checks for changes about twice per second, and updates the display if any changes are found.
