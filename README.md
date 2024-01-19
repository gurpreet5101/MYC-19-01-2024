# MYC-19-01-2024

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx grompp -f step4.0_minimization.mdp -o minimization.tpr -c step3_input.gro  -r step3_input.gro -p topol.top
                       :-) GROMACS - gmx grompp, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx grompp -f step4.0_minimization.mdp -o minimization.tpr -c step3_input.gro -r step3_input.gro -p topol.top

Setting the LD random seed to -1149840641

Generated 627 of the 630 non-bonded parameter combinations
Generating 1-4 interactions: fudge = 1

Generated 325 of the 630 1-4 parameter combinations

Excluding 3 bonded neighbours molecule type 'PROA'

turning H bonds into constraints...

Excluding 1 bonded neighbours molecule type 'POT'

turning H bonds into constraints...

Excluding 1 bonded neighbours molecule type 'CLA'

turning H bonds into constraints...

Excluding 2 bonded neighbours molecule type 'TIP3'

turning H bonds into constraints...
Analysing residue names:
There are:    80    Protein residues
There are: 40263      Other residues
Analysing Protein...
Analysing residues not classified as Protein/DNA/RNA/Water and splitting into groups...
Number of degrees of freedom in T-Coupling group rest is 244329.00
The integrator does not provide a ensemble temperature, there is no system ensemble temperature

The largest distance between excluded atoms is 0.394 nm between atom 526 and 534

NOTE 1 [file step4.0_minimization.mdp]:
  Removing center of mass motion in the presence of position restraints
  might cause artifacts. When you are using position restraints to
  equilibrate a macro-molecule, the artifacts are usually negligible.

Calculating fourier grid dimensions for X Y Z
Using a fourier grid of 96x96x96, spacing 0.114 0.114 0.114

Estimate for the relative computational load of the PME mesh part: 0.05

This run will generate roughly 9 Mb of data

There was 1 NOTE

GROMACS reminds you: "Since the mathematicians have invaded the theory of relativity I do not understand it myself any more." (Albert Einstein)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx mdrun -v -deffnm minimization
                       :-) GROMACS - gmx mdrun, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx mdrun -v -deffnm minimization

Compiled SIMD: None, but for this host/run AVX2_256 might be better (see log).
Reading file minimization.tpr, VERSION 2023 (single precision)
1 GPU selected for this run.
Mapping of GPU IDs to the 1 GPU task in the 1 rank on this node:
  PP:0
PP tasks will do (non-perturbed) short-ranged interactions on the GPU
PP task will update and constrain coordinates on the CPU
Using 1 MPI thread
Using 16 OpenMP threads 


Steepest Descents:
   Tolerance (Fmax)   =  1.00000e+03
   Number of steps    =         5000
