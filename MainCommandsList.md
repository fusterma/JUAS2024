# Main commands list
**N. Fuster-Marti­nez, G. Sterbini, D. Gamba, S. Kostoglou, J. Olivares** 

## MAD-X commands

	mb : sbend, angle = ??, l = ??; 
	mb1 : mb, at = ??; 
	
	match, sequence = ??;
	global, q1 = ??;
	global, q2 = ??;
	vary, name = ??, step = 0.00001;
	vary, name = ??, step = 0.00001;
	lmdif, call = 50, tolerances = 1e-6;
	endmatch;
	
	track, dump, file = name, deltap = ??;
	start, x = ??, px = ?? , y = ??, py = ??;
	start, x = ??, px = ?? , y = ??, py = ??;
	run, turns = 100;
	
	match, sequence = ??;
	constraint, range = #e, betx = ??;
	constraint, range = #e, alfx = ??;
	vary, name = ??, step = 0.00001;
	vary, name = ??, step = 0.00001;
	lmdif, call = 50, tolerances = 1e-6;
	endmatch;
	
	twiss, sequence = name, betx = ??, alfx = ??, bety = ??, alfy = ??;
	
	
## Cpymad library commands
	
	from cpymad.madx import MadX
	
	madx = Madx()
	
	madx.call('name_of_the_file.madx')
	
	madx.table.twiss.dframe()
	madx.table.sum.dframe()
	
	madx.input('MAD-X command')
	
	
## Python


#### Plot example code ##


	#### To change the size of the plot window
	# plt.rcParams['figure.dpi'] = 100

	#### Plot command
	# plt.plot(x,y,'ob',label='Example')

	#### Adding labels
	# plt.xlabel('s[m]')
	# plt.ylabel('[m]')
	
	#### Adding a legend
	# plt.legend(loc='best')


		
		
