\# CPU Scheduling Simulator



A Python-based CPU Scheduling Simulator that implements and compares four fundamental CPU scheduling algorithms:



\* FCFS (First Come First Serve)

\* SJF (Shortest Job First)

\* Round Robin

\* Priority Scheduling



The simulator calculates important scheduling metrics and generates Gantt charts for visual comparison.



\## Features



\* Text-based Gantt charts

\* Completion Time (CT)

\* Turnaround Time (TAT)

\* Waiting Time (WT)

\* Response Time (RT)

\* Average WT, TAT and RT

\* Comparison of all four scheduling algorithms

\* CPU idle-time handling

\* Custom process input

\* CSV file input

\* Configurable Round Robin time quantum

\* Optional preemptive SJF (SRTF) and Priority scheduling

\* Matplotlib visualization with Gantt charts and comparison graphs



\## Algorithms



| Algorithm   | Type                      |

| ----------- | ------------------------- |

| FCFS        | Non-preemptive            |

| SJF         | Non-preemptive by default |

| Round Robin | Preemptive                |

| Priority    | Non-preemptive by default |



Lower priority numbers represent higher priority.



\## How to Run



\### Run the built-in demo



```bash

python cpu\_scheduler.py

```



\### Enter processes manually



```bash

python cpu\_scheduler.py -i

```



\### Use a CSV file



```bash

python cpu\_scheduler.py -f procs.csv

```



CSV format:



```text

pid,arrival,burst,priority

P1,0,8,2

P2,1,4,1

P3,2,6,3

```



\### Change Round Robin quantum



```bash

python cpu\_scheduler.py -q 4

```



\### Enable preemptive scheduling



```bash

python cpu\_scheduler.py --preemptive

```



\### Save the visualization



```bash

python cpu\_scheduler.py --save demo\_output.png --no-show

```



\## Demo Results



For the built-in demo:



\* \*\*SJF\*\* achieved the lowest average waiting time: \*\*6.20\*\*

\* \*\*SJF\*\* achieved the lowest average turnaround time: \*\*12.00\*\*

\* \*\*Round Robin\*\* achieved the lowest average response time: \*\*2.40\*\*



The generated visualization is available in \[`demo\_output.png`](demo\_output.png).



\## Technologies Used



\* Python

\* Matplotlib

\* Data Structures \& Algorithms

\* CPU Scheduling Concepts



\## Project Structure



```text

CPU Scheduler/

│

├── cpu\_scheduler.py

├── demo\_output.png

└── README.md

```