Step=    0, Dmax= 1.0e-02 nm, Epot= -1.93202e+06 Fmax= 2.07569e+04, atom= 213
Step=    1, Dmax= 1.0e-02 nm, Epot= -1.93252e+06 Fmax= 4.68300e+03, atom= 211
Step=    2, Dmax= 1.2e-02 nm, Epot= -1.93353e+06 Fmax= 3.34274e+03, atom= 212
Step=    3, Dmax= 1.4e-02 nm, Epot= -1.93393e+06 Fmax= 1.06917e+04, atom= 211
Step=    4, Dmax= 1.7e-02 nm, Epot= -1.93465e+06 Fmax= 9.54183e+03, atom= 211
Step=    6, Dmax= 1.0e-02 nm, Epot= -1.93553e+06 Fmax= 3.63384e+03, atom= 211
Step=    7, Dmax= 1.2e-02 nm, Epot= -1.93554e+06 Fmax= 1.08555e+04, atom= 211
Step=    8, Dmax= 1.5e-02 nm, Epot= -1.93626e+06 Fmax= 7.74382e+03, atom= 211
Step=   10, Dmax= 9.0e-03 nm, Epot= -1.93692e+06 Fmax= 3.07591e+03, atom= 823
Step=   12, Dmax= 5.4e-03 nm, Epot= -1.93726e+06 Fmax= 3.85112e+03, atom= 823
Step=   13, Dmax= 6.4e-03 nm, Epot= -1.93757e+06 Fmax= 4.42476e+03, atom= 823
Step=   14, Dmax= 7.7e-03 nm, Epot= -1.93782e+06 Fmax= 5.54052e+03, atom= 823
Step=   15, Dmax= 9.3e-03 nm, Epot= -1.93806e+06 Fmax= 6.38516e+03, atom= 823
Step=   16, Dmax= 1.1e-02 nm, Epot= -1.93816e+06 Fmax= 7.95743e+03, atom= 823
Step=   17, Dmax= 1.3e-02 nm, Epot= -1.93826e+06 Fmax= 9.22410e+03, atom= 823
Step=   19, Dmax= 8.0e-03 nm, Epot= -1.93944e+06 Fmax= 1.25065e+03, atom= 41
Step=   20, Dmax= 9.6e-03 nm, Epot= -1.93984e+06 Fmax= 1.09844e+04, atom= 41
Step=   21, Dmax= 1.2e-02 nm, Epot= -1.94107e+06 Fmax= 4.08515e+03, atom= 41
Step=   23, Dmax= 6.9e-03 nm, Epot= -1.94133e+06 Fmax= 4.87300e+03, atom= 41
Step=   24, Dmax= 8.3e-03 nm, Epot= -1.94156e+06 Fmax= 5.98617e+03, atom= 41
Step=   25, Dmax= 1.0e-02 nm, Epot= -1.94178e+06 Fmax= 6.95997e+03, atom= 851
Step=   26, Dmax= 1.2e-02 nm, Epot= -1.94190e+06 Fmax= 8.62787e+03, atom= 851
Step=   27, Dmax= 1.4e-02 nm, Epot= -1.94201e+06 Fmax= 1.02245e+04, atom= 851
Step=   29, Dmax= 8.6e-03 nm, Epot= -1.94297e+06 Fmax= 1.06293e+03, atom= 851
Step=   30, Dmax= 1.0e-02 nm, Epot= -1.94385e+06 Fmax= 1.26587e+04, atom= 851
Step=   31, Dmax= 1.2e-02 nm, Epot= -1.94486e+06 Fmax= 3.56901e+03, atom= 851
Step=   33, Dmax= 7.5e-03 nm, Epot= -1.94510e+06 Fmax= 6.24110e+03, atom= 851
Step=   34, Dmax= 8.9e-03 nm, Epot= -1.94540e+06 Fmax= 5.40545e+03, atom= 851
Step=   35, Dmax= 1.1e-02 nm, Epot= -1.94553e+06 Fmax= 8.68289e+03, atom= 851
Step=   36, Dmax= 1.3e-02 nm, Epot= -1.94584e+06 Fmax= 8.09676e+03, atom= 851
Step=   38, Dmax= 7.7e-03 nm, Epot= -1.94629e+06 Fmax= 1.99410e+03, atom= 851
Step=   39, Dmax= 9.3e-03 nm, Epot= -1.94667e+06 Fmax= 1.00071e+04, atom= 851
Step=   40, Dmax= 1.1e-02 nm, Epot= -1.94720e+06 Fmax= 4.53753e+03, atom= 851
Step=   42, Dmax= 6.7e-03 nm, Epot= -1.94746e+06 Fmax= 4.15504e+03, atom= 851
Step=   43, Dmax= 8.0e-03 nm, Epot= -1.94769e+06 Fmax= 6.35750e+03, atom= 851
Step=   44, Dmax= 9.6e-03 nm, Epot= -1.94796e+06 Fmax= 6.16478e+03, atom= 851
Step=   45, Dmax= 1.2e-02 nm, Epot= -1.94811e+06 Fmax= 8.96375e+03, atom= 851
Step=   46, Dmax= 1.4e-02 nm, Epot= -1.94836e+06 Fmax= 9.07135e+03, atom= 851
Step=   47, Dmax= 1.7e-02 nm, Epot= -1.94839e+06 Fmax= 1.27097e+04, atom= 851
Step=   48, Dmax= 2.0e-02 nm, Epot= -1.94860e+06 Fmax= 1.32545e+04, atom= 851
Step=   50, Dmax= 1.2e-02 nm, Epot= -1.94934e+06 Fmax= 2.32106e+03, atom= 851
Step=   51, Dmax= 1.4e-02 nm, Epot= -1.94948e+06 Fmax= 1.62959e+04, atom= 851
Step=   52, Dmax= 1.7e-02 nm, Epot= -1.95039e+06 Fmax= 6.18574e+03, atom= 851
Step=   54, Dmax= 1.0e-02 nm, Epot= -1.95060e+06 Fmax= 7.26721e+03, atom= 851
Step=   55, Dmax= 1.2e-02 nm, Epot= -1.95079e+06 Fmax= 8.97902e+03, atom= 851
Step=   56, Dmax= 1.5e-02 nm, Epot= -1.95097e+06 Fmax= 1.03991e+04, atom= 851
Step=   57, Dmax= 1.8e-02 nm, Epot= -1.95106e+06 Fmax= 1.29965e+04, atom= 851
Step=   58, Dmax= 2.1e-02 nm, Epot= -1.95116e+06 Fmax= 1.48985e+04, atom= 851
Step=   60, Dmax= 1.3e-02 nm, Epot= -1.95193e+06 Fmax= 1.82587e+03, atom= 851
Step=   61, Dmax= 1.5e-02 nm, Epot= -1.95230e+06 Fmax= 1.82066e+04, atom= 851
Step=   62, Dmax= 1.9e-02 nm, Epot= -1.95328e+06 Fmax= 5.95566e+03, atom= 851
Step=   64, Dmax= 1.1e-02 nm, Epot= -1.95346e+06 Fmax= 8.48183e+03, atom= 851
Step=   65, Dmax= 1.3e-02 nm, Epot= -1.95367e+06 Fmax= 8.97284e+03, atom= 851
Step=   66, Dmax= 1.6e-02 nm, Epot= -1.95378e+06 Fmax= 1.18447e+04, atom= 851
Step=   67, Dmax= 1.9e-02 nm, Epot= -1.95393e+06 Fmax= 1.32898e+04, atom= 851
Step=   69, Dmax= 1.2e-02 nm, Epot= -1.95450e+06 Fmax= 1.79943e+03, atom= 851
Step=   70, Dmax= 1.4e-02 nm, Epot= -1.95500e+06 Fmax= 1.63505e+04, atom= 851
Step=   71, Dmax= 1.7e-02 nm, Epot= -1.95570e+06 Fmax= 5.33472e+03, atom= 851
Step=   73, Dmax= 1.0e-02 nm, Epot= -1.95589e+06 Fmax= 7.71431e+03, atom= 851
Step=   74, Dmax= 1.2e-02 nm, Epot= -1.95611e+06 Fmax= 7.84340e+03, atom= 851
Step=   75, Dmax= 1.4e-02 nm, Epot= -1.95624e+06 Fmax= 1.09307e+04, atom= 851
Step=   76, Dmax= 1.7e-02 nm, Epot= -1.95643e+06 Fmax= 1.14713e+04, atom= 851
Step=   77, Dmax= 2.1e-02 nm, Epot= -1.95644e+06 Fmax= 1.55689e+04, atom= 851
Step=   78, Dmax= 2.5e-02 nm, Epot= -1.95658e+06 Fmax= 1.66704e+04, atom= 851
Step=   80, Dmax= 1.5e-02 nm, Epot= -1.95730e+06 Fmax= 2.63989e+03, atom= 851
Step=   81, Dmax= 1.8e-02 nm, Epot= -1.95733e+06 Fmax= 2.05394e+04, atom= 851
Step=   82, Dmax= 2.1e-02 nm, Epot= -1.95827e+06 Fmax= 7.35951e+03, atom= 851
Step=   84, Dmax= 1.3e-02 nm, Epot= -1.95843e+06 Fmax= 9.34744e+03, atom= 851
Step=   85, Dmax= 1.5e-02 nm, Epot= -1.95860e+06 Fmax= 1.08163e+04, atom= 851
Step=   86, Dmax= 1.8e-02 nm, Epot= -1.95871e+06 Fmax= 1.32471e+04, atom= 851
Step=   87, Dmax= 2.2e-02 nm, Epot= -1.95879e+06 Fmax= 1.57987e+04, atom= 851
Step=   89, Dmax= 1.3e-02 nm, Epot= -1.95940e+06 Fmax= 1.65534e+03, atom= 851
Step=   90, Dmax= 1.6e-02 nm, Epot= -1.95998e+06 Fmax= 1.92581e+04, atom= 851
Step=   91, Dmax= 1.9e-02 nm, Epot= -1.96074e+06 Fmax= 5.80896e+03, atom= 851
Step=   93, Dmax= 1.1e-02 nm, Epot= -1.96090e+06 Fmax= 9.28903e+03, atom= 851
Step=   94, Dmax= 1.4e-02 nm, Epot= -1.96111e+06 Fmax= 8.69289e+03, atom= 851
Step=   95, Dmax= 1.7e-02 nm, Epot= -1.96119e+06 Fmax= 1.30062e+04, atom= 851
Step=   96, Dmax= 2.0e-02 nm, Epot= -1.96139e+06 Fmax= 1.28853e+04, atom= 851
Step=   98, Dmax= 1.2e-02 nm, Epot= -1.96180e+06 Fmax= 2.63255e+03, atom= 851
Step=   99, Dmax= 1.4e-02 nm, Epot= -1.96203e+06 Fmax= 1.59641e+04, atom= 851
Step=  100, Dmax= 1.7e-02 nm, Epot= -1.96257e+06 Fmax= 6.43084e+03, atom= 851
Step=  102, Dmax= 1.0e-02 nm, Epot= -1.96276e+06 Fmax= 6.99451e+03, atom= 851
Step=  103, Dmax= 1.2e-02 nm, Epot= -1.96291e+06 Fmax= 9.18516e+03, atom= 851
Step=  104, Dmax= 1.5e-02 nm, Epot= -1.96308e+06 Fmax= 1.01418e+04, atom= 851
Step=  105, Dmax= 1.8e-02 nm, Epot= -1.96318e+06 Fmax= 1.31655e+04, atom= 851
Step=  106, Dmax= 2.1e-02 nm, Epot= -1.96330e+06 Fmax= 1.46500e+04, atom= 851
Step=  108, Dmax= 1.3e-02 nm, Epot= -1.96378e+06 Fmax= 2.01507e+03, atom= 851
Step=  109, Dmax= 1.5e-02 nm, Epot= -1.96414e+06 Fmax= 1.79941e+04, atom= 851
Step=  110, Dmax= 1.8e-02 nm, Epot= -1.96478e+06 Fmax= 6.07724e+03, atom= 851
Step=  112, Dmax= 1.1e-02 nm, Epot= -1.96494e+06 Fmax= 8.33012e+03, atom= 851
Step=  113, Dmax= 1.3e-02 nm, Epot= -1.96512e+06 Fmax= 9.05718e+03, atom= 851
Step=  114, Dmax= 1.6e-02 nm, Epot= -1.96523e+06 Fmax= 1.17030e+04, atom= 851
Step=  115, Dmax= 1.9e-02 nm, Epot= -1.96536e+06 Fmax= 1.33402e+04, atom= 851
Step=  116, Dmax= 2.3e-02 nm, Epot= -1.96540e+06 Fmax= 1.65396e+04, atom= 851
Step=  117, Dmax= 2.8e-02 nm, Epot= -1.96542e+06 Fmax= 1.95452e+04, atom= 851
Step=  119, Dmax= 1.7e-02 nm, Epot= -1.96617e+06 Fmax= 2.16141e+03, atom= 851
Step=  120, Dmax= 2.0e-02 nm, Epot= -1.96635e+06 Fmax= 2.37757e+04, atom= 851
Step=  121, Dmax= 2.4e-02 nm, Epot= -1.96728e+06 Fmax= 7.38367e+03, atom= 851
Step=  123, Dmax= 1.4e-02 nm, Epot= -1.96739e+06 Fmax= 1.13680e+04, atom= 851
Step=  124, Dmax= 1.7e-02 nm, Epot= -1.96757e+06 Fmax= 1.09658e+04, atom= 851
Step=  125, Dmax= 2.1e-02 nm, Epot= -1.96758e+06 Fmax= 1.59888e+04, atom= 851
Step=  126, Dmax= 2.5e-02 nm, Epot= -1.96774e+06 Fmax= 1.61614e+04, atom= 851
Step=  128, Dmax= 1.5e-02 nm, Epot= -1.96825e+06 Fmax= 3.08630e+03, atom= 851
Step=  129, Dmax= 1.8e-02 nm, Epot= -1.96827e+06 Fmax= 2.00353e+04, atom= 851
Step=  130, Dmax= 2.1e-02 nm, Epot= -1.96894e+06 Fmax= 7.76375e+03, atom= 851
Step=  132, Dmax= 1.3e-02 nm, Epot= -1.96909e+06 Fmax= 8.91124e+03, atom= 851
Step=  133, Dmax= 1.5e-02 nm, Epot= -1.96922e+06 Fmax= 1.11797e+04, atom= 851
Step=  134, Dmax= 1.8e-02 nm, Epot= -1.96934e+06 Fmax= 1.28212e+04, atom= 851
Step=  135, Dmax= 2.2e-02 nm, Epot= -1.96938e+06 Fmax= 1.61274e+04, atom= 851
Step=  136, Dmax= 2.7e-02 nm, Epot= -1.96944e+06 Fmax= 1.84044e+04, atom= 851
Step=  138, Dmax= 1.6e-02 nm, Epot= -1.97006e+06 Fmax= 2.26179e+03, atom= 851
Step=  139, Dmax= 1.9e-02 nm, Epot= -1.97018e+06 Fmax= 2.26474e+04, atom= 851
Step=  140, Dmax= 2.3e-02 nm, Epot= -1.97102e+06 Fmax= 7.23738e+03, atom= 851
Step=  142, Dmax= 1.4e-02 nm, Epot= -1.97113e+06 Fmax= 1.06413e+04, atom= 851
Step=  143, Dmax= 1.7e-02 nm, Epot= -1.97130e+06 Fmax= 1.09504e+04, atom= 851
Step=  144, Dmax= 2.0e-02 nm, Epot= -1.97133e+06 Fmax= 1.48231e+04, atom= 851
Step=  145, Dmax= 2.4e-02 nm, Epot= -1.97144e+06 Fmax= 1.62792e+04, atom= 851
Step=  147, Dmax= 1.4e-02 nm, Epot= -1.97194e+06 Fmax= 2.42307e+03, atom= 851
Step=  148, Dmax= 1.7e-02 nm, Epot= -1.97211e+06 Fmax= 1.99794e+04, atom= 851
Step=  149, Dmax= 2.1e-02 nm, Epot= -1.97274e+06 Fmax= 6.88857e+03, atom= 851
Step=  151, Dmax= 1.2e-02 nm, Epot= -1.97287e+06 Fmax= 9.24414e+03, atom= 851
Step=  152, Dmax= 1.5e-02 nm, Epot= -1.97301e+06 Fmax= 1.00245e+04, atom= 851
Step=  153, Dmax= 1.8e-02 nm, Epot= -1.97310e+06 Fmax= 1.32016e+04, atom= 851
Step=  154, Dmax= 2.1e-02 nm, Epot= -1.97320e+06 Fmax= 1.45320e+04, atom= 851
Step=  156, Dmax= 1.3e-02 nm, Epot= -1.97361e+06 Fmax= 2.07624e+03, atom= 851
Step=  157, Dmax= 1.5e-02 nm, Epot= -1.97390e+06 Fmax= 1.78957e+04, atom= 851
Step=  158, Dmax= 1.8e-02 nm, Epot= -1.97443e+06 Fmax= 6.09169e+03, atom= 851
Step=  160, Dmax= 1.1e-02 nm, Epot= -1.97457e+06 Fmax= 8.27825e+03, atom= 851
Step=  161, Dmax= 1.3e-02 nm, Epot= -1.97471e+06 Fmax= 9.04648e+03, atom= 851
Step=  162, Dmax= 1.6e-02 nm, Epot= -1.97481e+06 Fmax= 1.16544e+04, atom= 851
Step=  163, Dmax= 1.9e-02 nm, Epot= -1.97492e+06 Fmax= 1.33014e+04, atom= 851
Step=  164, Dmax= 2.3e-02 nm, Epot= -1.97495e+06 Fmax= 1.64893e+04, atom= 851
Step=  165, Dmax= 2.7e-02 nm, Epot= -1.97497e+06 Fmax= 1.94725e+04, atom= 851
Step=  167, Dmax= 1.6e-02 nm, Epot= -1.97561e+06 Fmax= 2.16639e+03, atom= 851
Step=  168, Dmax= 2.0e-02 nm, Epot= -1.97575e+06 Fmax= 2.36639e+04, atom= 851
Step=  169, Dmax= 2.4e-02 nm, Epot= -1.97655e+06 Fmax= 7.39918e+03, atom= 851
Step=  171, Dmax= 1.4e-02 nm, Epot= -1.97665e+06 Fmax= 1.12843e+04, atom= 851
Step=  172, Dmax= 1.7e-02 nm, Epot= -1.97680e+06 Fmax= 1.09829e+04, atom= 851
Step=  173, Dmax= 2.1e-02 nm, Epot= -1.97681e+06 Fmax= 1.58783e+04, atom= 851
Step=  174, Dmax= 2.5e-02 nm, Epot= -1.97694e+06 Fmax= 1.61742e+04, atom= 851
Step=  176, Dmax= 1.5e-02 nm, Epot= -1.97738e+06 Fmax= 3.00965e+03, atom= 851
Step=  177, Dmax= 1.8e-02 nm, Epot= -1.97741e+06 Fmax= 2.00563e+04, atom= 851
Step=  178, Dmax= 2.1e-02 nm, Epot= -1.97800e+06 Fmax= 7.65030e+03, atom= 851
Step=  180, Dmax= 1.3e-02 nm, Epot= -1.97813e+06 Fmax= 8.97446e+03, atom= 851
Step=  181, Dmax= 1.5e-02 nm, Epot= -1.97824e+06 Fmax= 1.10466e+04, atom= 851
Step=  182, Dmax= 1.8e-02 nm, Epot= -1.97834e+06 Fmax= 1.28814e+04, atom= 851
Step=  183, Dmax= 2.2e-02 nm, Epot= -1.97838e+06 Fmax= 1.59686e+04, atom= 851
Step=  184, Dmax= 2.6e-02 nm, Epot= -1.97841e+06 Fmax= 1.84569e+04, atom= 851
Step=  186, Dmax= 1.6e-02 nm, Epot= -1.97896e+06 Fmax= 2.14078e+03, atom= 851
Step=  187, Dmax= 1.9e-02 nm, Epot= -1.97907e+06 Fmax= 2.27195e+04, atom= 851
Step=  188, Dmax= 2.3e-02 nm, Epot= -1.97985e+06 Fmax= 7.06914e+03, atom= 851
Step=  190, Dmax= 1.4e-02 nm, Epot= -1.97993e+06 Fmax= 1.07511e+04, atom= 851
Step=  191, Dmax= 1.6e-02 nm, Epot= -1.98008e+06 Fmax= 1.07674e+04, atom= 851
Step=  192, Dmax= 2.0e-02 nm, Epot= -1.98010e+06 Fmax= 1.49268e+04, atom= 851
Step=  193, Dmax= 2.4e-02 nm, Epot= -1.98020e+06 Fmax= 1.60702e+04, atom= 851
Step=  195, Dmax= 1.4e-02 nm, Epot= -1.98063e+06 Fmax= 2.57273e+03, atom= 851
Step=  196, Dmax= 1.7e-02 nm, Epot= -1.98073e+06 Fmax= 1.97519e+04, atom= 851
Step=  197, Dmax= 2.0e-02 nm, Epot= -1.98129e+06 Fmax= 7.03287e+03, atom= 851
Step=  199, Dmax= 1.2e-02 nm, Epot= -1.98140e+06 Fmax= 9.03830e+03, atom= 851
Step=  200, Dmax= 1.5e-02 nm, Epot= -1.98152e+06 Fmax= 1.01730e+04, atom= 851
Step=  201, Dmax= 1.8e-02 nm, Epot= -1.98159e+06 Fmax= 1.29723e+04, atom= 851
Step=  202, Dmax= 2.1e-02 nm, Epot= -1.98167e+06 Fmax= 1.46753e+04, atom= 851
Step=  204, Dmax= 1.3e-02 nm, Epot= -1.98204e+06 Fmax= 1.87690e+03, atom= 851
Step=  205, Dmax= 1.5e-02 nm, Epot= -1.98232e+06 Fmax= 1.80574e+04, atom= 851
Step=  206, Dmax= 1.8e-02 nm, Epot= -1.98283e+06 Fmax= 5.85364e+03, atom= 851
Step=  208, Dmax= 1.1e-02 nm, Epot= -1.98294e+06 Fmax= 8.46758e+03, atom= 851
Step=  209, Dmax= 1.3e-02 nm, Epot= -1.98307e+06 Fmax= 8.79845e+03, atom= 851
Step=  210, Dmax= 1.6e-02 nm, Epot= -1.98314e+06 Fmax= 1.18375e+04, atom= 851
Step=  211, Dmax= 1.9e-02 nm, Epot= -1.98325e+06 Fmax= 1.30333e+04, atom= 851
Step=  213, Dmax= 1.1e-02 nm, Epot= -1.98355e+06 Fmax= 1.91713e+03, atom= 851
Step=  214, Dmax= 1.4e-02 nm, Epot= -1.98384e+06 Fmax= 1.59925e+04, atom= 851
Step=  215, Dmax= 1.6e-02 nm, Epot= -1.98423e+06 Fmax= 5.49387e+03, atom= 851
Step=  217, Dmax= 9.9e-03 nm, Epot= -1.98435e+06 Fmax= 7.40576e+03, atom= 851
Step=  218, Dmax= 1.2e-02 nm, Epot= -1.98448e+06 Fmax= 8.01610e+03, atom= 851
Step=  219, Dmax= 1.4e-02 nm, Epot= -1.98457e+06 Fmax= 1.05566e+04, atom= 851
Step=  220, Dmax= 1.7e-02 nm, Epot= -1.98467e+06 Fmax= 1.16428e+04, atom= 851
Step=  221, Dmax= 2.0e-02 nm, Epot= -1.98471e+06 Fmax= 1.51150e+04, atom= 851
Step=  222, Dmax= 2.5e-02 nm, Epot= -1.98477e+06 Fmax= 1.68268e+04, atom= 851
Step=  224, Dmax= 1.5e-02 nm, Epot= -1.98522e+06 Fmax= 2.28816e+03, atom= 851
Step=  225, Dmax= 1.8e-02 nm, Epot= -1.98529e+06 Fmax= 2.07430e+04, atom= 851
Step=  226, Dmax= 2.1e-02 nm, Epot= -1.98591e+06 Fmax= 6.88056e+03, atom= 851
Step=  228, Dmax= 1.3e-02 nm, Epot= -1.98600e+06 Fmax= 9.66813e+03, atom= 851
Step=  229, Dmax= 1.5e-02 nm, Epot= -1.98612e+06 Fmax= 1.02867e+04, atom= 851
Step=  230, Dmax= 1.8e-02 nm, Epot= -1.98616e+06 Fmax= 1.35554e+04, atom= 851
Step=  231, Dmax= 2.2e-02 nm, Epot= -1.98624e+06 Fmax= 1.51916e+04, atom= 851
Step=  233, Dmax= 1.3e-02 nm, Epot= -1.98662e+06 Fmax= 2.09661e+03, atom= 851
Step=  234, Dmax= 1.6e-02 nm, Epot= -1.98680e+06 Fmax= 1.85897e+04, atom= 851
Step=  235, Dmax= 1.9e-02 nm, Epot= -1.98729e+06 Fmax= 6.24810e+03, atom= 851
Step=  237, Dmax= 1.1e-02 nm, Epot= -1.98738e+06 Fmax= 8.66471e+03, atom= 851
Step=  238, Dmax= 1.4e-02 nm, Epot= -1.98751e+06 Fmax= 9.15600e+03, atom= 851
Step=  239, Dmax= 1.6e-02 nm, Epot= -1.98756e+06 Fmax= 1.23110e+04, atom= 851
Step=  240, Dmax= 2.0e-02 nm, Epot= -1.98765e+06 Fmax= 1.33389e+04, atom= 851
Step=  242, Dmax= 1.2e-02 nm, Epot= -1.98796e+06 Fmax= 2.01953e+03, atom= 851
Step=  243, Dmax= 1.4e-02 nm, Epot= -1.98817e+06 Fmax= 1.64560e+04, atom= 851
Step=  244, Dmax= 1.7e-02 nm, Epot= -1.98858e+06 Fmax= 5.71810e+03, atom= 851
Step=  246, Dmax= 1.0e-02 nm, Epot= -1.98869e+06 Fmax= 7.57707e+03, atom= 851
Step=  247, Dmax= 1.2e-02 nm, Epot= -1.98879e+06 Fmax= 8.43394e+03, atom= 851
Step=  248, Dmax= 1.5e-02 nm, Epot= -1.98888e+06 Fmax= 1.07124e+04, atom= 851
Step=  249, Dmax= 1.8e-02 nm, Epot= -1.98896e+06 Fmax= 1.23524e+04, atom= 851
Step=  250, Dmax= 2.1e-02 nm, Epot= -1.98900e+06 Fmax= 1.52013e+04, atom= 851
Step=  251, Dmax= 2.5e-02 nm, Epot= -1.98901e+06 Fmax= 1.80356e+04, atom= 851
Step=  253, Dmax= 1.5e-02 nm, Epot= -1.98949e+06 Fmax= 1.96361e+03, atom= 851
Step=  254, Dmax= 1.8e-02 nm, Epot= -1.98963e+06 Fmax= 2.18989e+04, atom= 851
Step=  255, Dmax= 2.2e-02 nm, Epot= -1.99025e+06 Fmax= 6.81483e+03, atom= 851
Step=  257, Dmax= 1.3e-02 nm, Epot= -1.99033e+06 Fmax= 1.04497e+04, atom= 851
Step=  258, Dmax= 1.6e-02 nm, Epot= -1.99045e+06 Fmax= 1.01423e+04, atom= 851
Step=  259, Dmax= 1.9e-02 nm, Epot= -1.99045e+06 Fmax= 1.46817e+04, atom= 851
Step=  260, Dmax= 2.3e-02 nm, Epot= -1.99056e+06 Fmax= 1.49602e+04, atom= 851
Step=  262, Dmax= 1.4e-02 nm, Epot= -1.99090e+06 Fmax= 2.78033e+03, atom= 851
Step=  263, Dmax= 1.6e-02 nm, Epot= -1.99093e+06 Fmax= 1.85581e+04, atom= 851
Step=  264, Dmax= 2.0e-02 nm, Epot= -1.99139e+06 Fmax= 7.05764e+03, atom= 851
Step=  266, Dmax= 1.2e-02 nm, Epot= -1.99149e+06 Fmax= 8.31694e+03, atom= 851
Step=  267, Dmax= 1.4e-02 nm, Epot= -1.99158e+06 Fmax= 1.01873e+04, atom= 851
Step=  268, Dmax= 1.7e-02 nm, Epot= -1.99166e+06 Fmax= 1.19413e+04, atom= 851
Step=  269, Dmax= 2.0e-02 nm, Epot= -1.99169e+06 Fmax= 1.47218e+04, atom= 851
Step=  270, Dmax= 2.4e-02 nm, Epot= -1.99171e+06 Fmax= 1.71163e+04, atom= 851
Step=  272, Dmax= 1.5e-02 nm, Epot= -1.99216e+06 Fmax= 1.93355e+03, atom= 851
Step=  273, Dmax= 1.8e-02 nm, Epot= -1.99226e+06 Fmax= 2.10665e+04, atom= 851
Step=  274, Dmax= 2.1e-02 nm, Epot= -1.99286e+06 Fmax= 6.47430e+03, atom= 851
Step=  276, Dmax= 1.3e-02 nm, Epot= -1.99294e+06 Fmax= 1.00073e+04, atom= 851
Step=  277, Dmax= 1.5e-02 nm, Epot= -1.99306e+06 Fmax= 9.88140e+03, atom= 851
Step=  278, Dmax= 1.8e-02 nm, Epot= -1.99306e+06 Fmax= 1.38817e+04, atom= 851
Step=  279, Dmax= 2.2e-02 nm, Epot= -1.99315e+06 Fmax= 1.47675e+04, atom= 851
Step=  281, Dmax= 1.3e-02 nm, Epot= -1.99349e+06 Fmax= 2.46320e+03, atom= 851
Step=  282, Dmax= 1.6e-02 nm, Epot= -1.99355e+06 Fmax= 1.81671e+04, atom= 851
Step=  283, Dmax= 1.9e-02 nm, Epot= -1.99400e+06 Fmax= 6.59316e+03, atom= 851
Step=  285, Dmax= 1.1e-02 nm, Epot= -1.99409e+06 Fmax= 8.25721e+03, atom= 851
Step=  286, Dmax= 1.4e-02 nm, Epot= -1.99418e+06 Fmax= 9.50818e+03, atom= 851
Step=  287, Dmax= 1.6e-02 nm, Epot= -1.99425e+06 Fmax= 1.18820e+04, atom= 851
Step=  288, Dmax= 2.0e-02 nm, Epot= -1.99431e+06 Fmax= 1.36846e+04, atom= 851
Step=  290, Dmax= 1.2e-02 nm, Epot= -1.99461e+06 Fmax= 1.62121e+03, atom= 851
Step=  291, Dmax= 1.4e-02 nm, Epot= -1.99487e+06 Fmax= 1.68279e+04, atom= 851
Step=  292, Dmax= 1.7e-02 nm, Epot= -1.99528e+06 Fmax= 5.27944e+03, atom= 851
Step=  294, Dmax= 1.0e-02 nm, Epot= -1.99536e+06 Fmax= 7.96181e+03, atom= 851
Step=  295, Dmax= 1.2e-02 nm, Epot= -1.99547e+06 Fmax= 7.99629e+03, atom= 851
Step=  296, Dmax= 1.5e-02 nm, Epot= -1.99552e+06 Fmax= 1.10866e+04, atom= 851
Step=  297, Dmax= 1.8e-02 nm, Epot= -1.99562e+06 Fmax= 1.18997e+04, atom= 851
Step=  299, Dmax= 1.1e-02 nm, Epot= -1.99586e+06 Fmax= 1.91819e+03, atom= 851
Step=  300, Dmax= 1.3e-02 nm, Epot= -1.99606e+06 Fmax= 1.46335e+04, atom= 851
Step=  301, Dmax= 1.5e-02 nm, Epot= -1.99637e+06 Fmax= 5.22896e+03, atom= 851
Step=  303, Dmax= 9.1e-03 nm, Epot= -1.99647e+06 Fmax= 6.68830e+03, atom= 851
Step=  304, Dmax= 1.1e-02 nm, Epot= -1.99656e+06 Fmax= 7.57251e+03, atom= 851
Step=  305, Dmax= 1.3e-02 nm, Epot= -1.99664e+06 Fmax= 9.59056e+03, atom= 851
Step=  306, Dmax= 1.6e-02 nm, Epot= -1.99672e+06 Fmax= 1.09366e+04, atom= 851
Step=  307, Dmax= 1.9e-02 nm, Epot= -1.99675e+06 Fmax= 1.37911e+04, atom= 851
Step=  308, Dmax= 2.3e-02 nm, Epot= -1.99679e+06 Fmax= 1.57452e+04, atom= 851
Step=  310, Dmax= 1.4e-02 nm, Epot= -1.99716e+06 Fmax= 1.93160e+03, atom= 851
Step=  311, Dmax= 1.6e-02 nm, Epot= -1.99726e+06 Fmax= 1.93836e+04, atom= 851
Step=  312, Dmax= 2.0e-02 nm, Epot= -1.99777e+06 Fmax= 6.15832e+03, atom= 851
Step=  314, Dmax= 1.2e-02 nm, Epot= -1.99783e+06 Fmax= 9.13946e+03, atom= 851
Step=  315, Dmax= 1.4e-02 nm, Epot= -1.99794e+06 Fmax= 9.30422e+03, atom= 851
Step=  316, Dmax= 1.7e-02 nm, Epot= -1.99796e+06 Fmax= 1.27416e+04, atom= 851
Step=  317, Dmax= 2.0e-02 nm, Epot= -1.99804e+06 Fmax= 1.38266e+04, atom= 851
Step=  319, Dmax= 1.2e-02 nm, Epot= -1.99833e+06 Fmax= 2.15012e+03, atom= 851
Step=  320, Dmax= 1.5e-02 nm, Epot= -1.99843e+06 Fmax= 1.69755e+04, atom= 851
Step=  321, Dmax= 1.8e-02 nm, Epot= -1.99882e+06 Fmax= 5.98479e+03, atom= 851
Step=  323, Dmax= 1.1e-02 nm, Epot= -1.99891e+06 Fmax= 7.78996e+03, atom= 851
Step=  324, Dmax= 1.3e-02 nm, Epot= -1.99900e+06 Fmax= 8.68833e+03, atom= 851
Step=  325, Dmax= 1.5e-02 nm, Epot= -1.99905e+06 Fmax= 1.11484e+04, atom= 851
Step=  326, Dmax= 1.8e-02 nm, Epot= -1.99911e+06 Fmax= 1.25683e+04, atom= 851
Step=  328, Dmax= 1.1e-02 nm, Epot= -1.99937e+06 Fmax= 1.63271e+03, atom= 851
Step=  329, Dmax= 1.3e-02 nm, Epot= -1.99960e+06 Fmax= 1.54682e+04, atom= 851
Step=  330, Dmax= 1.6e-02 nm, Epot= -1.99994e+06 Fmax= 5.03412e+03, atom= 851
Step=  332, Dmax= 9.4e-03 nm, Epot= -2.00002e+06 Fmax= 7.25411e+03, atom= 851
Step=  333, Dmax= 1.1e-02 nm, Epot= -2.00012e+06 Fmax= 7.54428e+03, atom= 851
Step=  334, Dmax= 1.4e-02 nm, Epot= -2.00018e+06 Fmax= 1.01580e+04, atom= 851
Step=  335, Dmax= 1.6e-02 nm, Epot= -2.00025e+06 Fmax= 1.11586e+04, atom= 851
Step=  336, Dmax= 2.0e-02 nm, Epot= -2.00026e+06 Fmax= 1.43185e+04, atom= 851
Step=  337, Dmax= 2.3e-02 nm, Epot= -2.00029e+06 Fmax= 1.63974e+04, atom= 851
Step=  339, Dmax= 1.4e-02 nm, Epot= -2.00069e+06 Fmax= 2.08201e+03, atom= 851
Step=  340, Dmax= 1.7e-02 nm, Epot= -2.00072e+06 Fmax= 1.99978e+04, atom= 851
Step=  341, Dmax= 2.0e-02 nm, Epot= -2.00122e+06 Fmax= 6.54492e+03, atom= 851
Step=  343, Dmax= 1.2e-02 nm, Epot= -2.00128e+06 Fmax= 9.39354e+03, atom= 851
Step=  344, Dmax= 1.5e-02 nm, Epot= -2.00137e+06 Fmax= 9.64731e+03, atom= 851
Step=  345, Dmax= 1.8e-02 nm, Epot= -2.00139e+06 Fmax= 1.32895e+04, atom= 851
Step=  346, Dmax= 2.1e-02 nm, Epot= -2.00146e+06 Fmax= 1.41162e+04, atom= 851
Step=  348, Dmax= 1.3e-02 nm, Epot= -2.00176e+06 Fmax= 2.28727e+03, atom= 851
Step=  349, Dmax= 1.5e-02 nm, Epot= -2.00180e+06 Fmax= 1.74587e+04, atom= 851
Step=  350, Dmax= 1.8e-02 nm, Epot= -2.00220e+06 Fmax= 6.22579e+03, atom= 851
Step=  352, Dmax= 1.1e-02 nm, Epot= -2.00228e+06 Fmax= 7.98398e+03, atom= 851
Step=  353, Dmax= 1.3e-02 nm, Epot= -2.00236e+06 Fmax= 9.11870e+03, atom= 851
Step=  354, Dmax= 1.6e-02 nm, Epot= -2.00240e+06 Fmax= 1.13396e+04, atom= 851
Step=  355, Dmax= 1.9e-02 nm, Epot= -2.00245e+06 Fmax= 1.33014e+04, atom= 851
Step=  357, Dmax= 1.1e-02 nm, Epot= -2.00272e+06 Fmax= 1.51646e+03, atom= 851
Step=  358, Dmax= 1.4e-02 nm, Epot= -2.00296e+06 Fmax= 1.61870e+04, atom= 851
Step=  359, Dmax= 1.6e-02 nm, Epot= -2.00330e+06 Fmax= 5.10290e+03, atom= 851
Step=  361, Dmax= 9.8e-03 nm, Epot= -2.00338e+06 Fmax= 7.68721e+03, atom= 851
Step=  362, Dmax= 1.2e-02 nm, Epot= -2.00348e+06 Fmax= 7.59819e+03, atom= 851
Step=  363, Dmax= 1.4e-02 nm, Epot= -2.00351e+06 Fmax= 1.08036e+04, atom= 851
Step=  364, Dmax= 1.7e-02 nm, Epot= -2.00360e+06 Fmax= 1.12008e+04, atom= 851
Step=  366, Dmax= 1.0e-02 nm, Epot= -2.00380e+06 Fmax= 1.97675e+03, atom= 851
Step=  367, Dmax= 1.2e-02 nm, Epot= -2.00394e+06 Fmax= 1.38672e+04, atom= 851
Step=  368, Dmax= 1.5e-02 nm, Epot= -2.00421e+06 Fmax= 5.14699e+03, atom= 851
Step=  370, Dmax= 8.7e-03 nm, Epot= -2.00429e+06 Fmax= 6.26326e+03, atom= 851
Step=  371, Dmax= 1.0e-02 nm, Epot= -2.00438e+06 Fmax= 7.46064e+03, atom= 851
Step=  372, Dmax= 1.3e-02 nm, Epot= -2.00444e+06 Fmax= 8.96585e+03, atom= 851
Step=  373, Dmax= 1.5e-02 nm, Epot= -2.00450e+06 Fmax= 1.08056e+04, atom= 851
Step=  374, Dmax= 1.8e-02 nm, Epot= -2.00454e+06 Fmax= 1.28339e+04, atom= 851
Step=  375, Dmax= 2.2e-02 nm, Epot= -2.00455e+06 Fmax= 1.56554e+04, atom= 851
Step=  377, Dmax= 1.3e-02 nm, Epot= -2.00489e+06 Fmax= 1.48175e+03, atom= 851
Step=  378, Dmax= 1.6e-02 nm, Epot= -2.00510e+06 Fmax= 1.89503e+04, atom= 851
Step=  379, Dmax= 1.9e-02 nm, Epot= -2.00554e+06 Fmax= 5.65814e+03, atom= 851
Step=  381, Dmax= 1.1e-02 nm, Epot= -2.00559e+06 Fmax= 9.14633e+03, atom= 851
Step=  382, Dmax= 1.4e-02 nm, Epot= -2.00569e+06 Fmax= 8.51579e+03, atom= 851
Step=  383, Dmax= 1.6e-02 nm, Epot= -2.00570e+06 Fmax= 1.27618e+04, atom= 851
Step=  384, Dmax= 1.9e-02 nm, Epot= -2.00578e+06 Fmax= 1.26650e+04, atom= 851
Step=  386, Dmax= 1.2e-02 nm, Epot= -2.00602e+06 Fmax= 2.55793e+03, atom= 851
Step=  387, Dmax= 1.4e-02 nm, Epot= -2.00605e+06 Fmax= 1.57415e+04, atom= 851
Step=  388, Dmax= 1.7e-02 nm, Epot= -2.00636e+06 Fmax= 6.22665e+03, atom= 851
Step=  390, Dmax= 1.0e-02 nm, Epot= -2.00644e+06 Fmax= 6.96314e+03, atom= 851
Step=  391, Dmax= 1.2e-02 nm, Epot= -2.00651e+06 Fmax= 8.89857e+03, atom= 851
Step=  392, Dmax= 1.5e-02 nm, Epot= -2.00658e+06 Fmax= 1.00842e+04, atom= 851
Step=  393, Dmax= 1.7e-02 nm, Epot= -2.00661e+06 Fmax= 1.27713e+04, atom= 851
Step=  394, Dmax= 2.1e-02 nm, Epot= -2.00664e+06 Fmax= 1.45429e+04, atom= 851
Step=  396, Dmax= 1.3e-02 nm, Epot= -2.00693e+06 Fmax= 1.80557e+03, atom= 851
Step=  397, Dmax= 1.5e-02 nm, Epot= -2.00702e+06 Fmax= 1.79053e+04, atom= 851
Step=  398, Dmax= 1.8e-02 nm, Epot= -2.00743e+06 Fmax= 5.71031e+03, atom= 851
Step=  400, Dmax= 1.1e-02 nm, Epot= -2.00749e+06 Fmax= 8.43815e+03, atom= 851
Step=  401, Dmax= 1.3e-02 nm, Epot= -2.00757e+06 Fmax= 8.61093e+03, atom= 851
Step=  402, Dmax= 1.6e-02 nm, Epot= -2.00759e+06 Fmax= 1.17766e+04, atom= 851
Step=  403, Dmax= 1.9e-02 nm, Epot= -2.00766e+06 Fmax= 1.27825e+04, atom= 851
Step=  405, Dmax= 1.1e-02 nm, Epot= -2.00790e+06 Fmax= 1.98448e+03, atom= 851
Step=  406, Dmax= 1.4e-02 nm, Epot= -2.00800e+06 Fmax= 1.56921e+04, atom= 851
Step=  407, Dmax= 1.6e-02 nm, Epot= -2.00830e+06 Fmax= 5.53188e+03, atom= 851
Step=  409, Dmax= 9.7e-03 nm, Epot= -2.00838e+06 Fmax= 7.20102e+03, atom= 851
Step=  410, Dmax= 1.2e-02 nm, Epot= -2.00845e+06 Fmax= 8.03600e+03, atom= 851
Step=  411, Dmax= 1.4e-02 nm, Epot= -2.00849e+06 Fmax= 1.03004e+04, atom= 851
Step=  412, Dmax= 1.7e-02 nm, Epot= -2.00855e+06 Fmax= 1.16300e+04, atom= 851
Step=  413, Dmax= 2.0e-02 nm, Epot= -2.00855e+06 Fmax= 1.47903e+04, atom= 851
Step=  414, Dmax= 2.4e-02 nm, Epot= -2.00856e+06 Fmax= 1.67627e+04, atom= 851
Step=  416, Dmax= 1.5e-02 nm, Epot= -2.00894e+06 Fmax= 2.11554e+03, atom= 851
Step=  418, Dmax= 8.7e-03 nm, Epot= -2.00907e+06 Fmax= 9.32663e+03, atom= 851
Step=  419, Dmax= 1.0e-02 nm, Epot= -2.00921e+06 Fmax= 4.33419e+03, atom= 851
Step=  420, Dmax= 1.3e-02 nm, Epot= -2.00921e+06 Fmax= 1.19969e+04, atom= 851
Step=  421, Dmax= 1.5e-02 nm, Epot= -2.00938e+06 Fmax= 7.67125e+03, atom= 851
Step=  423, Dmax= 9.0e-03 nm, Epot= -2.00950e+06 Fmax= 4.15082e+03, atom= 851
Step=  424, Dmax= 1.1e-02 nm, Epot= -2.00954e+06 Fmax= 1.00421e+04, atom= 851
Step=  425, Dmax= 1.3e-02 nm, Epot= -2.00967e+06 Fmax= 6.96299e+03, atom= 851
Step=  427, Dmax= 7.8e-03 nm, Epot= -2.00978e+06 Fmax= 3.22303e+03, atom= 851
Step=  428, Dmax= 9.4e-03 nm, Epot= -2.00985e+06 Fmax= 8.99960e+03, atom= 851
Step=  429, Dmax= 1.1e-02 nm, Epot= -2.00997e+06 Fmax= 5.68476e+03, atom= 851
Step=  431, Dmax= 6.7e-03 nm, Epot= -2.01006e+06 Fmax= 3.13775e+03, atom= 851
Step=  432, Dmax= 8.1e-03 nm, Epot= -2.01014e+06 Fmax= 7.45334e+03, atom= 851
Step=  433, Dmax= 9.7e-03 nm, Epot= -2.01025e+06 Fmax= 5.24056e+03, atom= 851
Step=  434, Dmax= 1.2e-02 nm, Epot= -2.01028e+06 Fmax= 1.00265e+04, atom= 851
Step=  435, Dmax= 1.4e-02 nm, Epot= -2.01039e+06 Fmax= 8.24365e+03, atom= 851
Step=  437, Dmax= 8.4e-03 nm, Epot= -2.01051e+06 Fmax= 2.70058e+03, atom= 851
Step=  438, Dmax= 1.0e-02 nm, Epot= -2.01059e+06 Fmax= 1.04350e+04, atom= 851
Step=  439, Dmax= 1.2e-02 nm, Epot= -2.01075e+06 Fmax= 5.34547e+03, atom= 851
Step=  441, Dmax= 7.2e-03 nm, Epot= -2.01083e+06 Fmax= 4.13299e+03, atom= 851
Step=  442, Dmax= 8.7e-03 nm, Epot= -2.01090e+06 Fmax= 7.25258e+03, atom= 851
Step=  443, Dmax= 1.0e-02 nm, Epot= -2.01100e+06 Fmax= 6.38658e+03, atom= 851
Step=  444, Dmax= 1.3e-02 nm, Epot= -2.01103e+06 Fmax= 1.00207e+04, atom= 851
Step=  445, Dmax= 1.5e-02 nm, Epot= -2.01111e+06 Fmax= 9.60819e+03, atom= 851
Step=  447, Dmax= 9.0e-03 nm, Epot= -2.01127e+06 Fmax= 2.14969e+03, atom= 851
Step=  448, Dmax= 1.1e-02 nm, Epot= -2.01137e+06 Fmax= 1.19724e+04, atom= 851
Step=  449, Dmax= 1.3e-02 nm, Epot= -2.01156e+06 Fmax= 4.98623e+03, atom= 851
Step=  451, Dmax= 7.8e-03 nm, Epot= -2.01164e+06 Fmax= 5.19454e+03, atom= 851
Step=  452, Dmax= 9.4e-03 nm, Epot= -2.01171e+06 Fmax= 7.04359e+03, atom= 851
Step=  453, Dmax= 1.1e-02 nm, Epot= -2.01177e+06 Fmax= 7.60945e+03, atom= 851
Step=  454, Dmax= 1.3e-02 nm, Epot= -2.01182e+06 Fmax= 1.00223e+04, atom= 851
Step=  455, Dmax= 1.6e-02 nm, Epot= -2.01187e+06 Fmax= 1.10666e+04, atom= 851
Step=  457, Dmax= 9.7e-03 nm, Epot= -2.01206e+06 Fmax= 1.56427e+03, atom= 851
Step=  458, Dmax= 1.2e-02 nm, Epot= -2.01222e+06 Fmax= 1.36304e+04, atom= 851
Step=  459, Dmax= 1.4e-02 nm, Epot= -2.01247e+06 Fmax= 4.59812e+03, atom= 851
Step=  461, Dmax= 8.4e-03 nm, Epot= -2.01254e+06 Fmax= 6.33045e+03, atom= 851
Step=  462, Dmax= 1.0e-02 nm, Epot= -2.01262e+06 Fmax= 6.82396e+03, atom= 851
Step=  463, Dmax= 1.2e-02 nm, Epot= -2.01266e+06 Fmax= 8.91725e+03, atom= 851
Step=  464, Dmax= 1.4e-02 nm, Epot= -2.01272e+06 Fmax= 1.00308e+04, atom= 851
Step=  465, Dmax= 1.7e-02 nm, Epot= -2.01273e+06 Fmax= 1.26245e+04, atom= 851
Step=  466, Dmax= 2.1e-02 nm, Epot= -2.01276e+06 Fmax= 1.46768e+04, atom= 851
Step=  468, Dmax= 1.3e-02 nm, Epot= -2.01305e+06 Fmax= 1.74235e+03, atom= 851
Step=  469, Dmax= 1.5e-02 nm, Epot= -2.01312e+06 Fmax= 1.78807e+04, atom= 851
Step=  470, Dmax= 1.8e-02 nm, Epot= -2.01349e+06 Fmax= 5.70609e+03, atom= 851
Step=  472, Dmax= 1.1e-02 nm, Epot= -2.01354e+06 Fmax= 8.46397e+03, atom= 851
Step=  473, Dmax= 1.3e-02 nm, Epot= -2.01362e+06 Fmax= 8.46478e+03, atom= 851
Step=  474, Dmax= 1.6e-02 nm, Epot= -2.01363e+06 Fmax= 1.19226e+04, atom= 851
Step=  475, Dmax= 1.9e-02 nm, Epot= -2.01369e+06 Fmax= 1.24461e+04, atom= 851
Step=  477, Dmax= 1.1e-02 nm, Epot= -2.01390e+06 Fmax= 2.14530e+03, atom= 851
Step=  478, Dmax= 1.3e-02 nm, Epot= -2.01395e+06 Fmax= 1.54024e+04, atom= 851
Step=  479, Dmax= 1.6e-02 nm, Epot= -2.01423e+06 Fmax= 5.65636e+03, atom= 851
Step=  481, Dmax= 9.7e-03 nm, Epot= -2.01430e+06 Fmax= 6.97959e+03, atom= 851
Step=  482, Dmax= 1.2e-02 nm, Epot= -2.01436e+06 Fmax= 8.22361e+03, atom= 851
Step=  483, Dmax= 1.4e-02 nm, Epot= -2.01441e+06 Fmax= 9.96756e+03, atom= 851
Step=  484, Dmax= 1.7e-02 nm, Epot= -2.01444e+06 Fmax= 1.19356e+04, atom= 851
Step=  485, Dmax= 2.0e-02 nm, Epot= -2.01445e+06 Fmax= 1.42423e+04, atom= 851
Step=  487, Dmax= 1.2e-02 nm, Epot= -2.01472e+06 Fmax= 1.42918e+03, atom= 851
Step=  488, Dmax= 1.4e-02 nm, Epot= -2.01485e+06 Fmax= 1.74832e+04, atom= 851
Step=  489, Dmax= 1.7e-02 nm, Epot= -2.01522e+06 Fmax= 5.16153e+03, atom= 851
Step=  491, Dmax= 1.0e-02 nm, Epot= -2.01527e+06 Fmax= 8.38496e+03, atom= 851
Step=  492, Dmax= 1.2e-02 nm, Epot= -2.01535e+06 Fmax= 7.95671e+03, atom= 851
Step=  493, Dmax= 1.5e-02 nm, Epot= -2.01536e+06 Fmax= 1.15807e+04, atom= 851
Step=  494, Dmax= 1.8e-02 nm, Epot= -2.01543e+06 Fmax= 1.19565e+04, atom= 851
Step=  496, Dmax= 1.1e-02 nm, Epot= -2.01562e+06 Fmax= 2.19246e+03, atom= 851
Step=  497, Dmax= 1.3e-02 nm, Epot= -2.01567e+06 Fmax= 1.47647e+04, atom= 851
Step=  498, Dmax= 1.6e-02 nm, Epot= -2.01593e+06 Fmax= 5.57571e+03, atom= 851
Step=  500, Dmax= 9.3e-03 nm, Epot= -2.01599e+06 Fmax= 6.62281e+03, atom= 851
Step=  501, Dmax= 1.1e-02 nm, Epot= -2.01604e+06 Fmax= 7.98056e+03, atom= 851
Step=  502, Dmax= 1.3e-02 nm, Epot= -2.01609e+06 Fmax= 9.59203e+03, atom= 851
Step=  503, Dmax= 1.6e-02 nm, Epot= -2.01613e+06 Fmax= 1.14257e+04, atom= 851
Step=  504, Dmax= 1.9e-02 nm, Epot= -2.01614e+06 Fmax= 1.38937e+04, atom= 851
Step=  506, Dmax= 1.2e-02 nm, Epot= -2.01639e+06 Fmax= 1.33108e+03, atom= 851
Step=  507, Dmax= 1.4e-02 nm, Epot= -2.01657e+06 Fmax= 1.68421e+04, atom= 851
Step=  508, Dmax= 1.7e-02 nm, Epot= -2.01690e+06 Fmax= 5.02643e+03, atom= 851
Step=  510, Dmax= 1.0e-02 nm, Epot= -2.01695e+06 Fmax= 8.12799e+03, atom= 851
Step=  511, Dmax= 1.2e-02 nm, Epot= -2.01703e+06 Fmax= 7.57331e+03, atom= 851
Step=  512, Dmax= 1.4e-02 nm, Epot= -2.01703e+06 Fmax= 1.13369e+04, atom= 851
Step=  513, Dmax= 1.7e-02 nm, Epot= -2.01710e+06 Fmax= 1.12684e+04, atom= 851
Step=  515, Dmax= 1.0e-02 nm, Epot= -2.01728e+06 Fmax= 2.27034e+03, atom= 851
Step=  516, Dmax= 1.2e-02 nm, Epot= -2.01732e+06 Fmax= 1.39955e+04, atom= 851
Step=  517, Dmax= 1.5e-02 nm, Epot= -2.01755e+06 Fmax= 5.53782e+03, atom= 851
Step=  519, Dmax= 9.0e-03 nm, Epot= -2.01761e+06 Fmax= 6.18668e+03, atom= 851
Step=  520, Dmax= 1.1e-02 nm, Epot= -2.01767e+06 Fmax= 7.91369e+03, atom= 851
Step=  521, Dmax= 1.3e-02 nm, Epot= -2.01772e+06 Fmax= 8.96161e+03, atom= 851
Step=  522, Dmax= 1.6e-02 nm, Epot= -2.01775e+06 Fmax= 1.13537e+04, atom= 851
Step=  523, Dmax= 1.9e-02 nm, Epot= -2.01778e+06 Fmax= 1.29314e+04, atom= 851
Step=  525, Dmax= 1.1e-02 nm, Epot= -2.01799e+06 Fmax= 1.61031e+03, atom= 851
Step=  526, Dmax= 1.3e-02 nm, Epot= -2.01809e+06 Fmax= 1.59018e+04, atom= 851
Step=  527, Dmax= 1.6e-02 nm, Epot= -2.01839e+06 Fmax= 5.09616e+03, atom= 851
Step=  529, Dmax= 9.6e-03 nm, Epot= -2.01844e+06 Fmax= 7.48337e+03, atom= 851
Step=  530, Dmax= 1.2e-02 nm, Epot= -2.01850e+06 Fmax= 7.67238e+03, atom= 851
Step=  531, Dmax= 1.4e-02 nm, Epot= -2.01853e+06 Fmax= 1.04536e+04, atom= 851
Step=  532, Dmax= 1.7e-02 nm, Epot= -2.01858e+06 Fmax= 1.13775e+04, atom= 851
Step=  534, Dmax= 1.0e-02 nm, Epot= -2.01876e+06 Fmax= 1.74313e+03, atom= 851
Step=  535, Dmax= 1.2e-02 nm, Epot= -2.01886e+06 Fmax= 1.39767e+04, atom= 851
Step=  536, Dmax= 1.4e-02 nm, Epot= -2.01908e+06 Fmax= 4.88489e+03, atom= 851
Step=  538, Dmax= 8.6e-03 nm, Epot= -2.01914e+06 Fmax= 6.43510e+03, atom= 851
Step=  539, Dmax= 1.0e-02 nm, Epot= -2.01920e+06 Fmax= 7.10932e+03, atom= 851
Step=  540, Dmax= 1.2e-02 nm, Epot= -2.01924e+06 Fmax= 9.19108e+03, atom= 851
Step=  541, Dmax= 1.5e-02 nm, Epot= -2.01929e+06 Fmax= 1.03058e+04, atom= 851
Step=  542, Dmax= 1.8e-02 nm, Epot= -2.01929e+06 Fmax= 1.31781e+04, atom= 851
Step=  543, Dmax= 2.2e-02 nm, Epot= -2.01931e+06 Fmax= 1.48772e+04, atom= 851
Step=  545, Dmax= 1.3e-02 nm, Epot= -2.01958e+06 Fmax= 1.91729e+03, atom= 851
Step=  547, Dmax= 7.7e-03 nm, Epot= -2.01968e+06 Fmax= 8.24196e+03, atom= 851
Step=  548, Dmax= 9.3e-03 nm, Epot= -2.01979e+06 Fmax= 3.90412e+03, atom= 851
Step=  549, Dmax= 1.1e-02 nm, Epot= -2.01981e+06 Fmax= 1.06169e+04, atom= 851
Step=  550, Dmax= 1.3e-02 nm, Epot= -2.01993e+06 Fmax= 6.87110e+03, atom= 851
Step=  552, Dmax= 8.0e-03 nm, Epot= -2.02002e+06 Fmax= 3.63529e+03, atom= 851
Step=  553, Dmax= 9.6e-03 nm, Epot= -2.02006e+06 Fmax= 8.98336e+03, atom= 851
Step=  554, Dmax= 1.2e-02 nm, Epot= -2.02016e+06 Fmax= 6.13122e+03, atom= 851
Step=  556, Dmax= 6.9e-03 nm, Epot= -2.02024e+06 Fmax= 2.92755e+03, atom= 851
Step=  557, Dmax= 8.3e-03 nm, Epot= -2.02030e+06 Fmax= 7.93519e+03, atom= 851
Step=  558, Dmax= 1.0e-02 nm, Epot= -2.02040e+06 Fmax= 5.12218e+03, atom= 851
Step=  559, Dmax= 1.2e-02 nm, Epot= -2.02040e+06 Fmax= 1.05042e+04, atom= 851
Step=  560, Dmax= 1.4e-02 nm, Epot= -2.02051e+06 Fmax= 8.30702e+03, atom= 851
Step=  562, Dmax= 8.6e-03 nm, Epot= -2.02062e+06 Fmax= 2.99467e+03, atom= 851
Step=  563, Dmax= 1.0e-02 nm, Epot= -2.02066e+06 Fmax= 1.05762e+04, atom= 851
Step=  564, Dmax= 1.2e-02 nm, Epot= -2.02079e+06 Fmax= 5.68071e+03, atom= 851
Step=  566, Dmax= 7.5e-03 nm, Epot= -2.02086e+06 Fmax= 4.06417e+03, atom= 851
Step=  567, Dmax= 8.9e-03 nm, Epot= -2.02091e+06 Fmax= 7.61464e+03, atom= 851
Step=  568, Dmax= 1.1e-02 nm, Epot= -2.02098e+06 Fmax= 6.42984e+03, atom= 851
Step=  569, Dmax= 1.3e-02 nm, Epot= -2.02100e+06 Fmax= 1.03754e+04, atom= 851
Step=  570, Dmax= 1.5e-02 nm, Epot= -2.02108e+06 Fmax= 9.85839e+03, atom= 851
Step=  572, Dmax= 9.3e-03 nm, Epot= -2.02121e+06 Fmax= 2.29979e+03, atom= 851
Step=  573, Dmax= 1.1e-02 nm, Epot= -2.02125e+06 Fmax= 1.22894e+04, atom= 851
Step=  574, Dmax= 1.3e-02 nm, Epot= -2.02143e+06 Fmax= 5.19525e+03, atom= 851
Step=  576, Dmax= 8.0e-03 nm, Epot= -2.02149e+06 Fmax= 5.29021e+03, atom= 851
Step=  577, Dmax= 9.6e-03 nm, Epot= -2.02154e+06 Fmax= 7.26668e+03, atom= 851
Step=  578, Dmax= 1.2e-02 nm, Epot= -2.02160e+06 Fmax= 7.84123e+03, atom= 851
Step=  579, Dmax= 1.4e-02 nm, Epot= -2.02163e+06 Fmax= 1.02320e+04, atom= 851
Step=  580, Dmax= 1.7e-02 nm, Epot= -2.02167e+06 Fmax= 1.15340e+04, atom= 851
Step=  582, Dmax= 1.0e-02 nm, Epot= -2.02184e+06 Fmax= 1.54676e+03, atom= 851
Step=  583, Dmax= 1.2e-02 nm, Epot= -2.02196e+06 Fmax= 1.41221e+04, atom= 851
Step=  584, Dmax= 1.4e-02 nm, Epot= -2.02217e+06 Fmax= 4.67996e+03, atom= 851
Step=  586, Dmax= 8.6e-03 nm, Epot= -2.02222e+06 Fmax= 6.61238e+03, atom= 851
Step=  587, Dmax= 1.0e-02 nm, Epot= -2.02229e+06 Fmax= 6.88929e+03, atom= 851
Step=  588, Dmax= 1.2e-02 nm, Epot= -2.02232e+06 Fmax= 9.36522e+03, atom= 851
Step=  589, Dmax= 1.5e-02 nm, Epot= -2.02237e+06 Fmax= 1.00724e+04, atom= 851
Step=  590, Dmax= 1.8e-02 nm, Epot= -2.02237e+06 Fmax= 1.33438e+04, atom= 851
Step=  591, Dmax= 2.1e-02 nm, Epot= -2.02239e+06 Fmax= 1.46271e+04, atom= 851
Step=  593, Dmax= 1.3e-02 nm, Epot= -2.02264e+06 Fmax= 2.11898e+03, atom= 851
Step=  595, Dmax= 7.7e-03 nm, Epot= -2.02272e+06 Fmax= 8.00076e+03, atom= 851
Step=  596, Dmax= 9.3e-03 nm, Epot= -2.02282e+06 Fmax= 4.10808e+03, atom= 851
Step=  597, Dmax= 1.1e-02 nm, Epot= -2.02284e+06 Fmax= 1.03722e+04, atom= 851
Step=  598, Dmax= 1.3e-02 nm, Epot= -2.02294e+06 Fmax= 7.06521e+03, atom= 851
Step=  600, Dmax= 8.0e-03 nm, Epot= -2.02303e+06 Fmax= 3.40930e+03, atom= 851
Step=  601, Dmax= 9.6e-03 nm, Epot= -2.02307e+06 Fmax= 9.17343e+03, atom= 851
Step=  602, Dmax= 1.2e-02 nm, Epot= -2.02316e+06 Fmax= 5.89534e+03, atom= 851
Step=  604, Dmax= 6.9e-03 nm, Epot= -2.02323e+06 Fmax= 3.13809e+03, atom= 851
Step=  605, Dmax= 8.3e-03 nm, Epot= -2.02329e+06 Fmax= 7.68980e+03, atom= 851
Step=  606, Dmax= 1.0e-02 nm, Epot= -2.02337e+06 Fmax= 5.32945e+03, atom= 851
Step=  607, Dmax= 1.2e-02 nm, Epot= -2.02339e+06 Fmax= 1.02494e+04, atom= 851
Step=  608, Dmax= 1.4e-02 nm, Epot= -2.02348e+06 Fmax= 8.50722e+03, atom= 851
Step=  610, Dmax= 8.6e-03 nm, Epot= -2.02358e+06 Fmax= 2.76038e+03, atom= 851
Step=  611, Dmax= 1.0e-02 nm, Epot= -2.02362e+06 Fmax= 1.07712e+04, atom= 851
Step=  612, Dmax= 1.2e-02 nm, Epot= -2.02375e+06 Fmax= 5.43599e+03, atom= 851
Step=  614, Dmax= 7.4e-03 nm, Epot= -2.02381e+06 Fmax= 4.28145e+03, atom= 851
Step=  615, Dmax= 8.9e-03 nm, Epot= -2.02386e+06 Fmax= 7.36033e+03, atom= 851
Step=  616, Dmax= 1.1e-02 nm, Epot= -2.02392e+06 Fmax= 6.64354e+03, atom= 851
Step=  617, Dmax= 1.3e-02 nm, Epot= -2.02394e+06 Fmax= 1.01111e+04, atom= 851
Step=  618, Dmax= 1.5e-02 nm, Epot= -2.02400e+06 Fmax= 1.00646e+04, atom= 851
Step=  620, Dmax= 9.2e-03 nm, Epot= -2.02413e+06 Fmax= 2.05727e+03, atom= 851
Step=  621, Dmax= 1.1e-02 nm, Epot= -2.02420e+06 Fmax= 1.24883e+04, atom= 851
Step=  622, Dmax= 1.3e-02 nm, Epot= -2.02437e+06 Fmax= 4.94254e+03, atom= 851
Step=  624, Dmax= 8.0e-03 nm, Epot= -2.02442e+06 Fmax= 5.51502e+03, atom= 851
Step=  625, Dmax= 9.6e-03 nm, Epot= -2.02447e+06 Fmax= 7.00316e+03, atom= 851
Step=  626, Dmax= 1.2e-02 nm, Epot= -2.02451e+06 Fmax= 8.06192e+03, atom= 851
Step=  627, Dmax= 1.4e-02 nm, Epot= -2.02455e+06 Fmax= 9.95695e+03, atom= 851
Step=  628, Dmax= 1.7e-02 nm, Epot= -2.02457e+06 Fmax= 1.17465e+04, atom= 851
Step=  629, Dmax= 2.0e-02 nm, Epot= -2.02458e+06 Fmax= 1.41850e+04, atom= 851
Step=  631, Dmax= 1.2e-02 nm, Epot= -2.02480e+06 Fmax= 1.34424e+03, atom= 851
Step=  632, Dmax= 1.4e-02 nm, Epot= -2.02491e+06 Fmax= 1.73797e+04, atom= 851
Step=  633, Dmax= 1.7e-02 nm, Epot= -2.02522e+06 Fmax= 5.06231e+03, atom= 851
Step=  635, Dmax= 1.0e-02 nm, Epot= -2.02525e+06 Fmax= 8.35020e+03, atom= 851
Step=  636, Dmax= 1.2e-02 nm, Epot= -2.02532e+06 Fmax= 7.84418e+03, atom= 851
Step=  638, Dmax= 7.4e-03 nm, Epot= -2.02540e+06 Fmax= 1.87385e+03, atom= 851
Step=  639, Dmax= 8.9e-03 nm, Epot= -2.02550e+06 Fmax= 9.80984e+03, atom= 851
Step=  640, Dmax= 1.1e-02 nm, Epot= -2.02561e+06 Fmax= 4.17342e+03, atom= 851
Step=  642, Dmax= 6.4e-03 nm, Epot= -2.02567e+06 Fmax= 4.21661e+03, atom= 851
Step=  643, Dmax= 7.7e-03 nm, Epot= -2.02572e+06 Fmax= 5.82925e+03, atom= 851
Step=  644, Dmax= 9.2e-03 nm, Epot= -2.02577e+06 Fmax= 6.25745e+03, atom= 851
Step=  645, Dmax= 1.1e-02 nm, Epot= -2.02581e+06 Fmax= 8.20369e+03, atom= 851
Step=  646, Dmax= 1.3e-02 nm, Epot= -2.02585e+06 Fmax= 9.20758e+03, atom= 851
Step=  647, Dmax= 1.6e-02 nm, Epot= -2.02587e+06 Fmax= 1.16078e+04, atom= 851
Step=  648, Dmax= 1.9e-02 nm, Epot= -2.02589e+06 Fmax= 1.34776e+04, atom= 851
Step=  650, Dmax= 1.1e-02 nm, Epot= -2.02609e+06 Fmax= 1.60014e+03, atom= 851
Step=  651, Dmax= 1.4e-02 nm, Epot= -2.02616e+06 Fmax= 1.64504e+04, atom= 851
Step=  652, Dmax= 1.7e-02 nm, Epot= -2.02642e+06 Fmax= 5.21378e+03, atom= 851
Step=  654, Dmax= 9.9e-03 nm, Epot= -2.02646e+06 Fmax= 7.80827e+03, atom= 851
Step=  655, Dmax= 1.2e-02 nm, Epot= -2.02651e+06 Fmax= 7.74315e+03, atom= 851
Step=  656, Dmax= 1.4e-02 nm, Epot= -2.02653e+06 Fmax= 1.09914e+04, atom= 851
Step=  657, Dmax= 1.7e-02 nm, Epot= -2.02657e+06 Fmax= 1.13972e+04, atom= 851
Step=  659, Dmax= 1.0e-02 nm, Epot= -2.02672e+06 Fmax= 2.01661e+03, atom= 851
Step=  660, Dmax= 1.2e-02 nm, Epot= -2.02676e+06 Fmax= 1.40911e+04, atom= 851
Step=  661, Dmax= 1.5e-02 nm, Epot= -2.02696e+06 Fmax= 5.26418e+03, atom= 851
Step=  663, Dmax= 8.9e-03 nm, Epot= -2.02701e+06 Fmax= 6.34348e+03, atom= 851
Step=  664, Dmax= 1.1e-02 nm, Epot= -2.02705e+06 Fmax= 7.62890e+03, atom= 851
Step=  665, Dmax= 1.3e-02 nm, Epot= -2.02709e+06 Fmax= 9.08333e+03, atom= 851
Step=  666, Dmax= 1.5e-02 nm, Epot= -2.02712e+06 Fmax= 1.10449e+04, atom= 851
Step=  667, Dmax= 1.8e-02 nm, Epot= -2.02713e+06 Fmax= 1.30083e+04, atom= 851
Step=  669, Dmax= 1.1e-02 nm, Epot= -2.02732e+06 Fmax= 1.39987e+03, atom= 851
Step=  670, Dmax= 1.3e-02 nm, Epot= -2.02741e+06 Fmax= 1.59436e+04, atom= 851
Step=  671, Dmax= 1.6e-02 nm, Epot= -2.02766e+06 Fmax= 4.86722e+03, atom= 851
Step=  673, Dmax= 9.6e-03 nm, Epot= -2.02770e+06 Fmax= 7.58250e+03, atom= 851
Step=  674, Dmax= 1.1e-02 nm, Epot= -2.02776e+06 Fmax= 7.43647e+03, atom= 851
Step=  675, Dmax= 1.4e-02 nm, Epot= -2.02776e+06 Fmax= 1.05144e+04, atom= 851
Step=  676, Dmax= 1.7e-02 nm, Epot= -2.02782e+06 Fmax= 1.11161e+04, atom= 851
Step=  678, Dmax= 9.9e-03 nm, Epot= -2.02796e+06 Fmax= 1.87855e+03, atom= 851
Step=  679, Dmax= 1.2e-02 nm, Epot= -2.02801e+06 Fmax= 1.37137e+04, atom= 851
Step=  680, Dmax= 1.4e-02 nm, Epot= -2.02819e+06 Fmax= 4.96899e+03, atom= 851
Step=  682, Dmax= 8.6e-03 nm, Epot= -2.02824e+06 Fmax= 6.24617e+03, atom= 851
Step=  683, Dmax= 1.0e-02 nm, Epot= -2.02829e+06 Fmax= 7.16831e+03, atom= 851
Step=  684, Dmax= 1.2e-02 nm, Epot= -2.02832e+06 Fmax= 8.98296e+03, atom= 851
Step=  685, Dmax= 1.5e-02 nm, Epot= -2.02836e+06 Fmax= 1.03275e+04, atom= 851
Step=  686, Dmax= 1.8e-02 nm, Epot= -2.02837e+06 Fmax= 1.29408e+04, atom= 851
Step=  687, Dmax= 2.1e-02 nm, Epot= -2.02837e+06 Fmax= 1.48487e+04, atom= 851
Step=  689, Dmax= 1.3e-02 nm, Epot= -2.02859e+06 Fmax= 1.79207e+03, atom= 851
Step=  691, Dmax= 7.7e-03 nm, Epot= -2.02868e+06 Fmax= 8.26766e+03, atom= 851
Step=  692, Dmax= 9.2e-03 nm, Epot= -2.02877e+06 Fmax= 3.76957e+03, atom= 851
Step=  693, Dmax= 1.1e-02 nm, Epot= -2.02878e+06 Fmax= 1.06072e+04, atom= 851
Step=  694, Dmax= 1.3e-02 nm, Epot= -2.02888e+06 Fmax= 6.72085e+03, atom= 851
Step=  696, Dmax= 7.9e-03 nm, Epot= -2.02895e+06 Fmax= 3.68481e+03, atom= 851
Step=  697, Dmax= 9.5e-03 nm, Epot= -2.02899e+06 Fmax= 8.82198e+03, atom= 851
Step=  698, Dmax= 1.1e-02 nm, Epot= -2.02907e+06 Fmax= 6.14837e+03, atom= 851
Step=  700, Dmax= 6.9e-03 nm, Epot= -2.02913e+06 Fmax= 2.82867e+03, atom= 851
Step=  701, Dmax= 8.2e-03 nm, Epot= -2.02918e+06 Fmax= 7.92686e+03, atom= 851
Step=  702, Dmax= 9.9e-03 nm, Epot= -2.02925e+06 Fmax= 5.01190e+03, atom= 851
Step=  703, Dmax= 1.2e-02 nm, Epot= -2.02926e+06 Fmax= 1.04633e+04, atom= 851
Step=  704, Dmax= 1.4e-02 nm, Epot= -2.02934e+06 Fmax= 8.17571e+03, atom= 851
Step=  706, Dmax= 8.5e-03 nm, Epot= -2.02942e+06 Fmax= 3.01812e+03, atom= 851
Step=  707, Dmax= 1.0e-02 nm, Epot= -2.02945e+06 Fmax= 1.04339e+04, atom= 851
Step=  708, Dmax= 1.2e-02 nm, Epot= -2.02956e+06 Fmax= 5.66835e+03, atom= 851
Step=  710, Dmax= 7.4e-03 nm, Epot= -2.02962e+06 Fmax= 3.98863e+03, atom= 851
Step=  711, Dmax= 8.9e-03 nm, Epot= -2.02966e+06 Fmax= 7.57701e+03, atom= 851
Step=  712, Dmax= 1.1e-02 nm, Epot= -2.02973e+06 Fmax= 6.33982e+03, atom= 851
Step=  713, Dmax= 1.3e-02 nm, Epot= -2.02973e+06 Fmax= 1.03050e+04, atom= 851
Step=  714, Dmax= 1.5e-02 nm, Epot= -2.02979e+06 Fmax= 9.74435e+03, atom= 851
Step=  716, Dmax= 9.2e-03 nm, Epot= -2.02990e+06 Fmax= 2.29823e+03, atom= 851
Step=  717, Dmax= 1.1e-02 nm, Epot= -2.02993e+06 Fmax= 1.21652e+04, atom= 851
Step=  718, Dmax= 1.3e-02 nm, Epot= -2.03008e+06 Fmax= 5.15368e+03, atom= 851
Step=  720, Dmax= 7.9e-03 nm, Epot= -2.03013e+06 Fmax= 5.23736e+03, atom= 851
Step=  721, Dmax= 9.5e-03 nm, Epot= -2.03017e+06 Fmax= 7.19959e+03, atom= 851
Step=  722, Dmax= 1.1e-02 nm, Epot= -2.03021e+06 Fmax= 7.77099e+03, atom= 851
Step=  723, Dmax= 1.4e-02 nm, Epot= -2.03024e+06 Fmax= 1.01308e+04, atom= 851
Step=  724, Dmax= 1.6e-02 nm, Epot= -2.03026e+06 Fmax= 1.14369e+04, atom= 851
Step=  726, Dmax= 9.9e-03 nm, Epot= -2.03040e+06 Fmax= 1.51994e+03, atom= 851
Step=  727, Dmax= 1.2e-02 nm, Epot= -2.03050e+06 Fmax= 1.40190e+04, atom= 851
Step=  728, Dmax= 1.4e-02 nm, Epot= -2.03067e+06 Fmax= 4.60525e+03, atom= 851
Step=  730, Dmax= 8.5e-03 nm, Epot= -2.03071e+06 Fmax= 6.58690e+03, atom= 851
Step=  731, Dmax= 1.0e-02 nm, Epot= -2.03077e+06 Fmax= 6.78643e+03, atom= 851
Step=  732, Dmax= 1.2e-02 nm, Epot= -2.03079e+06 Fmax= 9.32100e+03, atom= 851
Step=  733, Dmax= 1.5e-02 nm, Epot= -2.03083e+06 Fmax= 9.93293e+03, atom= 851
Step=  735, Dmax= 8.8e-03 nm, Epot= -2.03094e+06 Fmax= 1.60903e+03, atom= 851
Step=  736, Dmax= 1.1e-02 nm, Epot= -2.03103e+06 Fmax= 1.22369e+04, atom= 851
Step=  737, Dmax= 1.3e-02 nm, Epot= -2.03118e+06 Fmax= 4.41393e+03, atom= 851
Step=  739, Dmax= 7.6e-03 nm, Epot= -2.03122e+06 Fmax= 5.56441e+03, atom= 851
Step=  740, Dmax= 9.2e-03 nm, Epot= -2.03127e+06 Fmax= 6.45324e+03, atom= 851
Step=  741, Dmax= 1.1e-02 nm, Epot= -2.03130e+06 Fmax= 7.91746e+03, atom= 851
Step=  742, Dmax= 1.3e-02 nm, Epot= -2.03133e+06 Fmax= 9.39161e+03, atom= 851
Step=  743, Dmax= 1.6e-02 nm, Epot= -2.03135e+06 Fmax= 1.12951e+04, atom= 851
Step=  744, Dmax= 1.9e-02 nm, Epot= -2.03136e+06 Fmax= 1.36409e+04, atom= 851
Step=  746, Dmax= 1.1e-02 nm, Epot= -2.03154e+06 Fmax= 1.34386e+03, atom= 851
Step=  747, Dmax= 1.4e-02 nm, Epot= -2.03164e+06 Fmax= 1.65921e+04, atom= 851
Step=  748, Dmax= 1.6e-02 nm, Epot= -2.03188e+06 Fmax= 4.93385e+03, atom= 851
Step=  750, Dmax= 9.9e-03 nm, Epot= -2.03191e+06 Fmax= 8.02406e+03, atom= 851
Step=  751, Dmax= 1.2e-02 nm, Epot= -2.03196e+06 Fmax= 7.43015e+03, atom= 851
Step=  752, Dmax= 1.4e-02 nm, Epot= -2.03196e+06 Fmax= 1.11959e+04, atom= 851
Step=  753, Dmax= 1.7e-02 nm, Epot= -2.03201e+06 Fmax= 1.10553e+04, atom= 851
Step=  755, Dmax= 1.0e-02 nm, Epot= -2.03214e+06 Fmax= 2.27952e+03, atom= 851
Step=  756, Dmax= 1.2e-02 nm, Epot= -2.03215e+06 Fmax= 1.37173e+04, atom= 851
Step=  757, Dmax= 1.5e-02 nm, Epot= -2.03232e+06 Fmax= 5.52078e+03, atom= 851
Step=  759, Dmax= 8.8e-03 nm, Epot= -2.03236e+06 Fmax= 6.01832e+03, atom= 851
Step=  760, Dmax= 1.1e-02 nm, Epot= -2.03240e+06 Fmax= 7.87079e+03, atom= 851
Step=  761, Dmax= 1.3e-02 nm, Epot= -2.03243e+06 Fmax= 8.73938e+03, atom= 851
Step=  762, Dmax= 1.5e-02 nm, Epot= -2.03245e+06 Fmax= 1.12696e+04, atom= 851
Step=  763, Dmax= 1.8e-02 nm, Epot= -2.03247e+06 Fmax= 1.26365e+04, atom= 851
Step=  765, Dmax= 1.1e-02 nm, Epot= -2.03262e+06 Fmax= 1.68672e+03, atom= 851
Step=  766, Dmax= 1.3e-02 nm, Epot= -2.03267e+06 Fmax= 1.55260e+04, atom= 851
Step=  767, Dmax= 1.6e-02 nm, Epot= -2.03288e+06 Fmax= 5.15347e+03, atom= 851
Step=  769, Dmax= 9.5e-03 nm, Epot= -2.03291e+06 Fmax= 7.22970e+03, atom= 851
Step=  770, Dmax= 1.1e-02 nm, Epot= -2.03296e+06 Fmax= 7.69869e+03, atom= 851
Step=  771, Dmax= 1.4e-02 nm, Epot= -2.03297e+06 Fmax= 1.01438e+04, atom= 851
Step=  772, Dmax= 1.6e-02 nm, Epot= -2.03300e+06 Fmax= 1.13575e+04, atom= 851
Step=  774, Dmax= 9.8e-03 nm, Epot= -2.03313e+06 Fmax= 1.55760e+03, atom= 851
Step=  775, Dmax= 1.2e-02 nm, Epot= -2.03322e+06 Fmax= 1.39387e+04, atom= 851
Step=  776, Dmax= 1.4e-02 nm, Epot= -2.03338e+06 Fmax= 4.62664e+03, atom= 851
Step=  778, Dmax= 8.5e-03 nm, Epot= -2.03341e+06 Fmax= 6.52995e+03, atom= 851
Step=  779, Dmax= 1.0e-02 nm, Epot= -2.03346e+06 Fmax= 6.80012e+03, atom= 851
Step=  780, Dmax= 1.2e-02 nm, Epot= -2.03348e+06 Fmax= 9.25789e+03, atom= 851
Step=  781, Dmax= 1.5e-02 nm, Epot= -2.03352e+06 Fmax= 9.93462e+03, atom= 851
Step=  783, Dmax= 8.8e-03 nm, Epot= -2.03363e+06 Fmax= 1.57173e+03, atom= 851
Step=  784, Dmax= 1.1e-02 nm, Epot= -2.03371e+06 Fmax= 1.22286e+04, atom= 851
Step=  785, Dmax= 1.3e-02 nm, Epot= -2.03385e+06 Fmax= 4.37126e+03, atom= 851
Step=  787, Dmax= 7.6e-03 nm, Epot= -2.03389e+06 Fmax= 5.57447e+03, atom= 851
Step=  788, Dmax= 9.1e-03 nm, Epot= -2.03393e+06 Fmax= 6.40613e+03, atom= 851
Step=  789, Dmax= 1.1e-02 nm, Epot= -2.03396e+06 Fmax= 7.91862e+03, atom= 851
Step=  790, Dmax= 1.3e-02 nm, Epot= -2.03399e+06 Fmax= 9.33661e+03, atom= 851
Step=  791, Dmax= 1.6e-02 nm, Epot= -2.03401e+06 Fmax= 1.12843e+04, atom= 851
Step=  792, Dmax= 1.9e-02 nm, Epot= -2.03402e+06 Fmax= 1.35742e+04, atom= 851
Step=  794, Dmax= 1.1e-02 nm, Epot= -2.03418e+06 Fmax= 1.36299e+03, atom= 851
Step=  795, Dmax= 1.4e-02 nm, Epot= -2.03428e+06 Fmax= 1.65232e+04, atom= 851
Step=  796, Dmax= 1.6e-02 nm, Epot= -2.03449e+06 Fmax= 4.93488e+03, atom= 851
Step=  798, Dmax= 9.8e-03 nm, Epot= -2.03452e+06 Fmax= 7.98227e+03, atom= 851
Step=  799, Dmax= 1.2e-02 nm, Epot= -2.03457e+06 Fmax= 7.42277e+03, atom= 851
Step=  800, Dmax= 1.4e-02 nm, Epot= -2.03457e+06 Fmax= 1.11455e+04, atom= 851
Step=  801, Dmax= 1.7e-02 nm, Epot= -2.03462e+06 Fmax= 1.10352e+04, atom= 851
Step=  803, Dmax= 1.0e-02 nm, Epot= -2.03473e+06 Fmax= 2.25854e+03, atom= 851
Step=  804, Dmax= 1.2e-02 nm, Epot= -2.03476e+06 Fmax= 1.36857e+04, atom= 851
Step=  805, Dmax= 1.5e-02 nm, Epot= -2.03490e+06 Fmax= 5.49348e+03, atom= 851
Step=  807, Dmax= 8.8e-03 nm, Epot= -2.03495e+06 Fmax= 6.00795e+03, atom= 851
Step=  808, Dmax= 1.1e-02 nm, Epot= -2.03498e+06 Fmax= 7.83894e+03, atom= 851
Step=  809, Dmax= 1.3e-02 nm, Epot= -2.03502e+06 Fmax= 8.71809e+03, atom= 851
Step=  810, Dmax= 1.5e-02 nm, Epot= -2.03503e+06 Fmax= 1.12291e+04, atom= 851
Step=  811, Dmax= 1.8e-02 nm, Epot= -2.03505e+06 Fmax= 1.26010e+04, atom= 851
Step=  813, Dmax= 1.1e-02 nm, Epot= -2.03520e+06 Fmax= 1.67814e+03, atom= 851
Step=  814, Dmax= 1.3e-02 nm, Epot= -2.03524e+06 Fmax= 1.54769e+04, atom= 851
Step=  815, Dmax= 1.6e-02 nm, Epot= -2.03543e+06 Fmax= 5.13920e+03, atom= 851
Step=  817, Dmax= 9.5e-03 nm, Epot= -2.03547e+06 Fmax= 7.20473e+03, atom= 851
Step=  818, Dmax= 1.1e-02 nm, Epot= -2.03550e+06 Fmax= 7.67781e+03, atom= 851
Step=  819, Dmax= 1.4e-02 nm, Epot= -2.03552e+06 Fmax= 1.01078e+04, atom= 851
Step=  820, Dmax= 1.6e-02 nm, Epot= -2.03555e+06 Fmax= 1.13276e+04, atom= 851
Step=  822, Dmax= 9.8e-03 nm, Epot= -2.03567e+06 Fmax= 1.54668e+03, atom= 851
Step=  823, Dmax= 1.2e-02 nm, Epot= -2.03574e+06 Fmax= 1.39049e+04, atom= 851
Step=  824, Dmax= 1.4e-02 nm, Epot= -2.03590e+06 Fmax= 4.60145e+03, atom= 851
Step=  826, Dmax= 8.5e-03 nm, Epot= -2.03594e+06 Fmax= 6.52164e+03, atom= 851
Step=  827, Dmax= 1.0e-02 nm, Epot= -2.03598e+06 Fmax= 6.76666e+03, atom= 851
Step=  828, Dmax= 1.2e-02 nm, Epot= -2.03600e+06 Fmax= 9.24200e+03, atom= 851
Step=  829, Dmax= 1.5e-02 nm, Epot= -2.03603e+06 Fmax= 9.88998e+03, atom= 851
Step=  831, Dmax= 8.8e-03 nm, Epot= -2.03613e+06 Fmax= 1.58096e+03, atom= 851
Step=  832, Dmax= 1.1e-02 nm, Epot= -2.03621e+06 Fmax= 1.21728e+04, atom= 851
Step=  833, Dmax= 1.3e-02 nm, Epot= -2.03634e+06 Fmax= 4.37575e+03, atom= 851
Step=  835, Dmax= 7.6e-03 nm, Epot= -2.03638e+06 Fmax= 5.53821e+03, atom= 851
Step=  836, Dmax= 9.1e-03 nm, Epot= -2.03641e+06 Fmax= 6.40607e+03, atom= 851
Step=  837, Dmax= 1.1e-02 nm, Epot= -2.03644e+06 Fmax= 7.87326e+03, atom= 851
Step=  838, Dmax= 1.3e-02 nm, Epot= -2.03647e+06 Fmax= 9.32914e+03, atom= 851
Step=  839, Dmax= 1.6e-02 nm, Epot= -2.03649e+06 Fmax= 1.12270e+04, atom= 851
Step=  840, Dmax= 1.9e-02 nm, Epot= -2.03650e+06 Fmax= 1.35548e+04, atom= 851
Step=  842, Dmax= 1.1e-02 nm, Epot= -2.03665e+06 Fmax= 1.33504e+03, atom= 851
Step=  843, Dmax= 1.4e-02 nm, Epot= -2.03674e+06 Fmax= 1.64970e+04, atom= 851
Step=  844, Dmax= 1.6e-02 nm, Epot= -2.03694e+06 Fmax= 4.89289e+03, atom= 851
Step=  846, Dmax= 9.8e-03 nm, Epot= -2.03697e+06 Fmax= 7.98653e+03, atom= 851
Step=  847, Dmax= 1.2e-02 nm, Epot= -2.03702e+06 Fmax= 7.36943e+03, atom= 851
Step=  849, Dmax= 7.1e-03 nm, Epot= -2.03708e+06 Fmax= 1.84851e+03, atom= 851
Step=  850, Dmax= 8.5e-03 nm, Epot= -2.03714e+06 Fmax= 9.17921e+03, atom= 851
Step=  851, Dmax= 1.0e-02 nm, Epot= -2.03722e+06 Fmax= 4.10604e+03, atom= 851
Step=  853, Dmax= 6.1e-03 nm, Epot= -2.03727e+06 Fmax= 3.85877e+03, atom= 851
Step=  854, Dmax= 7.3e-03 nm, Epot= -2.03731e+06 Fmax= 5.72975e+03, atom= 851
Step=  855, Dmax= 8.8e-03 nm, Epot= -2.03735e+06 Fmax= 5.73622e+03, atom= 851
Step=  856, Dmax= 1.1e-02 nm, Epot= -2.03737e+06 Fmax= 8.07325e+03, atom= 851
Step=  857, Dmax= 1.3e-02 nm, Epot= -2.03741e+06 Fmax= 8.43421e+03, atom= 851
Step=  858, Dmax= 1.5e-02 nm, Epot= -2.03742e+06 Fmax= 1.14566e+04, atom= 851
Step=  859, Dmax= 1.8e-02 nm, Epot= -2.03744e+06 Fmax= 1.23025e+04, atom= 851
Step=  861, Dmax= 1.1e-02 nm, Epot= -2.03758e+06 Fmax= 1.93563e+03, atom= 851
Step=  862, Dmax= 1.3e-02 nm, Epot= -2.03760e+06 Fmax= 1.51543e+04, atom= 851
Step=  863, Dmax= 1.6e-02 nm, Epot= -2.03776e+06 Fmax= 5.39744e+03, atom= 851
Step=  865, Dmax= 9.4e-03 nm, Epot= -2.03780e+06 Fmax= 6.91520e+03, atom= 851
Step=  866, Dmax= 1.1e-02 nm, Epot= -2.03783e+06 Fmax= 7.92283e+03, atom= 851
Step=  867, Dmax= 1.4e-02 nm, Epot= -2.03786e+06 Fmax= 9.81072e+03, atom= 851
Step=  868, Dmax= 1.6e-02 nm, Epot= -2.03787e+06 Fmax= 1.15619e+04, atom= 851
Step=  869, Dmax= 2.0e-02 nm, Epot= -2.03787e+06 Fmax= 1.39624e+04, atom= 851
Step=  871, Dmax= 1.2e-02 nm, Epot= -2.03804e+06 Fmax= 1.33079e+03, atom= 851
Step=  872, Dmax= 1.4e-02 nm, Epot= -2.03810e+06 Fmax= 1.70752e+04, atom= 851
Step=  873, Dmax= 1.7e-02 nm, Epot= -2.03833e+06 Fmax= 5.02532e+03, atom= 851
Step=  875, Dmax= 1.0e-02 nm, Epot= -2.03835e+06 Fmax= 8.17481e+03, atom= 851
Step=  876, Dmax= 1.2e-02 nm, Epot= -2.03839e+06 Fmax= 7.77391e+03, atom= 851
Step=  878, Dmax= 7.3e-03 nm, Epot= -2.03846e+06 Fmax= 1.79106e+03, atom= 851
Step=  879, Dmax= 8.8e-03 nm, Epot= -2.03852e+06 Fmax= 9.72468e+03, atom= 851
Step=  880, Dmax= 1.1e-02 nm, Epot= -2.03861e+06 Fmax= 4.03850e+03, atom= 851
Step=  882, Dmax= 6.3e-03 nm, Epot= -2.03865e+06 Fmax= 4.22628e+03, atom= 851
Step=  883, Dmax= 7.6e-03 nm, Epot= -2.03868e+06 Fmax= 5.65918e+03, atom= 851
Step=  884, Dmax= 9.1e-03 nm, Epot= -2.03872e+06 Fmax= 6.24573e+03, atom= 851
Step=  885, Dmax= 1.1e-02 nm, Epot= -2.03875e+06 Fmax= 7.98748e+03, atom= 851
Step=  886, Dmax= 1.3e-02 nm, Epot= -2.03878e+06 Fmax= 9.15991e+03, atom= 851
Step=  887, Dmax= 1.6e-02 nm, Epot= -2.03879e+06 Fmax= 1.13292e+04, atom= 851
Step=  888, Dmax= 1.9e-02 nm, Epot= -2.03880e+06 Fmax= 1.33735e+04, atom= 851
Step=  890, Dmax= 1.1e-02 nm, Epot= -2.03895e+06 Fmax= 1.46770e+03, atom= 851
Step=  891, Dmax= 1.4e-02 nm, Epot= -2.03899e+06 Fmax= 1.63192e+04, atom= 851
Step=  892, Dmax= 1.6e-02 nm, Epot= -2.03919e+06 Fmax= 5.00351e+03, atom= 851
Step=  894, Dmax= 9.8e-03 nm, Epot= -2.03922e+06 Fmax= 7.82791e+03, atom= 851
Step=  895, Dmax= 1.2e-02 nm, Epot= -2.03926e+06 Fmax= 7.47872e+03, atom= 851
Step=  896, Dmax= 1.4e-02 nm, Epot= -2.03927e+06 Fmax= 1.09728e+04, atom= 851
Step=  897, Dmax= 1.7e-02 nm, Epot= -2.03931e+06 Fmax= 1.10663e+04, atom= 851
Step=  899, Dmax= 1.0e-02 nm, Epot= -2.03941e+06 Fmax= 2.14420e+03, atom= 851
Step=  900, Dmax= 1.2e-02 nm, Epot= -2.03942e+06 Fmax= 1.36977e+04, atom= 851
Step=  901, Dmax= 1.5e-02 nm, Epot= -2.03957e+06 Fmax= 5.36274e+03, atom= 851
Step=  903, Dmax= 8.7e-03 nm, Epot= -2.03960e+06 Fmax= 6.06395e+03, atom= 851
Step=  904, Dmax= 1.0e-02 nm, Epot= -2.03963e+06 Fmax= 7.69707e+03, atom= 851
Step=  905, Dmax= 1.3e-02 nm, Epot= -2.03966e+06 Fmax= 8.75404e+03, atom= 851
Step=  906, Dmax= 1.5e-02 nm, Epot= -2.03967e+06 Fmax= 1.10683e+04, atom= 851
Step=  907, Dmax= 1.8e-02 nm, Epot= -2.03968e+06 Fmax= 1.26103e+04, atom= 851
Step=  909, Dmax= 1.1e-02 nm, Epot= -2.03982e+06 Fmax= 1.57939e+03, atom= 851
Step=  910, Dmax= 1.3e-02 nm, Epot= -2.03986e+06 Fmax= 1.54666e+04, atom= 851
Step=  911, Dmax= 1.6e-02 nm, Epot= -2.04004e+06 Fmax= 5.02309e+03, atom= 851
Step=  913, Dmax= 9.4e-03 nm, Epot= -2.04006e+06 Fmax= 7.23858e+03, atom= 851
Step=  914, Dmax= 1.1e-02 nm, Epot= -2.04010e+06 Fmax= 7.55181e+03, atom= 851
Step=  915, Dmax= 1.4e-02 nm, Epot= -2.04012e+06 Fmax= 1.01200e+04, atom= 851
Step=  916, Dmax= 1.6e-02 nm, Epot= -2.04014e+06 Fmax= 1.11807e+04, atom= 851
Step=  918, Dmax= 9.7e-03 nm, Epot= -2.04024e+06 Fmax= 1.61092e+03, atom= 851
Step=  919, Dmax= 1.2e-02 nm, Epot= -2.04030e+06 Fmax= 1.37494e+04, atom= 851
Step=  920, Dmax= 1.4e-02 nm, Epot= -2.04045e+06 Fmax= 4.63962e+03, atom= 851
Step=  922, Dmax= 8.4e-03 nm, Epot= -2.04048e+06 Fmax= 6.41207e+03, atom= 851
Step=  923, Dmax= 1.0e-02 nm, Epot= -2.04052e+06 Fmax= 6.79151e+03, atom= 851
Step=  924, Dmax= 1.2e-02 nm, Epot= -2.04053e+06 Fmax= 9.11636e+03, atom= 851
Step=  925, Dmax= 1.5e-02 nm, Epot= -2.04055e+06 Fmax= 9.89368e+03, atom= 851
Step=  927, Dmax= 8.7e-03 nm, Epot= -2.04064e+06 Fmax= 1.50585e+03, atom= 851
Step=  928, Dmax= 1.0e-02 nm, Epot= -2.04072e+06 Fmax= 1.21589e+04, atom= 851
Step=  929, Dmax= 1.3e-02 nm, Epot= -2.04083e+06 Fmax= 4.28711e+03, atom= 851
Step=  931, Dmax= 7.5e-03 nm, Epot= -2.04086e+06 Fmax= 5.56215e+03, atom= 851
Step=  932, Dmax= 9.1e-03 nm, Epot= -2.04090e+06 Fmax= 6.30765e+03, atom= 851
Step=  933, Dmax= 1.1e-02 nm, Epot= -2.04093e+06 Fmax= 7.88037e+03, atom= 851
Step=  934, Dmax= 1.3e-02 nm, Epot= -2.04096e+06 Fmax= 9.21433e+03, atom= 851
Step=  935, Dmax= 1.6e-02 nm, Epot= -2.04096e+06 Fmax= 1.12110e+04, atom= 851
Step=  936, Dmax= 1.9e-02 nm, Epot= -2.04097e+06 Fmax= 1.34152e+04, atom= 851
Step=  938, Dmax= 1.1e-02 nm, Epot= -2.04112e+06 Fmax= 1.37938e+03, atom= 851
Step=  939, Dmax= 1.4e-02 nm, Epot= -2.04117e+06 Fmax= 1.63485e+04, atom= 851
Step=  940, Dmax= 1.6e-02 nm, Epot= -2.04136e+06 Fmax= 4.90596e+03, atom= 851
Step=  942, Dmax= 9.7e-03 nm, Epot= -2.04138e+06 Fmax= 7.88990e+03, atom= 851
Step=  943, Dmax= 1.2e-02 nm, Epot= -2.04142e+06 Fmax= 7.36893e+03, atom= 851
Step=  944, Dmax= 1.4e-02 nm, Epot= -2.04142e+06 Fmax= 1.10260e+04, atom= 851
Step=  945, Dmax= 1.7e-02 nm, Epot= -2.04146e+06 Fmax= 1.09445e+04, atom= 851
Step=  947, Dmax= 1.0e-02 nm, Epot= -2.04157e+06 Fmax= 2.22527e+03, atom= 851
Step=  948, Dmax= 1.2e-02 nm, Epot= -2.04158e+06 Fmax= 1.35658e+04, atom= 851
Step=  949, Dmax= 1.5e-02 nm, Epot= -2.04171e+06 Fmax= 5.43511e+03, atom= 851
Step=  951, Dmax= 8.7e-03 nm, Epot= -2.04175e+06 Fmax= 5.95698e+03, atom= 851
Step=  952, Dmax= 1.0e-02 nm, Epot= -2.04177e+06 Fmax= 7.76112e+03, atom= 851
Step=  953, Dmax= 1.3e-02 nm, Epot= -2.04179e+06 Fmax= 8.63893e+03, atom= 851
Step=  954, Dmax= 1.5e-02 nm, Epot= -2.04180e+06 Fmax= 1.11221e+04, atom= 851
Step=  955, Dmax= 1.8e-02 nm, Epot= -2.04182e+06 Fmax= 1.24830e+04, atom= 851
Step=  957, Dmax= 1.1e-02 nm, Epot= -2.04195e+06 Fmax= 1.66293e+03, atom= 851
Step=  958, Dmax= 1.3e-02 nm, Epot= -2.04196e+06 Fmax= 1.53264e+04, atom= 851
Step=  959, Dmax= 1.6e-02 nm, Epot= -2.04214e+06 Fmax= 5.09804e+03, atom= 851
Step=  961, Dmax= 9.4e-03 nm, Epot= -2.04217e+06 Fmax= 7.12828e+03, atom= 851
Step=  962, Dmax= 1.1e-02 nm, Epot= -2.04220e+06 Fmax= 7.61506e+03, atom= 851
Step=  963, Dmax= 1.3e-02 nm, Epot= -2.04221e+06 Fmax= 1.00026e+04, atom= 851
Step=  964, Dmax= 1.6e-02 nm, Epot= -2.04223e+06 Fmax= 1.12322e+04, atom= 851
Step=  966, Dmax= 9.7e-03 nm, Epot= -2.04233e+06 Fmax= 1.51961e+03, atom= 851
Step=  967, Dmax= 1.2e-02 nm, Epot= -2.04239e+06 Fmax= 1.37907e+04, atom= 851
Step=  968, Dmax= 1.4e-02 nm, Epot= -2.04253e+06 Fmax= 4.53984e+03, atom= 851
Step=  970, Dmax= 8.4e-03 nm, Epot= -2.04255e+06 Fmax= 6.47998e+03, atom= 851
Step=  971, Dmax= 1.0e-02 nm, Epot= -2.04259e+06 Fmax= 6.68216e+03, atom= 851
Step=  972, Dmax= 1.2e-02 nm, Epot= -2.04261e+06 Fmax= 9.17706e+03, atom= 851
Step=  973, Dmax= 1.5e-02 nm, Epot= -2.04263e+06 Fmax= 9.77405e+03, atom= 851
Step=  975, Dmax= 8.7e-03 nm, Epot= -2.04272e+06 Fmax= 1.59000e+03, atom= 851
Step=  976, Dmax= 1.0e-02 nm, Epot= -2.04278e+06 Fmax= 1.20308e+04, atom= 851
Step=  977, Dmax= 1.3e-02 nm, Epot= -2.04289e+06 Fmax= 4.36362e+03, atom= 851
Step=  979, Dmax= 7.5e-03 nm, Epot= -2.04292e+06 Fmax= 5.45669e+03, atom= 851
Step=  980, Dmax= 9.0e-03 nm, Epot= -2.04295e+06 Fmax= 6.37613e+03, atom= 851
Step=  981, Dmax= 1.1e-02 nm, Epot= -2.04298e+06 Fmax= 7.76799e+03, atom= 851
Step=  982, Dmax= 1.3e-02 nm, Epot= -2.04300e+06 Fmax= 9.27354e+03, atom= 851
Step=  983, Dmax= 1.6e-02 nm, Epot= -2.04301e+06 Fmax= 1.10883e+04, atom= 851
Step=  984, Dmax= 1.9e-02 nm, Epot= -2.04301e+06 Fmax= 1.34613e+04, atom= 851
Step=  986, Dmax= 1.1e-02 nm, Epot= -2.04315e+06 Fmax= 1.28746e+03, atom= 851
Step=  987, Dmax= 1.3e-02 nm, Epot= -2.04321e+06 Fmax= 1.63791e+04, atom= 851
Step=  988, Dmax= 1.6e-02 nm, Epot= -2.04340e+06 Fmax= 4.80707e+03, atom= 851
Step=  990, Dmax= 9.7e-03 nm, Epot= -2.04342e+06 Fmax= 7.95407e+03, atom= 851
Step=  991, Dmax= 1.2e-02 nm, Epot= -2.04346e+06 Fmax= 7.25668e+03, atom= 851
Step=  993, Dmax= 7.0e-03 nm, Epot= -2.04351e+06 Fmax= 1.87560e+03, atom= 851
Step=  994, Dmax= 8.4e-03 nm, Epot= -2.04356e+06 Fmax= 9.04701e+03, atom= 851
Step=  995, Dmax= 1.0e-02 nm, Epot= -2.04363e+06 Fmax= 4.11408e+03, atom= 851
Step=  997, Dmax= 6.0e-03 nm, Epot= -2.04367e+06 Fmax= 3.77503e+03, atom= 851
Step=  998, Dmax= 7.2e-03 nm, Epot= -2.04370e+06 Fmax= 5.72396e+03, atom= 851
Step=  999, Dmax= 8.7e-03 nm, Epot= -2.04373e+06 Fmax= 5.63381e+03, atom= 851
Step= 1000, Dmax= 1.0e-02 nm, Epot= -2.04375e+06 Fmax= 8.04648e+03, atom= 851
Step= 1001, Dmax= 1.3e-02 nm, Epot= -2.04378e+06 Fmax= 8.30460e+03, atom= 851
Step= 1002, Dmax= 1.5e-02 nm, Epot= -2.04379e+06 Fmax= 1.14000e+04, atom= 851
Step= 1003, Dmax= 1.8e-02 nm, Epot= -2.04381e+06 Fmax= 1.21351e+04, atom= 851
Step= 1005, Dmax= 1.1e-02 nm, Epot= -2.04393e+06 Fmax= 1.96996e+03, atom= 851
Step= 1007, Dmax= 6.5e-03 nm, Epot= -2.04397e+06 Fmax= 6.52363e+03, atom= 851
Step= 1008, Dmax= 7.8e-03 nm, Epot= -2.04402e+06 Fmax= 3.66991e+03, atom= 851
Step= 1009, Dmax= 9.3e-03 nm, Epot= -2.04404e+06 Fmax= 8.51160e+03, atom= 851
Step= 1010, Dmax= 1.1e-02 nm, Epot= -2.04409e+06 Fmax= 6.16806e+03, atom= 851
Step= 1012, Dmax= 6.7e-03 nm, Epot= -2.04414e+06 Fmax= 2.63859e+03, atom= 851
Step= 1013, Dmax= 8.1e-03 nm, Epot= -2.04417e+06 Fmax= 7.95848e+03, atom= 851
Step= 1014, Dmax= 9.7e-03 nm, Epot= -2.04422e+06 Fmax= 4.71420e+03, atom= 851
Step= 1016, Dmax= 5.8e-03 nm, Epot= -2.04426e+06 Fmax= 2.89374e+03, atom= 851
Step= 1017, Dmax= 7.0e-03 nm, Epot= -2.04429e+06 Fmax= 6.20810e+03, atom= 851
Step= 1018, Dmax= 8.4e-03 nm, Epot= -2.04433e+06 Fmax= 4.75348e+03, atom= 851
Step= 1019, Dmax= 1.0e-02 nm, Epot= -2.04434e+06 Fmax= 8.35114e+03, atom= 851
Step= 1020, Dmax= 1.2e-02 nm, Epot= -2.04438e+06 Fmax= 7.43776e+03, atom= 851
Step= 1022, Dmax= 7.2e-03 nm, Epot= -2.04444e+06 Fmax= 2.03624e+03, atom= 851
Step= 1023, Dmax= 8.7e-03 nm, Epot= -2.04448e+06 Fmax= 9.36252e+03, atom= 851
Step= 1024, Dmax= 1.0e-02 nm, Epot= -2.04455e+06 Fmax= 4.26732e+03, atom= 851
Step= 1026, Dmax= 6.2e-03 nm, Epot= -2.04459e+06 Fmax= 3.91804e+03, atom= 851
Step= 1027, Dmax= 7.5e-03 nm, Epot= -2.04462e+06 Fmax= 5.87088e+03, atom= 851
Step= 1028, Dmax= 9.0e-03 nm, Epot= -2.04466e+06 Fmax= 5.91980e+03, atom= 851
Step= 1029, Dmax= 1.1e-02 nm, Epot= -2.04467e+06 Fmax= 8.17505e+03, atom= 851
Step= 1030, Dmax= 1.3e-02 nm, Epot= -2.04470e+06 Fmax= 8.80746e+03, atom= 851
Step= 1031, Dmax= 1.6e-02 nm, Epot= -2.04471e+06 Fmax= 1.14834e+04, atom= 851
Step= 1032, Dmax= 1.9e-02 nm, Epot= -2.04472e+06 Fmax= 1.29816e+04, atom= 851
Step= 1034, Dmax= 1.1e-02 nm, Epot= -2.04485e+06 Fmax= 1.71531e+03, atom= 851
Step= 1035, Dmax= 1.3e-02 nm, Epot= -2.04485e+06 Fmax= 1.59152e+04, atom= 851
Step= 1036, Dmax= 1.6e-02 nm, Epot= -2.04502e+06 Fmax= 5.20537e+03, atom= 851
Step= 1038, Dmax= 9.7e-03 nm, Epot= -2.04505e+06 Fmax= 7.49216e+03, atom= 851
Step= 1039, Dmax= 1.2e-02 nm, Epot= -2.04508e+06 Fmax= 7.66788e+03, atom= 851
Step= 1041, Dmax= 7.0e-03 nm, Epot= -2.04514e+06 Fmax= 1.43084e+03, atom= 851
Step= 1042, Dmax= 8.4e-03 nm, Epot= -2.04520e+06 Fmax= 9.45580e+03, atom= 851
Step= 1043, Dmax= 1.0e-02 nm, Epot= -2.04528e+06 Fmax= 3.66219e+03, atom= 851
Step= 1045, Dmax= 6.0e-03 nm, Epot= -2.04531e+06 Fmax= 4.19634e+03, atom= 851
Step= 1046, Dmax= 7.2e-03 nm, Epot= -2.04534e+06 Fmax= 5.27009e+03, atom= 851
Step= 1047, Dmax= 8.7e-03 nm, Epot= -2.04537e+06 Fmax= 6.04677e+03, atom= 851
Step= 1048, Dmax= 1.0e-02 nm, Epot= -2.04539e+06 Fmax= 7.58604e+03, atom= 851
Step= 1049, Dmax= 1.2e-02 nm, Epot= -2.04541e+06 Fmax= 8.70769e+03, atom= 851
Step= 1050, Dmax= 1.5e-02 nm, Epot= -2.04542e+06 Fmax= 1.09280e+04, atom= 851
Step= 1051, Dmax= 1.8e-02 nm, Epot= -2.04543e+06 Fmax= 1.25251e+04, atom= 851
Step= 1053, Dmax= 1.1e-02 nm, Epot= -2.04555e+06 Fmax= 1.53168e+03, atom= 851
Step= 1054, Dmax= 1.3e-02 nm, Epot= -2.04558e+06 Fmax= 1.53502e+04, atom= 851
Step= 1055, Dmax= 1.6e-02 nm, Epot= -2.04574e+06 Fmax= 4.94706e+03, atom= 851
Step= 1057, Dmax= 9.3e-03 nm, Epot= -2.04576e+06 Fmax= 7.19642e+03, atom= 851
Step= 1058, Dmax= 1.1e-02 nm, Epot= -2.04579e+06 Fmax= 7.45432e+03, atom= 851
Step= 1059, Dmax= 1.3e-02 nm, Epot= -2.04580e+06 Fmax= 1.00490e+04, atom= 851
Step= 1060, Dmax= 1.6e-02 nm, Epot= -2.04582e+06 Fmax= 1.10503e+04, atom= 851
Step= 1062, Dmax= 9.7e-03 nm, Epot= -2.04592e+06 Fmax= 1.61951e+03, atom= 851
Step= 1063, Dmax= 1.2e-02 nm, Epot= -2.04595e+06 Fmax= 1.35969e+04, atom= 851
Step= 1064, Dmax= 1.4e-02 nm, Epot= -2.04608e+06 Fmax= 4.61703e+03, atom= 851
Step= 1066, Dmax= 8.3e-03 nm, Epot= -2.04611e+06 Fmax= 6.32931e+03, atom= 851
Step= 1067, Dmax= 1.0e-02 nm, Epot= -2.04613e+06 Fmax= 6.74874e+03, atom= 851
Step= 1068, Dmax= 1.2e-02 nm, Epot= -2.04615e+06 Fmax= 9.00824e+03, atom= 851
Step= 1069, Dmax= 1.4e-02 nm, Epot= -2.04618e+06 Fmax= 9.82129e+03, atom= 851
Step= 1071, Dmax= 8.6e-03 nm, Epot= -2.04626e+06 Fmax= 1.47040e+03, atom= 851
Step= 1072, Dmax= 1.0e-02 nm, Epot= -2.04631e+06 Fmax= 1.20645e+04, atom= 851
Step= 1073, Dmax= 1.2e-02 nm, Epot= -2.04641e+06 Fmax= 4.22650e+03, atom= 851
Step= 1075, Dmax= 7.5e-03 nm, Epot= -2.04645e+06 Fmax= 5.52859e+03, atom= 851
Step= 1076, Dmax= 9.0e-03 nm, Epot= -2.04648e+06 Fmax= 6.22886e+03, atom= 851
Step= 1077, Dmax= 1.1e-02 nm, Epot= -2.04649e+06 Fmax= 7.82409e+03, atom= 851
Step= 1078, Dmax= 1.3e-02 nm, Epot= -2.04652e+06 Fmax= 9.10794e+03, atom= 851
Step= 1079, Dmax= 1.5e-02 nm, Epot= -2.04652e+06 Fmax= 1.11232e+04, atom= 851
Step= 1080, Dmax= 1.9e-02 nm, Epot= -2.04653e+06 Fmax= 1.32686e+04, atom= 851
Step= 1082, Dmax= 1.1e-02 nm, Epot= -2.04666e+06 Fmax= 1.38457e+03, atom= 851
Step= 1083, Dmax= 1.3e-02 nm, Epot= -2.04669e+06 Fmax= 1.61747e+04, atom= 851
Step= 1084, Dmax= 1.6e-02 nm, Epot= -2.04687e+06 Fmax= 4.87715e+03, atom= 851
Step= 1086, Dmax= 9.6e-03 nm, Epot= -2.04689e+06 Fmax= 7.79560e+03, atom= 851
Step= 1087, Dmax= 1.2e-02 nm, Epot= -2.04692e+06 Fmax= 7.31801e+03, atom= 851
Step= 1089, Dmax= 6.9e-03 nm, Epot= -2.04697e+06 Fmax= 1.75486e+03, atom= 851
Step= 1090, Dmax= 8.3e-03 nm, Epot= -2.04701e+06 Fmax= 9.09879e+03, atom= 851
Step= 1091, Dmax= 1.0e-02 nm, Epot= -2.04708e+06 Fmax= 3.97798e+03, atom= 851
Step= 1093, Dmax= 6.0e-03 nm, Epot= -2.04711e+06 Fmax= 3.86023e+03, atom= 851
Step= 1094, Dmax= 7.2e-03 nm, Epot= -2.04714e+06 Fmax= 5.57743e+03, atom= 851
Step= 1095, Dmax= 8.6e-03 nm, Epot= -2.04717e+06 Fmax= 5.70694e+03, atom= 851
Step= 1096, Dmax= 1.0e-02 nm, Epot= -2.04719e+06 Fmax= 7.88485e+03, atom= 851
Step= 1097, Dmax= 1.2e-02 nm, Epot= -2.04722e+06 Fmax= 8.36130e+03, atom= 851
Step= 1099, Dmax= 7.5e-03 nm, Epot= -2.04728e+06 Fmax= 1.38495e+03, atom= 851
Step= 1100, Dmax= 8.9e-03 nm, Epot= -2.04735e+06 Fmax= 1.02850e+04, atom= 851
Step= 1101, Dmax= 1.1e-02 nm, Epot= -2.04743e+06 Fmax= 3.77123e+03, atom= 851
Step= 1103, Dmax= 6.4e-03 nm, Epot= -2.04746e+06 Fmax= 4.64632e+03, atom= 851
Step= 1104, Dmax= 7.7e-03 nm, Epot= -2.04749e+06 Fmax= 5.49721e+03, atom= 851
Step= 1105, Dmax= 9.3e-03 nm, Epot= -2.04751e+06 Fmax= 6.62776e+03, atom= 851
Step= 1106, Dmax= 1.1e-02 nm, Epot= -2.04753e+06 Fmax= 7.97893e+03, atom= 851
Step= 1107, Dmax= 1.3e-02 nm, Epot= -2.04755e+06 Fmax= 9.47805e+03, atom= 851
Step= 1108, Dmax= 1.6e-02 nm, Epot= -2.04756e+06 Fmax= 1.15619e+04, atom= 851
Step= 1109, Dmax= 1.9e-02 nm, Epot= -2.04756e+06 Fmax= 1.35637e+04, atom= 851
Step= 1111, Dmax= 1.2e-02 nm, Epot= -2.04770e+06 Fmax= 1.49232e+03, atom= 851
Step= 1112, Dmax= 1.4e-02 nm, Epot= -2.04770e+06 Fmax= 1.66107e+04, atom= 851
Step= 1113, Dmax= 1.7e-02 nm, Epot= -2.04789e+06 Fmax= 5.13943e+03, atom= 851
Step= 1115, Dmax= 1.0e-02 nm, Epot= -2.04790e+06 Fmax= 7.86430e+03, atom= 851
Step= 1116, Dmax= 1.2e-02 nm, Epot= -2.04793e+06 Fmax= 7.83384e+03, atom= 851
Step= 1118, Dmax= 7.2e-03 nm, Epot= -2.04798e+06 Fmax= 1.58113e+03, atom= 851
Step= 1119, Dmax= 8.6e-03 nm, Epot= -2.04804e+06 Fmax= 9.75373e+03, atom= 851
Step= 1120, Dmax= 1.0e-02 nm, Epot= -2.04811e+06 Fmax= 3.79321e+03, atom= 851
Step= 1122, Dmax= 6.2e-03 nm, Epot= -2.04815e+06 Fmax= 4.34413e+03, atom= 851
Step= 1123, Dmax= 7.4e-03 nm, Epot= -2.04816e+06 Fmax= 5.38633e+03, atom= 851
Step= 1124, Dmax= 8.9e-03 nm, Epot= -2.04819e+06 Fmax= 6.33293e+03, atom= 851
Step= 1125, Dmax= 1.1e-02 nm, Epot= -2.04821e+06 Fmax= 7.67714e+03, atom= 851
Step= 1126, Dmax= 1.3e-02 nm, Epot= -2.04823e+06 Fmax= 9.20201e+03, atom= 851
Step= 1127, Dmax= 1.5e-02 nm, Epot= -2.04824e+06 Fmax= 1.09668e+04, atom= 851
Step= 1128, Dmax= 1.9e-02 nm, Epot= -2.04824e+06 Fmax= 1.33491e+04, atom= 851
Step= 1130, Dmax= 1.1e-02 nm, Epot= -2.04837e+06 Fmax= 1.25854e+03, atom= 851
Step= 1131, Dmax= 1.3e-02 nm, Epot= -2.04842e+06 Fmax= 1.62361e+04, atom= 851
Step= 1132, Dmax= 1.6e-02 nm, Epot= -2.04859e+06 Fmax= 4.74679e+03, atom= 851
Step= 1134, Dmax= 9.6e-03 nm, Epot= -2.04861e+06 Fmax= 7.89375e+03, atom= 851
Step= 1135, Dmax= 1.2e-02 nm, Epot= -2.04864e+06 Fmax= 7.17236e+03, atom= 851
Step= 1137, Dmax= 6.9e-03 nm, Epot= -2.04869e+06 Fmax= 1.87270e+03, atom= 851
Step= 1138, Dmax= 8.3e-03 nm, Epot= -2.04873e+06 Fmax= 8.94713e+03, atom= 851
Step= 1139, Dmax= 1.0e-02 nm, Epot= -2.04879e+06 Fmax= 4.08832e+03, atom= 851
Step= 1141, Dmax= 6.0e-03 nm, Epot= -2.04882e+06 Fmax= 3.72616e+03, atom= 851
Step= 1142, Dmax= 7.2e-03 nm, Epot= -2.04885e+06 Fmax= 5.68136e+03, atom= 851
Step= 1143, Dmax= 8.6e-03 nm, Epot= -2.04888e+06 Fmax= 5.56811e+03, atom= 851
Step= 1144, Dmax= 1.0e-02 nm, Epot= -2.04889e+06 Fmax= 7.98155e+03, atom= 851
Step= 1145, Dmax= 1.2e-02 nm, Epot= -2.04892e+06 Fmax= 8.21446e+03, atom= 851
Step= 1146, Dmax= 1.5e-02 nm, Epot= -2.04892e+06 Fmax= 1.13012e+04, atom= 851
Step= 1147, Dmax= 1.8e-02 nm, Epot= -2.04894e+06 Fmax= 1.20104e+04, atom= 851
Step= 1149, Dmax= 1.1e-02 nm, Epot= -2.04904e+06 Fmax= 1.96054e+03, atom= 851
Step= 1151, Dmax= 6.4e-03 nm, Epot= -2.04908e+06 Fmax= 6.45314e+03, atom= 851
Step= 1152, Dmax= 7.7e-03 nm, Epot= -2.04913e+06 Fmax= 3.64241e+03, atom= 851
Step= 1153, Dmax= 9.2e-03 nm, Epot= -2.04914e+06 Fmax= 8.42416e+03, atom= 851
Step= 1154, Dmax= 1.1e-02 nm, Epot= -2.04919e+06 Fmax= 6.11470e+03, atom= 851
Step= 1156, Dmax= 6.7e-03 nm, Epot= -2.04923e+06 Fmax= 2.60847e+03, atom= 851
Step= 1157, Dmax= 8.0e-03 nm, Epot= -2.04925e+06 Fmax= 7.88585e+03, atom= 851
Step= 1158, Dmax= 9.6e-03 nm, Epot= -2.04930e+06 Fmax= 4.66651e+03, atom= 851
Step= 1160, Dmax= 5.8e-03 nm, Epot= -2.04933e+06 Fmax= 2.86866e+03, atom= 851
Step= 1161, Dmax= 6.9e-03 nm, Epot= -2.04936e+06 Fmax= 6.14743e+03, atom= 851
Step= 1162, Dmax= 8.3e-03 nm, Epot= -2.04940e+06 Fmax= 4.70912e+03, atom= 851
Step= 1163, Dmax= 9.9e-03 nm, Epot= -2.04941e+06 Fmax= 8.27134e+03, atom= 851
Step= 1164, Dmax= 1.2e-02 nm, Epot= -2.04944e+06 Fmax= 7.36634e+03, atom= 851
Step= 1166, Dmax= 7.2e-03 nm, Epot= -2.04949e+06 Fmax= 2.01711e+03, atom= 851
Step= 1167, Dmax= 8.6e-03 nm, Epot= -2.04952e+06 Fmax= 9.27054e+03, atom= 851
Step= 1168, Dmax= 1.0e-02 nm, Epot= -2.04959e+06 Fmax= 4.22939e+03, atom= 851
Step= 1170, Dmax= 6.2e-03 nm, Epot= -2.04962e+06 Fmax= 3.87668e+03, atom= 851
Step= 1171, Dmax= 7.4e-03 nm, Epot= -2.04964e+06 Fmax= 5.82045e+03, atom= 851
Step= 1172, Dmax= 8.9e-03 nm, Epot= -2.04967e+06 Fmax= 5.85646e+03, atom= 851
Step= 1173, Dmax= 1.1e-02 nm, Epot= -2.04969e+06 Fmax= 8.10478e+03, atom= 851
Step= 1174, Dmax= 1.3e-02 nm, Epot= -2.04971e+06 Fmax= 8.71459e+03, atom= 851
Step= 1176, Dmax= 7.7e-03 nm, Epot= -2.04978e+06 Fmax= 1.37984e+03, atom= 851
Step= 1177, Dmax= 9.2e-03 nm, Epot= -2.04983e+06 Fmax= 1.07578e+04, atom= 851
Step= 1178, Dmax= 1.1e-02 nm, Epot= -2.04992e+06 Fmax= 3.75936e+03, atom= 851
Step= 1180, Dmax= 6.6e-03 nm, Epot= -2.04994e+06 Fmax= 4.96643e+03, atom= 851
Step= 1181, Dmax= 8.0e-03 nm, Epot= -2.04997e+06 Fmax= 5.46146e+03, atom= 851
Step= 1182, Dmax= 9.6e-03 nm, Epot= -2.04999e+06 Fmax= 7.09985e+03, atom= 851
Step= 1183, Dmax= 1.1e-02 nm, Epot= -2.05001e+06 Fmax= 7.91521e+03, atom= 851
Step= 1184, Dmax= 1.4e-02 nm, Epot= -2.05002e+06 Fmax= 1.01762e+04, atom= 851
Step= 1185, Dmax= 1.7e-02 nm, Epot= -2.05003e+06 Fmax= 1.14380e+04, atom= 851
Step= 1187, Dmax= 9.9e-03 nm, Epot= -2.05013e+06 Fmax= 1.51881e+03, atom= 851
Step= 1188, Dmax= 1.2e-02 nm, Epot= -2.05016e+06 Fmax= 1.40324e+04, atom= 851
Step= 1189, Dmax= 1.4e-02 nm, Epot= -2.05029e+06 Fmax= 4.66983e+03, atom= 851
Step= 1191, Dmax= 8.6e-03 nm, Epot= -2.05031e+06 Fmax= 6.52575e+03, atom= 851
Step= 1192, Dmax= 1.0e-02 nm, Epot= -2.05033e+06 Fmax= 6.97244e+03, atom= 851
Step= 1193, Dmax= 1.2e-02 nm, Epot= -2.05035e+06 Fmax= 9.15880e+03, atom= 851
Step= 1194, Dmax= 1.5e-02 nm, Epot= -2.05036e+06 Fmax= 1.02808e+04, atom= 851
Step= 1196, Dmax= 8.9e-03 nm, Epot= -2.05044e+06 Fmax= 1.39058e+03, atom= 851
Step= 1197, Dmax= 1.1e-02 nm, Epot= -2.05049e+06 Fmax= 1.26281e+04, atom= 851
Step= 1198, Dmax= 1.3e-02 nm, Epot= -2.05060e+06 Fmax= 4.15155e+03, atom= 851
Step= 1200, Dmax= 7.7e-03 nm, Epot= -2.05062e+06 Fmax= 5.93648e+03, atom= 851
Step= 1201, Dmax= 9.2e-03 nm, Epot= -2.05065e+06 Fmax= 6.11466e+03, atom= 851
Step= 1202, Dmax= 1.1e-02 nm, Epot= -2.05066e+06 Fmax= 8.40360e+03, atom= 851
Step= 1203, Dmax= 1.3e-02 nm, Epot= -2.05068e+06 Fmax= 8.94834e+03, atom= 851
Step= 1205, Dmax= 8.0e-03 nm, Epot= -2.05074e+06 Fmax= 1.45902e+03, atom= 851
Step= 1206, Dmax= 9.6e-03 nm, Epot= -2.05079e+06 Fmax= 1.10113e+04, atom= 851
Step= 1207, Dmax= 1.1e-02 nm, Epot= -2.05088e+06 Fmax= 3.99980e+03, atom= 851
Step= 1209, Dmax= 6.9e-03 nm, Epot= -2.05091e+06 Fmax= 4.99156e+03, atom= 851
Step= 1210, Dmax= 8.3e-03 nm, Epot= -2.05093e+06 Fmax= 5.84091e+03, atom= 851
Step= 1211, Dmax= 9.9e-03 nm, Epot= -2.05095e+06 Fmax= 7.10985e+03, atom= 851
Step= 1212, Dmax= 1.2e-02 nm, Epot= -2.05097e+06 Fmax= 8.49060e+03, atom= 851
Step= 1213, Dmax= 1.4e-02 nm, Epot= -2.05098e+06 Fmax= 1.01539e+04, atom= 851
Step= 1214, Dmax= 1.7e-02 nm, Epot= -2.05098e+06 Fmax= 1.23185e+04, atom= 851
Step= 1216, Dmax= 1.0e-02 nm, Epot= -2.05110e+06 Fmax= 1.17931e+03, atom= 851
Step= 1217, Dmax= 1.2e-02 nm, Epot= -2.05115e+06 Fmax= 1.49961e+04, atom= 851
Step= 1218, Dmax= 1.5e-02 nm, Epot= -2.05129e+06 Fmax= 4.39632e+03, atom= 851
Step= 1220, Dmax= 8.9e-03 nm, Epot= -2.05131e+06 Fmax= 7.28277e+03, atom= 851
Step= 1221, Dmax= 1.1e-02 nm, Epot= -2.05135e+06 Fmax= 6.64377e+03, atom= 851
Step= 1223, Dmax= 6.4e-03 nm, Epot= -2.05139e+06 Fmax= 1.71800e+03, atom= 851
Step= 1224, Dmax= 7.7e-03 nm, Epot= -2.05142e+06 Fmax= 8.28400e+03, atom= 851
Step= 1225, Dmax= 9.2e-03 nm, Epot= -2.05148e+06 Fmax= 3.76566e+03, atom= 851
Step= 1227, Dmax= 5.5e-03 nm, Epot= -2.05151e+06 Fmax= 3.45731e+03, atom= 851
Step= 1228, Dmax= 6.6e-03 nm, Epot= -2.05154e+06 Fmax= 5.23810e+03, atom= 851
Step= 1229, Dmax= 8.0e-03 nm, Epot= -2.05157e+06 Fmax= 5.16023e+03, atom= 851
Step= 1230, Dmax= 9.5e-03 nm, Epot= -2.05158e+06 Fmax= 7.36267e+03, atom= 851
Step= 1231, Dmax= 1.1e-02 nm, Epot= -2.05160e+06 Fmax= 7.60817e+03, atom= 851
Step= 1232, Dmax= 1.4e-02 nm, Epot= -2.05160e+06 Fmax= 1.04279e+04, atom= 851
Step= 1233, Dmax= 1.6e-02 nm, Epot= -2.05162e+06 Fmax= 1.11215e+04, atom= 851
Step= 1235, Dmax= 9.9e-03 nm, Epot= -2.05172e+06 Fmax= 1.79553e+03, atom= 851
Step= 1236, Dmax= 1.2e-02 nm, Epot= -2.05172e+06 Fmax= 1.37038e+04, atom= 851
Step= 1237, Dmax= 1.4e-02 nm, Epot= -2.05185e+06 Fmax= 4.93684e+03, atom= 851
Step= 1239, Dmax= 8.5e-03 nm, Epot= -2.05186e+06 Fmax= 6.23174e+03, atom= 851
Step= 1240, Dmax= 1.0e-02 nm, Epot= -2.05188e+06 Fmax= 7.22344e+03, atom= 851
Step= 1241, Dmax= 1.2e-02 nm, Epot= -2.05189e+06 Fmax= 8.86095e+03, atom= 851
Step= 1242, Dmax= 1.5e-02 nm, Epot= -2.05190e+06 Fmax= 1.05187e+04, atom= 851
Step= 1243, Dmax= 1.8e-02 nm, Epot= -2.05190e+06 Fmax= 1.26336e+04, atom= 851
Step= 1245, Dmax= 1.1e-02 nm, Epot= -2.05202e+06 Fmax= 1.24127e+03, atom= 851
Step= 1246, Dmax= 1.3e-02 nm, Epot= -2.05204e+06 Fmax= 1.54482e+04, atom= 851
Step= 1247, Dmax= 1.5e-02 nm, Epot= -2.05221e+06 Fmax= 4.59528e+03, atom= 851
Step= 1249, Dmax= 9.2e-03 nm, Epot= -2.05222e+06 Fmax= 7.38215e+03, atom= 851
Step= 1250, Dmax= 1.1e-02 nm, Epot= -2.05225e+06 Fmax= 7.07928e+03, atom= 851
Step= 1251, Dmax= 1.3e-02 nm, Epot= -2.05225e+06 Fmax= 1.01985e+04, atom= 851
Step= 1252, Dmax= 1.6e-02 nm, Epot= -2.05227e+06 Fmax= 1.06271e+04, atom= 851
Step= 1254, Dmax= 9.5e-03 nm, Epot= -2.05236e+06 Fmax= 1.87856e+03, atom= 851
Step= 1255, Dmax= 1.1e-02 nm, Epot= -2.05236e+06 Fmax= 1.31402e+04, atom= 851
Step= 1256, Dmax= 1.4e-02 nm, Epot= -2.05247e+06 Fmax= 4.84122e+03, atom= 851
Step= 1258, Dmax= 8.2e-03 nm, Epot= -2.05249e+06 Fmax= 5.95593e+03, atom= 851
Step= 1259, Dmax= 9.9e-03 nm, Epot= -2.05252e+06 Fmax= 6.95573e+03, atom= 851
Step= 1260, Dmax= 1.2e-02 nm, Epot= -2.05253e+06 Fmax= 8.59399e+03, atom= 851
Step= 1261, Dmax= 1.4e-02 nm, Epot= -2.05254e+06 Fmax= 9.99373e+03, atom= 851
Step= 1262, Dmax= 1.7e-02 nm, Epot= -2.05254e+06 Fmax= 1.24067e+04, atom= 851
Step= 1264, Dmax= 1.0e-02 nm, Epot= -2.05265e+06 Fmax= 1.04942e+03, atom= 851
Step= 1265, Dmax= 1.2e-02 nm, Epot= -2.05271e+06 Fmax= 1.50568e+04, atom= 851
Step= 1266, Dmax= 1.5e-02 nm, Epot= -2.05286e+06 Fmax= 4.27165e+03, atom= 851
Step= 1268, Dmax= 8.8e-03 nm, Epot= -2.05288e+06 Fmax= 7.37772e+03, atom= 851
Step= 1269, Dmax= 1.1e-02 nm, Epot= -2.05291e+06 Fmax= 6.50526e+03, atom= 851
Step= 1271, Dmax= 6.4e-03 nm, Epot= -2.05295e+06 Fmax= 1.83022e+03, atom= 851
Step= 1272, Dmax= 7.6e-03 nm, Epot= -2.05299e+06 Fmax= 8.14158e+03, atom= 851
Step= 1273, Dmax= 9.2e-03 nm, Epot= -2.05303e+06 Fmax= 3.86961e+03, atom= 851
Step= 1275, Dmax= 5.5e-03 nm, Epot= -2.05306e+06 Fmax= 3.33205e+03, atom= 851
Step= 1276, Dmax= 6.6e-03 nm, Epot= -2.05308e+06 Fmax= 5.33481e+03, atom= 851
Step= 1277, Dmax= 7.9e-03 nm, Epot= -2.05311e+06 Fmax= 5.03198e+03, atom= 851
Step= 1278, Dmax= 9.5e-03 nm, Epot= -2.05312e+06 Fmax= 7.45035e+03, atom= 851
Step= 1279, Dmax= 1.1e-02 nm, Epot= -2.05315e+06 Fmax= 7.47449e+03, atom= 851
Step= 1280, Dmax= 1.4e-02 nm, Epot= -2.05315e+06 Fmax= 1.05043e+04, atom= 851
Step= 1281, Dmax= 1.6e-02 nm, Epot= -2.05316e+06 Fmax= 1.09786e+04, atom= 851
Step= 1283, Dmax= 9.9e-03 nm, Epot= -2.05326e+06 Fmax= 1.89773e+03, atom= 851
Step= 1285, Dmax= 5.9e-03 nm, Epot= -2.05329e+06 Fmax= 5.85356e+03, atom= 851
Step= 1286, Dmax= 7.1e-03 nm, Epot= -2.05333e+06 Fmax= 3.44779e+03, atom= 851
Step= 1287, Dmax= 8.5e-03 nm, Epot= -2.05334e+06 Fmax= 7.67461e+03, atom= 851
Step= 1288, Dmax= 1.0e-02 nm, Epot= -2.05338e+06 Fmax= 5.72139e+03, atom= 851
Step= 1290, Dmax= 6.1e-03 nm, Epot= -2.05342e+06 Fmax= 2.31578e+03, atom= 851
Step= 1291, Dmax= 7.4e-03 nm, Epot= -2.05344e+06 Fmax= 7.35171e+03, atom= 851
Step= 1292, Dmax= 8.8e-03 nm, Epot= -2.05348e+06 Fmax= 4.21372e+03, atom= 851
Step= 1294, Dmax= 5.3e-03 nm, Epot= -2.05351e+06 Fmax= 2.72934e+03, atom= 851
Step= 1295, Dmax= 6.4e-03 nm, Epot= -2.05354e+06 Fmax= 5.57969e+03, atom= 851
Step= 1296, Dmax= 7.6e-03 nm, Epot= -2.05357e+06 Fmax= 4.42303e+03, atom= 851
Step= 1297, Dmax= 9.2e-03 nm, Epot= -2.05358e+06 Fmax= 7.53977e+03, atom= 851
Step= 1298, Dmax= 1.1e-02 nm, Epot= -2.05361e+06 Fmax= 6.86736e+03, atom= 851
Step= 1300, Dmax= 6.6e-03 nm, Epot= -2.05365e+06 Fmax= 1.77789e+03, atom= 851
Step= 1301, Dmax= 7.9e-03 nm, Epot= -2.05369e+06 Fmax= 8.62033e+03, atom= 851
Step= 1302, Dmax= 9.5e-03 nm, Epot= -2.05374e+06 Fmax= 3.81770e+03, atom= 851
Step= 1304, Dmax= 5.7e-03 nm, Epot= -2.05376e+06 Fmax= 3.65146e+03, atom= 851
Step= 1305, Dmax= 6.8e-03 nm, Epot= -2.05379e+06 Fmax= 5.28439e+03, atom= 851
Step= 1306, Dmax= 8.2e-03 nm, Epot= -2.05381e+06 Fmax= 5.47370e+03, atom= 851
Step= 1307, Dmax= 9.8e-03 nm, Epot= -2.05383e+06 Fmax= 7.39236e+03, atom= 851
Step= 1308, Dmax= 1.2e-02 nm, Epot= -2.05385e+06 Fmax= 8.10304e+03, atom= 851
Step= 1309, Dmax= 1.4e-02 nm, Epot= -2.05386e+06 Fmax= 1.04189e+04, atom= 851
Step= 1310, Dmax= 1.7e-02 nm, Epot= -2.05386e+06 Fmax= 1.19034e+04, atom= 851
Step= 1312, Dmax= 1.0e-02 nm, Epot= -2.05396e+06 Fmax= 1.50508e+03, atom= 851
Step= 1313, Dmax= 1.2e-02 nm, Epot= -2.05397e+06 Fmax= 1.45733e+04, atom= 851
Step= 1314, Dmax= 1.5e-02 nm, Epot= -2.05410e+06 Fmax= 4.69688e+03, atom= 851
Step= 1316, Dmax= 8.8e-03 nm, Epot= -2.05412e+06 Fmax= 6.88881e+03, atom= 851
Step= 1317, Dmax= 1.1e-02 nm, Epot= -2.05414e+06 Fmax= 6.94803e+03, atom= 851
Step= 1318, Dmax= 1.3e-02 nm, Epot= -2.05414e+06 Fmax= 9.72232e+03, atom= 851
Step= 1319, Dmax= 1.5e-02 nm, Epot= -2.05416e+06 Fmax= 1.01993e+04, atom= 851
Step= 1321, Dmax= 9.1e-03 nm, Epot= -2.05424e+06 Fmax= 1.74309e+03, atom= 851
Step= 1322, Dmax= 1.1e-02 nm, Epot= -2.05425e+06 Fmax= 1.25849e+04, atom= 851
Step= 1323, Dmax= 1.3e-02 nm, Epot= -2.05435e+06 Fmax= 4.64483e+03, atom= 851
Step= 1325, Dmax= 7.9e-03 nm, Epot= -2.05437e+06 Fmax= 5.68166e+03, atom= 851
Step= 1326, Dmax= 9.5e-03 nm, Epot= -2.05440e+06 Fmax= 6.75344e+03, atom= 851
Step= 1327, Dmax= 1.1e-02 nm, Epot= -2.05441e+06 Fmax= 8.11660e+03, atom= 851
Step= 1328, Dmax= 1.4e-02 nm, Epot= -2.05442e+06 Fmax= 9.79452e+03, atom= 851
Step= 1329, Dmax= 1.6e-02 nm, Epot= -2.05442e+06 Fmax= 1.16097e+04, atom= 851
Step= 1331, Dmax= 9.8e-03 nm, Epot= -2.05452e+06 Fmax= 1.21918e+03, atom= 851
Step= 1332, Dmax= 1.2e-02 nm, Epot= -2.05455e+06 Fmax= 1.42037e+04, atom= 851
Step= 1333, Dmax= 1.4e-02 nm, Epot= -2.05468e+06 Fmax= 4.32153e+03, atom= 851
Step= 1335, Dmax= 8.5e-03 nm, Epot= -2.05470e+06 Fmax= 6.75616e+03, atom= 851
Step= 1336, Dmax= 1.0e-02 nm, Epot= -2.05473e+06 Fmax= 6.60946e+03, atom= 851
Step= 1337, Dmax= 1.2e-02 nm, Epot= -2.05474e+06 Fmax= 9.36426e+03, atom= 851
Step= 1338, Dmax= 1.5e-02 nm, Epot= -2.05475e+06 Fmax= 9.88353e+03, atom= 851
Step= 1340, Dmax= 8.8e-03 nm, Epot= -2.05482e+06 Fmax= 1.67353e+03, atom= 851
Step= 1341, Dmax= 1.1e-02 nm, Epot= -2.05483e+06 Fmax= 1.22051e+04, atom= 851
Step= 1342, Dmax= 1.3e-02 nm, Epot= -2.05493e+06 Fmax= 4.41339e+03, atom= 851
Step= 1344, Dmax= 7.6e-03 nm, Epot= -2.05495e+06 Fmax= 5.56710e+03, atom= 851
Step= 1345, Dmax= 9.1e-03 nm, Epot= -2.05497e+06 Fmax= 6.36866e+03, atom= 851
Step= 1346, Dmax= 1.1e-02 nm, Epot= -2.05498e+06 Fmax= 8.00319e+03, atom= 851
Step= 1347, Dmax= 1.3e-02 nm, Epot= -2.05499e+06 Fmax= 9.17975e+03, atom= 851
Step= 1348, Dmax= 1.6e-02 nm, Epot= -2.05500e+06 Fmax= 1.15225e+04, atom= 851
Step= 1350, Dmax= 9.5e-03 nm, Epot= -2.05509e+06 Fmax= 9.11724e+02, atom= 851

