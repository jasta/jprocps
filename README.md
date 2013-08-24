jprocps
=======

Collection of Java procps-like utilities (such as top, ps, etc)

jtop
----

jtop is the only tool currently implemented, providing a top-like interface for
visualizing CPU usage of Java threads.  This is intended to give you a clue
what to look for when troubleshooting very large or complex multi-threaded Java
applications using jconsole or a traditional debugger.  Looking at you,
IntelliJ.

Sample Output
-------------

<pre>
  PID   TID USER       %CPU  %MEM  THREAD
13480 13483 jasta      104   2.3   main
13480 13497 jasta      86.3  2.3   C2 CompilerThread1
13480 13496 jasta      83.0  2.3   C2 CompilerThread0
 4866  4953 jasta      1.0   13.4  AWT-EventQueue-1 12.1.4#IC-129.713, eap:false
 4866 14154 jasta      0.9   13.4  ApplicationImpl pooled thread 36
 4866  5219 jasta      0.8   13.4  JobScheduler pool 5/8
</pre>
