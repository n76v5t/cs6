java c
Complex Physics — Midterm Exam 1
It is allowed to work in groups, but each student must hand it in separately (without copying) and include information about collaborators. A maximum of three students are allowed per group.
You may use basic programming libraries where meaningful (e.g. general numerical routines), as long as they do not implement the Ising model for you (everything we use in the exercise solutions is OK).
For the hand-in, please include your code in a file separate from your report. We will not grade the quality of your code (only what is written in the report), but you must submit it. In total, 10 points can be achieved by solving the problems 1 and 2 below (see annotation), which map directly onto your grade (in percent of the total course grade). The remaining 90 percent can be obtained from a second midterm exam (10 percent) and the oral exam (80 percent). Note: 2 extra credits can optionally be achieved by also solving problem 3.

Figure 1: (a) Schematic showing the basic lattice. Any given site i has a connection to sites i − 1 and i + 1, modulo the lattice size N. Only three sites i − 1, i, i + 1 are highlighted in the schematic for presentation clarity. (b) An example where each node has connectivity four, that is, each node has the links shown in (a) and two additional random links (exemplified here only for one site i, other random links are not shown for clarity of presentation, but exist for each site).
Ising Model
Consider the two different lattice geometries in Fig. 1a and b. The schematic in Fig. 1a displays a one-dimensional periodic closed ring consisting of N sites, where each site has two nearest neighbors. The schematic in Fig. 1b shows a modification of the closed ring, where each of the N sites on average has two additional links to random sites so that each site now has an average of four nearest neighbors. Notice that t代 写Complex Physics — Midterm Exam 1R
代做程序编程语言hese neighbors have to be kept fixed during the simulation of a given system size. Also, be aware that if site i is neighbor to site j then site j is also neighbor to site i.
In each of these two cases place an electron of spin- 2/1 on each site — modeled as our usual Ising model with si = ±1. Let the energy of any configuration of spins be described by the familiar ferromagnetic zero-field Ising model (J > 0, h = 0), i.e.

where ⟨ij⟩ denotes any bond that exists between sites i and j in the geometries shown.
1. Implement the Ising model for both geometries. Using a Metropolis algorithm, plot the order parameter ⟨si⟩ vs. T. How does the order parameter depend on T in each case? You will need to simulate various values of T and you will need to ensure that you have simulated for a sufficiently long time. 5pt
2. Explore possible phase transition behavior. of each system. In particular, try to assess if a critical temperature Tc can be found for either of these two cases. Keep in mind that Tc relates to the behavior. in the thermodynamic limit, so, besides choosing a sufficiently long simulation time, you will need to extrapolate to infinite system size (i.e., 1/N → 0). Hint: Try plotting the absolute value of average magnetization |m| vs. T for various N and visually inspect the plots. Optionally, you can even try to automatize the identification of Tc for each finite system and then plot Tc vs. 1/N, to obtain a finite-size scaling. Try to interpret your findings w.r.t. the value of Tc in the thermodynamic limit. 5pt
3. Extra credit: In the case of Fig. 1a, try to support your reasoning about Tc by discussing the introduction of a domain wall and the associated free energy change. How would this reasoning change if you modified Fig. 1a so that each sites i has two further links to i − 2 and i + 2? 2pt







         
加QQ：99515681  WX：codinghelp