writing lowest energy coordinates.

Steepest Descents converged to Fmax < 1000 in 1351 steps
Potential Energy  = -2.0550941e+06
Maximum force     =  9.1172430e+02 on atom 851
Norm of force     =  1.2023874e+01

GROMACS reminds you: "The best way to obtain plausible negative examples is to run a docking program with a biophysics-based function." (Julie Bernauer)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx energy -f minimization.edr -o potential1.xvg
                       :-) GROMACS - gmx energy, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx energy -f minimization.edr -o potential1.xvg

Opened minimization.edr as single precision energy file

Select the terms you want from the following list by
selecting either (part of) the name or the number or a combination.
End your selection with an empty line or a zero.
-------------------------------------------------------------------
  1  Bond             2  U-B              3  Proper-Dih.      4  Improper-Dih. 
  5  CMAP-Dih.        6  LJ-14            7  Coulomb-14       8  LJ-(SR)       
  9  Coulomb-(SR)    10  Coul.-recip.    11  Position-Rest.  12  Potential     
 13  Pressure        14  Constr.-rmsd    15  Vir-XX          16  Vir-XY        
 17  Vir-XZ          18  Vir-YX          19  Vir-YY          20  Vir-YZ        
 21  Vir-ZX          22  Vir-ZY          23  Vir-ZZ          24  Pres-XX       
 25  Pres-XY         26  Pres-XZ         27  Pres-YX         28  Pres-YY       
 29  Pres-YZ         30  Pres-ZX         31  Pres-ZY         32  Pres-ZZ       
 33  #Surf*SurfTen   34  T-rest        

