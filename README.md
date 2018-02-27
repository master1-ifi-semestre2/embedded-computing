# embedded-computing

```markdown
>>>[example_cmu] NuSMV -int short.smv 
*** This is NuSMV 2.6.0 (compiled on Wed Oct 14 15:32:58 2015)
*** Enabled addons are: compass
*** For more information on NuSMV see <http://nusmv.fbk.eu>
*** or email to <nusmv-users@list.fbk.eu>.
*** Please report bugs to <Please report bugs to <nusmv-users@fbk.eu>>

*** Copyright (c) 2010-2014, Fondazione Bruno Kessler

*** This version of NuSMV is linked to the CUDD library version 2.4.1
*** Copyright (c) 1995-2004, Regents of the University of Colorado

*** This version of NuSMV is linked to the MiniSat SAT solver. 
*** See http://minisat.se/MiniSat.html
*** Copyright (c) 2003-2006, Niklas Een, Niklas Sorensson
*** Copyright (c) 2007-2010, Niklas Sorensson

NuSMV > go
NuSMV > pick_state -r
NuSMV > pick_state 
counter.smv   dme1.smv      dme2.smv      mutex.smv     README        short.smv    
dme1.opt      dme2.opt      gigamax.ord   mutex1.smv    ring.smv      syncarb5.smv 
dme1.ord      dme2.ord      gigamax.smv   periodic.smv  semaphore.smv
NuSMV > print_current_state -v
Current state is 1.1
request = FALSE
state = ready
NuSMV > simulate -r -k 3
********  Simulation Starting From State 1.1   ********
NuSMV > show_traces -t
There is 1 trace currently available.
NuSMV > show_traces -v
    <!-- ################### Trace number: 1 ################### -->
Trace Description: Simulation Trace 
Trace Type: Simulation 
  -> State: 1.1 <-
    request = FALSE
    state = ready
  -> State: 1.2 <-
    request = TRUE
    state = ready
  -> State: 1.3 <-
    request = TRUE
    state = busy
  -> State: 1.4 <-
    request = FALSE
    state = ready
NuSMV > quit
>>>[example_cmu] 
```