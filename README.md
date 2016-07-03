# EMPAthY86
A cycle accurate simulator for Explicitly Many-Processor Approach (EMPA) computer.
In computing, the 70-years old single-processor view dominates both hardware and software development.
For today, the development of single-processor performance has stalled, mainly because of using a
single-processor approach to computing. 

The Explicitly Many-Processor Approach considers explicitly (as opposed to out-of-order or speculativ evaluation,
where multiple processing units are considered only implicitly) that MANY computing units are present (here
primarily the many-core processors are considered). The basic idea is that when executing a task is delegated
to a processing unit (PU), and there are several similar processing units around, the original PU can
outsource part of its tasks to other PUs.

This approach assumes some new actors in the game: a supervisor above the cores, which can accept and fulfill
such requests for making distributed processing, a compiler which can analyze the code for possible (and efficient!)
outsourcing, and cores which can work under control of the supervisor, can work with partly outsourced
code and (through the supervisor) can communicate with each other. This requires to implement some new
functionalities in the processor, to rethink (primarily from the point of HW/SW joint performance point of view)
the complete computing stack, and to implement a new, but with the old one upward compatible, computing.
The consequences of introducing the approach are promiseful: the single processor performance increases
(depending on the utilization method and circumstances) up to several hundreds times, the real-time performance
(interrupt latency and predictability) considerably enhances, reaching good processor performance needs less
technologycal efforts (less transistors) and even the energy consumption can be enhanced.

On this site some tools for making computing in this style are presented. The main piece is an EMPA simulator,
which is able to simulate EMPA program execution (both in GUI and CLI interface style), an assembler which
can produce executable files for the simulator, some example programs and documentation.

The work is of 'alpha' quality (but works in expert hands), and is the result of efforts of a 'one-man team'.
Presently the source of the code is not yet mature enough to publish, and also the way of the distribution
is limited: only Linux executables without packaging are distributed. As the time proceeds (and resources allow)
the palette will be broadened.