10 0
Last energy frame read 1069 time 1350.000         

Statistics over 1351 steps [ 0.0000 through 1350.0000 ps ], 1 data sets
All statistics are over 1070 points (frames)

Energy                      Average   Err.Est.       RMSD  Tot-Drift
-------------------------------------------------------------------------------
Coul. recip.                7260.04        490    1058.27    -3282.1  (kJ/mol)

GROMACS reminds you: "It seemed a good idea at first" (Gerrit Groenhof)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ ng

Command 'ng' not found, but can be installed with:

sudo apt install ng-common

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx energy -f minimization.edr -o potential.xvg -xvg none
                       :-) GROMACS - gmx energy, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx energy -f minimization.edr -o potential.xvg -xvg none

Opened minimization.edr as single precision energy file

Select the terms you want from the following list by
selecting either (part of) the name or the number or a combination.
End your selection with an empty line or a zero.
-------------------------------------------------------------------
  1  Bond             2  U-B              3  Proper-Dih.      4  Improper-Dih. 
  5  CMAP-Dih.        6  LJ-14            7  Coulomb-14       8  LJ-(SR)       
  9  Coulomb-(SR)    10  Coul.-recip.    11  Position-Rest.  12  Potential     
 13  Pressure        14  Constr.-rmsd    15  Vir-XX          16  Vir-XY        
 17  Vir-XZ          18  Vir-YX          19  Vir-YY          20  Vir-YZ        
 21  Vir-ZX          22  Vir-ZY          23  Vir-ZZ          24  Pres-XX       
 25  Pres-XY         26  Pres-XZ         27  Pres-YX         28  Pres-YY       
 29  Pres-YZ         30  Pres-ZX         31  Pres-ZY         32  Pres-ZZ       
 33  #Surf*SurfTen   34  T-rest        

