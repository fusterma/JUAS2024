# Main commands list
**N. Fuster-Marti­nez, G. Sterbini, D. Gamba, S. Kostoglou, J. Olivares** 

## MAD-X commands

Lattice elements definition:
    mb : sbend, angle = ??, l = ??; 
    mq : quadrupole, k1 = ??, l = ??;
    ms : sextupole, k2 = ??, l = ??;

Sequence definition:

   

  match, sequence = ??;
  
  global, q1 = ??;
  
  global, q2 = ??;
  
  vary, name = ??, step = 0.00001;
  
  vary, name = ??, step = 0.00001;
  
  lmdif, call = 50, tolerance = 1e-6;
  
  endmatch;


