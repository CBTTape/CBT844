# CBT844
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 844 is from Kevin Ferguson, and contains his program      *   FILE 844
//*           called ENQWATCH.  This is a continuously running      *   FILE 844
//*           task that watches for dataset enqueue conflicts       *   FILE 844
//*           and informs the TSO user if he/she is the culprit.    *   FILE 844
//*           There is more there, too.  See the doc.               *   FILE 844
//*                                                                 *   FILE 844
//*           email:  Kevin.Ferguson@ANICO.com                      *   FILE 844
//*                                                                 *   FILE 844
//*     Documentation for this program is provided in PDF format,   *   FILE 844
//*     but an attempt was made to convert it as well as possible,  *   FILE 844
//*     to plain text format, so it could be more usable directly   *   FILE 844
//*     from the mainframe machine.                                 *   FILE 844
//*                                                                 *   FILE 844
//*     Program Overview                                            *   FILE 844
//*                                                                 *   FILE 844
//*     The program, ENQWATCH, is based around the IBM supplied     *   FILE 844
//*     program ISGECMON with the features of the David Alcock's    *   FILE 844
//*     ISGECMOM added and massively re-written and some 'bells     *   FILE 844
//*     and whistles' added.                                        *   FILE 844
//*                                                                 *   FILE 844
//*     ENQWATCH will only work for dataset conflicts between       *   FILE 844
//*     batch jobs and TSO users. Conflicts between two or more     *   FILE 844
//*     batch jobs are not handled by this program.                 *   FILE 844
//*                                                                 *   FILE 844
//*     It is designed to be used as a long running program, in     *   FILE 844
//*     fact it won't end at all until you issue a stop for, or     *   FILE 844
//*     cancel, it.  The purpose of the program is the monitor      *   FILE 844
//*     the system for any dataset contention and if the holder     *   FILE 844
//*     of the resource is a TSO user, it will send them a          *   FILE 844
//*     message requesting that they free the resource.             *   FILE 844
//*                                                                 *   FILE 844
//*     The added features of ENQWATCH include:                     *   FILE 844
//*                                                                 *   FILE 844
//*      *   The ability to force an iteration of the loop          *   FILE 844
//*          thereby allowing automation to be written to           *   FILE 844
//*          immediately send a message to a TSO user if they       *   FILE 844
//*          are holding up an important batch run.                 *   FILE 844
//*                                                                 *   FILE 844
//*      *   More statistics are available including how many       *   FILE 844
//*          times the iteration was forced by the above            *   FILE 844
//*          feature.                                               *   FILE 844
//*                                                                 *   FILE 844
//*      *   The program has been modified to allow commands        *   FILE 844
//*          to take effect immediately rather than wait            *   FILE 844
//*          until the loop time limit is met.                      *   FILE 844
//*                                                                 *   FILE 844
//*      *   Dynamic adjustment of the wait time limit is now       *   FILE 844
//*          supported.                                             *   FILE 844
//*                                                                 *   FILE 844
```
