GS-TEC
======

Gaia SpectroPhotometry - Transient Events Classifier

This software classifies the spectra in Gaia BpRp format.

=== Prerequisites ==

- Include the environ variable GSTEC in your bash profile (.bashrc or .profile) pointing to the main folder containing the code:
i.ex.

export GSTEC=/Users/abc/Documents/GS-TEC

- Python libraries installed:
  - scipy
  - numpy
  - matplotlib
  - cosmolopy
  
=== USAGE ===

From src folder call the main class with the following parameters:

>python GSTEC

-p File containing the patterns (flux in BpRp format).
-e File containing the errors (errors in BpRpformat).
-n Number of processes to be created.
-l If plotting is required (false by default).


=== RESULTS ===
In the folder "data" the following results will appear:
- Folder "plots", plots of classified object (parameter determination and ranking aming classes) if option selected.
- Folder "results", a txt containing the reuslts of the execution and the parameters for each transient class.