10 0
Last energy frame read 1069 time 1350.000         

Statistics over 1351 steps [ 0.0000 through 1350.0000 ps ], 1 data sets
All statistics are over 1070 points (frames)

Energy                      Average   Err.Est.       RMSD  Tot-Drift
-------------------------------------------------------------------------------
Coul. recip.                7260.04        490    1058.27    -3282.1  (kJ/mol)

GROMACS reminds you: "Dreams seldom materialize on their own." (Dian Fossey)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx grompp -f step4.1_equilibration.mdp -o step4.1_equilibration.tpr -c minimization.gro -r step3_input.gro -p topol.top -n index.ndx
                       :-) GROMACS - gmx grompp, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx grompp -f step4.1_equilibration.mdp -o step4.1_equilibration.tpr -c minimization.gro -r step3_input.gro -p topol.top -n index.ndx

Replacing old mdp entry 'nstxtcout' by 'nstxout-compressed'

NOTE 1 [file step4.1_equilibration.mdp]:
  leapfrog does not yet support Nose-Hoover chains, nhchainlength reset to
  1

Setting the LD random seed to -1695613009

Generated 627 of the 630 non-bonded parameter combinations
Generating 1-4 interactions: fudge = 1

Generated 325 of the 630 1-4 parameter combinations

Excluding 3 bonded neighbours molecule type 'PROA'

turning H bonds into constraints...

Excluding 1 bonded neighbours molecule type 'POT'

turning H bonds into constraints...

Excluding 1 bonded neighbours molecule type 'CLA'

turning H bonds into constraints...

Excluding 2 bonded neighbours molecule type 'TIP3'

turning H bonds into constraints...

Setting gen_seed to -277487635

Velocities were taken from a Maxwell distribution at 303.15 K
Number of degrees of freedom in T-Coupling group SOLU is 3456.00
Number of degrees of freedom in T-Coupling group SOLV is 240870.00

The largest distance between excluded atoms is 0.400 nm between atom 917 and 925

Determining Verlet buffer for a tolerance of 0.005 kJ/mol/ps at 303.15 K

Calculated rlist for 1x1 atom pair-list as 1.238 nm, buffer size 0.038 nm

Set rlist, assuming 4x4 atom pair-list, to 1.200 nm, buffer size 0.000 nm

Note that mdrun will redetermine rlist based on the actual pair-list setup

NOTE 2 [file step4.1_equilibration.mdp]:
  Removing center of mass motion in the presence of position restraints
  might cause artifacts. When you are using position restraints to
  equilibrate a macro-molecule, the artifacts are usually negligible.

Calculating fourier grid dimensions for X Y Z
Using a fourier grid of 96x96x96, spacing 0.114 0.114 0.114

Estimate for the relative computational load of the PME mesh part: 0.06

This run will generate roughly 97 Mb of data

There were 2 NOTEs

GROMACS reminds you: "I am at two with nature." (Woody Allen)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx mdrun -deffnm step4.1_equilibration
                       :-) GROMACS - gmx mdrun, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx mdrun -deffnm step4.1_equilibration

Compiled SIMD: None, but for this host/run AVX2_256 might be better (see log).
Reading file step4.1_equilibration.tpr, VERSION 2023 (single precision)
Changing nstlist from 20 to 100, rlist from 1.2 to 1.298

1 GPU selected for this run.
Mapping of GPU IDs to the 2 GPU tasks in the 1 rank on this node:
  PP:0,PME:0
PP tasks will do (non-perturbed) short-ranged interactions on the GPU
PP task will update and constrain coordinates on the CPU
PME tasks will do all aspects on the GPU
Using 1 MPI thread
Using 16 OpenMP threads 

starting mdrun 'Title'
125000 steps,    125.0 ps.

Writing final coordinates.

               Core t (s)   Wall t (s)        (%)
       Time:     3800.837      237.554     1600.0
                 (ns/day)    (hour/ns)
Performance:       45.464        0.528

GROMACS reminds you: "I Caught It In the Face" (P.J. Harvey)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx energy -f nvt.edr -o temperature.xvg
                       :-) GROMACS - gmx energy, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx energy -f nvt.edr -o temperature.xvg


-------------------------------------------------------
Program:     gmx energy, version 2023
Source file: src/gromacs/commandline/cmdlineparser.cpp (line 271)
Function:    void gmx::CommandLineParser::parse(int*, char**)

Error in user input:
Invalid command-line options
  In command-line option -f
    File 'nvt.edr' does not exist or is not accessible.
    The file could not be opened.
      Reason: No such file or directory
      (call to fopen() returned error code 2)

For more information and tips for troubleshooting, please check the GROMACS
website at http://www.gromacs.org/Documentation/Errors
-------------------------------------------------------
student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx energy -f step4.1_equilibration.edr -o temperature.xvg
                       :-) GROMACS - gmx energy, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx energy -f step4.1_equilibration.edr -o temperature.xvg

Opened step4.1_equilibration.edr as single precision energy file

Select the terms you want from the following list by
selecting either (part of) the name or the number or a combination.
End your selection with an empty line or a zero.
-------------------------------------------------------------------
  1  Bond             2  U-B              3  Proper-Dih.      4  Improper-Dih. 
  5  CMAP-Dih.        6  LJ-14            7  Coulomb-14       8  LJ-(SR)       
  9  Coulomb-(SR)    10  Coul.-recip.    11  Position-Rest.  12  Potential     
 13  Kinetic-En.     14  Total-Energy    15  Conserved-En.   16  Temperature   
 17  Pressure        18  Constr.-rmsd    19  Vir-XX          20  Vir-XY        
 21  Vir-XZ          22  Vir-YX          23  Vir-YY          24  Vir-YZ        
 25  Vir-ZX          26  Vir-ZY          27  Vir-ZZ          28  Pres-XX       
 29  Pres-XY         30  Pres-XZ         31  Pres-YX         32  Pres-YY       
 33  Pres-YZ         34  Pres-ZX         35  Pres-ZY         36  Pres-ZZ       
 37  #Surf*SurfTen   38  T-SOLU          39  T-SOLV        

16 0
Last energy frame read 125 time  125.000          

Statistics over 125001 steps [ 0.0000 through 125.0000 ps ], 1 data sets
All statistics are over 1251 points

Energy                      Average   Err.Est.       RMSD  Tot-Drift
-------------------------------------------------------------------------------
Temperature                 303.165       0.03    12.4684  -0.187904  (K)

GROMACS reminds you: "I ought to warn you, I have no faith" (Jane Eyre in Jane Eyre by Charlotte Bronte)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx grompp -f step4.1_equilibration.mdp -o step4.2equilibration_NPT.tpr -c step4.1_equilibration.gro -r step3_input.gro -p topol.top -n index.ndx
                       :-) GROMACS - gmx grompp, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx grompp -f step4.1_equilibration.mdp -o step4.2equilibration_NPT.tpr -c step4.1_equilibration.gro -r step3_input.gro -p topol.top -n index.ndx

Replacing old mdp entry 'nstxtcout' by 'nstxout-compressed'

NOTE 1 [file step4.1_equilibration.mdp]:
  leapfrog does not yet support Nose-Hoover chains, nhchainlength reset to
  1

Setting the LD random seed to -369166419

Generated 627 of the 630 non-bonded parameter combinations
Generating 1-4 interactions: fudge = 1

Generated 325 of the 630 1-4 parameter combinations

Excluding 3 bonded neighbours molecule type 'PROA'

turning H bonds into constraints...

Excluding 1 bonded neighbours molecule type 'POT'

turning H bonds into constraints...

Excluding 1 bonded neighbours molecule type 'CLA'

turning H bonds into constraints...

Excluding 2 bonded neighbours molecule type 'TIP3'

turning H bonds into constraints...

Setting gen_seed to -94376351

Velocities were taken from a Maxwell distribution at 303.15 K
Number of degrees of freedom in T-Coupling group SOLU is 3456.00
Number of degrees of freedom in T-Coupling group SOLV is 240870.00

The largest distance between excluded atoms is 0.416 nm between atom 100 and 108

Determining Verlet buffer for a tolerance of 0.005 kJ/mol/ps at 303.15 K

Calculated rlist for 1x1 atom pair-list as 1.238 nm, buffer size 0.038 nm

Set rlist, assuming 4x4 atom pair-list, to 1.200 nm, buffer size 0.000 nm

Note that mdrun will redetermine rlist based on the actual pair-list setup

NOTE 2 [file step4.1_equilibration.mdp]:
  Removing center of mass motion in the presence of position restraints
  might cause artifacts. When you are using position restraints to
  equilibrate a macro-molecule, the artifacts are usually negligible.

Calculating fourier grid dimensions for X Y Z
Using a fourier grid of 96x96x96, spacing 0.114 0.114 0.114

Estimate for the relative computational load of the PME mesh part: 0.06

This run will generate roughly 97 Mb of data

There were 2 NOTEs

GROMACS reminds you: "The more clearly we can focus our attention on the wonders and realities of the universe about us, the less taste we shall have for destruction." (Rachel Carson)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx mdrun -v -deffnm step4.2equilibration_NPT
                       :-) GROMACS - gmx mdrun, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx mdrun -v -deffnm step4.2equilibration_NPT

Compiled SIMD: None, but for this host/run AVX2_256 might be better (see log).
Reading file step4.2equilibration_NPT.tpr, VERSION 2023 (single precision)
Changing nstlist from 20 to 100, rlist from 1.2 to 1.298

1 GPU selected for this run.
Mapping of GPU IDs to the 2 GPU tasks in the 1 rank on this node:
  PP:0,PME:0
PP tasks will do (non-perturbed) short-ranged interactions on the GPU
PP task will update and constrain coordinates on the CPU
PME tasks will do all aspects on the GPU
Using 1 MPI thread
Using 16 OpenMP threads 

starting mdrun 'Title'
125000 steps,    125.0 ps.
step 2700: timed with pme grid 96 96 96, coulomb cutoff 1.200: 745.1 M-cycles
step 2900: timed with pme grid 80 80 80, coulomb cutoff 1.363: 764.6 M-cycles
step 3100: timed with pme grid 72 72 72, coulomb cutoff 1.514: 861.7 M-cycles
step 3300: timed with pme grid 80 80 80, coulomb cutoff 1.363: 769.9 M-cycles
step 3500: timed with pme grid 84 84 84, coulomb cutoff 1.298: 735.9 M-cycles
step 3700: timed with pme grid 96 96 96, coulomb cutoff 1.200: 679.6 M-cycles
step 3900: timed with pme grid 84 84 84, coulomb cutoff 1.298: 731.8 M-cycles
step 4100: timed with pme grid 96 96 96, coulomb cutoff 1.200: 677.0 M-cycles
              optimal pme grid 96 96 96, coulomb cutoff 1.200
step 124900, remaining wall clock time:     0 s          
Writing final coordinates.
step 125000, remaining wall clock time:     0 s          
               Core t (s)   Wall t (s)        (%)
       Time:     3953.547      247.099     1600.0
                 (ns/day)    (hour/ns)
Performance:       43.707        0.549

GROMACS reminds you: "Your Bones Got a Little Machine" (Pixies)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx energy -f step4.2equilibration_NPT.edr -o pressure.xvg
                       :-) GROMACS - gmx energy, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx energy -f step4.2equilibration_NPT.edr -o pressure.xvg

Opened step4.2equilibration_NPT.edr as single precision energy file

Select the terms you want from the following list by
selecting either (part of) the name or the number or a combination.
End your selection with an empty line or a zero.
-------------------------------------------------------------------
  1  Bond             2  U-B              3  Proper-Dih.      4  Improper-Dih. 
  5  CMAP-Dih.        6  LJ-14            7  Coulomb-14       8  LJ-(SR)       
  9  Coulomb-(SR)    10  Coul.-recip.    11  Position-Rest.  12  Potential     
 13  Kinetic-En.     14  Total-Energy    15  Conserved-En.   16  Temperature   
 17  Pressure        18  Constr.-rmsd    19  Vir-XX          20  Vir-XY        
 21  Vir-XZ          22  Vir-YX          23  Vir-YY          24  Vir-YZ        
 25  Vir-ZX          26  Vir-ZY          27  Vir-ZZ          28  Pres-XX       
 29  Pres-XY         30  Pres-XZ         31  Pres-YX         32  Pres-YY       
 33  Pres-YZ         34  Pres-ZX         35  Pres-ZY         36  Pres-ZZ       
 37  #Surf*SurfTen   38  T-SOLU          39  T-SOLV        

17 0
Last energy frame read 125 time  125.000          

Statistics over 125001 steps [ 0.0000 through 125.0000 ps ], 1 data sets
All statistics are over 1251 points

Energy                      Average   Err.Est.       RMSD  Tot-Drift
-------------------------------------------------------------------------------
Pressure                   -998.138        3.8    60.2939    -5.1007  (bar)

GROMACS reminds you: "Be less curious about people and more curious about ideas." (Marie Curie)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx energy -f step4.2equilibration_NPT.edr -o pressure1.xvg
                       :-) GROMACS - gmx energy, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx energy -f step4.2equilibration_NPT.edr -o pressure1.xvg

Opened step4.2equilibration_NPT.edr as single precision energy file

Select the terms you want from the following list by
selecting either (part of) the name or the number or a combination.
End your selection with an empty line or a zero.
-------------------------------------------------------------------
  1  Bond             2  U-B              3  Proper-Dih.      4  Improper-Dih. 
  5  CMAP-Dih.        6  LJ-14            7  Coulomb-14       8  LJ-(SR)       
  9  Coulomb-(SR)    10  Coul.-recip.    11  Position-Rest.  12  Potential     
 13  Kinetic-En.     14  Total-Energy    15  Conserved-En.   16  Temperature   
 17  Pressure        18  Constr.-rmsd    19  Vir-XX          20  Vir-XY        
 21  Vir-XZ          22  Vir-YX          23  Vir-YY          24  Vir-YZ        
 25  Vir-ZX          26  Vir-ZY          27  Vir-ZZ          28  Pres-XX       
 29  Pres-XY         30  Pres-XZ         31  Pres-YX         32  Pres-YY       
 33  Pres-YZ         34  Pres-ZX         35  Pres-ZY         36  Pres-ZZ       
 37  #Surf*SurfTen   38  T-SOLU          39  T-SOLV        

18 0
Last energy frame read 125 time  125.000          

Statistics over 125001 steps [ 0.0000 through 125.0000 ps ], 1 data sets
All statistics are over 1251 points

Energy                      Average   Err.Est.       RMSD  Tot-Drift
-------------------------------------------------------------------------------
Constr. rmsd             1.76753e-09    1.8e-09 6.24915e-08 -1.05805e-08  ()

GROMACS reminds you: "Don't Grumble, Give a Whistle !" (Monty Python)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx energy -f step4.2equilibration_NPT.edr -o density.xvg
                       :-) GROMACS - gmx energy, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx energy -f step4.2equilibration_NPT.edr -o density.xvg

Opened step4.2equilibration_NPT.edr as single precision energy file

Select the terms you want from the following list by
selecting either (part of) the name or the number or a combination.
End your selection with an empty line or a zero.
-------------------------------------------------------------------
  1  Bond             2  U-B              3  Proper-Dih.      4  Improper-Dih. 
  5  CMAP-Dih.        6  LJ-14            7  Coulomb-14       8  LJ-(SR)       
  9  Coulomb-(SR)    10  Coul.-recip.    11  Position-Rest.  12  Potential     
 13  Kinetic-En.     14  Total-Energy    15  Conserved-En.   16  Temperature   
 17  Pressure        18  Constr.-rmsd    19  Vir-XX          20  Vir-XY        
 21  Vir-XZ          22  Vir-YX          23  Vir-YY          24  Vir-YZ        
 25  Vir-ZX          26  Vir-ZY          27  Vir-ZZ          28  Pres-XX       
 29  Pres-XY         30  Pres-XZ         31  Pres-YX         32  Pres-YY       
 33  Pres-YZ         34  Pres-ZX         35  Pres-ZY         36  Pres-ZZ       
 37  #Surf*SurfTen   38  T-SOLU          39  T-SOLV        

24 0
Last energy frame read 125 time  125.000          

Statistics over 125001 steps [ 0.0000 through 125.0000 ps ], 1 data sets
All statistics are over 1251 points

Energy                      Average   Err.Est.       RMSD  Tot-Drift
-------------------------------------------------------------------------------
Vir-YZ                      58.0113         31     2108.2    160.615  (kJ/mol)

GROMACS reminds you: "GROMACS First : Making MD Great Again" (Vedran Miletic)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx energy -f step4.2equilibration_NPT.edr -o density.xvg
                       :-) GROMACS - gmx energy, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx energy -f step4.2equilibration_NPT.edr -o density.xvg

Opened step4.2equilibration_NPT.edr as single precision energy file

Select the terms you want from the following list by
selecting either (part of) the name or the number or a combination.
End your selection with an empty line or a zero.
-------------------------------------------------------------------
  1  Bond             2  U-B              3  Proper-Dih.      4  Improper-Dih. 
  5  CMAP-Dih.        6  LJ-14            7  Coulomb-14       8  LJ-(SR)       
  9  Coulomb-(SR)    10  Coul.-recip.    11  Position-Rest.  12  Potential     
 13  Kinetic-En.     14  Total-Energy    15  Conserved-En.   16  Temperature   
 17  Pressure        18  Constr.-rmsd    19  Vir-XX          20  Vir-XY        
 21  Vir-XZ          22  Vir-YX          23  Vir-YY          24  Vir-YZ        
 25  Vir-ZX          26  Vir-ZY          27  Vir-ZZ          28  Pres-XX       
 29  Pres-XY         30  Pres-XZ         31  Pres-YX         32  Pres-YY       
 33  Pres-YZ         34  Pres-ZX         35  Pres-ZY         36  Pres-ZZ       
 37  #Surf*SurfTen   38  T-SOLU          39  T-SOLV        

15 0
Last energy frame read 125 time  125.000          

Statistics over 125001 steps [ 0.0000 through 125.0000 ps ], 1 data sets
All statistics are over 1251 points

Energy                      Average   Err.Est.       RMSD  Tot-Drift
-------------------------------------------------------------------------------
Conserved En.            -1.39516e+06        120     368.16    820.156  (kJ/mol)

GROMACS reminds you: "Aber wenn der Quarterback kommt, um dir die Brille abzunehmen, sag ihm: Danke, die bleibt wo sie ist" (Wir sind Helden)
student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx grompp -f step5_production.mdp -o step5_production.tpr -c step4.2equilibration_NPT.gro -t step4.2equilibration_NPT.cpt -p topol.top -n index.ndx
                       :-) GROMACS - gmx grompp, 2023 (-:p4.cpt -p topol.top -n index.ndx

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx grompp -f step5_production.mdp -o step5_production.tpr -c step4.2equilibration_NPT.gro -t step4.2equilibration_NPT.cpt -p topol.top -n index.ndx

Replacing old mdp entry 'nstxtcout' by 'nstxout-compressed'

NOTE 1 [file step5_production.mdp]:
  leapfrog does not yet support Nose-Hoover chains, nhchainlength reset to
  1

Setting the LD random seed to -857744449

Generated 627 of the 630 non-bonded parameter combinations
Generating 1-4 interactions: fudge = 1

Generated 325 of the 630 1-4 parameter combinations

Excluding 3 bonded neighbours molecule type 'PROA'

turning H bonds into constraints...

Excluding 1 bonded neighbours molecule type 'POT'

turning H bonds into constraints...

Excluding 1 bonded neighbours molecule type 'CLA'

turning H bonds into constraints...

Excluding 2 bonded neighbours molecule type 'TIP3'

turning H bonds into constraints...
Number of degrees of freedom in T-Coupling group SOLU is 3456.00
Number of degrees of freedom in T-Coupling group SOLV is 240870.00

The largest distance between excluded atoms is 0.412 nm between atom 483 and 491

Determining Verlet buffer for a tolerance of 0.005 kJ/mol/ps at 303.15 K

Calculated rlist for 1x1 atom pair-list as 1.296 nm, buffer size 0.096 nm

Set rlist, assuming 4x4 atom pair-list, to 1.223 nm, buffer size 0.023 nm

Note that mdrun will redetermine rlist based on the actual pair-list setup

Reading Coordinates, Velocities and Box size from old trajectory

Will read whole trajectory
Last frame         -1 time  125.000   

Using frame at t = 125 ps

Starting time for run is 0 ps
Calculating fourier grid dimensions for X Y Z
Using a fourier grid of 96x96x96, spacing 0.114 0.114 0.114

Estimate for the relative computational load of the PME mesh part: 0.06

This run will generate roughly 48 Mb of data

There was 1 NOTE

GROMACS reminds you: "Marie, you're looking more radiant every day!" (Pierre Curie)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx grompp -f step5_production.mdp -o step5_production.tpr -c step4.2equilibration_NPT.gro -t step4.2equilibration_NPT.cpt -p topol.top -n index.ndx
                       :-) GROMACS - gmx grompp, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx grompp -f step5_production.mdp -o step5_production.tpr -c step4.2equilibration_NPT.gro -t step4.2equilibration_NPT.cpt -p topol.top -n index.ndx

Replacing old mdp entry 'nstxtcout' by 'nstxout-compressed'

NOTE 1 [file step5_production.mdp]:
  leapfrog does not yet support Nose-Hoover chains, nhchainlength reset to
  1

Setting the LD random seed to -352321709

Generated 627 of the 630 non-bonded parameter combinations
Generating 1-4 interactions: fudge = 1

Generated 325 of the 630 1-4 parameter combinations

Excluding 3 bonded neighbours molecule type 'PROA'

turning H bonds into constraints...

Excluding 1 bonded neighbours molecule type 'POT'

turning H bonds into constraints...

Excluding 1 bonded neighbours molecule type 'CLA'

turning H bonds into constraints...

Excluding 2 bonded neighbours molecule type 'TIP3'

turning H bonds into constraints...
Number of degrees of freedom in T-Coupling group SOLU is 3456.00
Number of degrees of freedom in T-Coupling group SOLV is 240870.00

The largest distance between excluded atoms is 0.412 nm between atom 483 and 491

Determining Verlet buffer for a tolerance of 0.005 kJ/mol/ps at 303.15 K

Calculated rlist for 1x1 atom pair-list as 1.296 nm, buffer size 0.096 nm

Set rlist, assuming 4x4 atom pair-list, to 1.223 nm, buffer size 0.023 nm

Note that mdrun will redetermine rlist based on the actual pair-list setup

Reading Coordinates, Velocities and Box size from old trajectory

Will read whole trajectory
Last frame         -1 time  125.000   

Using frame at t = 125 ps

Starting time for run is 0 ps
Calculating fourier grid dimensions for X Y Z
Using a fourier grid of 96x96x96, spacing 0.114 0.114 0.114

Estimate for the relative computational load of the PME mesh part: 0.06

NOTE 2 [file step5_production.mdp]:
  This run will generate roughly 3576 Mb of data


There were 2 NOTEs

Back Off! I just backed up step5_production.tpr to ./#step5_production.tpr.1#

GROMACS reminds you: "Three Little Fonzies" (Pulp Fiction)

student@manipal2:~/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs$ gmx mdrun -deffnm step5_production -nb gpu
                       :-) GROMACS - gmx mdrun, 2023 (-:

Executable:   /usr/local/gromacs/bin/gmx
Data prefix:  /usr/local/gromacs
Working dir:  /home/student/Downloads/GURPREET/MYC/19.01.2024/charmm-gui-0564969315/gromacs
Command line:
  gmx mdrun -deffnm step5_production -nb gpu

Compiled SIMD: None, but for this host/run AVX2_256 might be better (see log).
Reading file step5_production.tpr, VERSION 2023 (single precision)
Changing nstlist from 20 to 100, rlist from 1.223 to 1.343

1 GPU selected for this run.
Mapping of GPU IDs to the 2 GPU tasks in the 1 rank on this node:
  PP:0,PME:0
PP tasks will do (non-perturbed) short-ranged interactions on the GPU
PP task will update and constrain coordinates on the CPU
PME tasks will do all aspects on the GPU
Using 1 MPI thread
Using 16 OpenMP threads 


WARNING: This run will generate roughly 3479 Mb of data

starting mdrun 'Title'
50000000 steps, 100000.0 ps.
