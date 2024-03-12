### Calmodulin Metadynamics Project

Molecular dynamics (MD) is a crucial tool in computational chemistry for simulating the time evolution of molecular systems across different levels of accuracy, from quantum simulations to atomistic models with empirically parameterized force fields. Despite its capabilities, MD traditionally faces limitations in capturing transitions between molecular states due to the short timescales of these events and difficulties in observing protein structures directly. This limitation restricts the study of longer-term phenomena like chemical reactions, protein folding, and aggregation through standard MD simulations, which typically cover timescales from picoseconds to microseconds.

To overcome these challenges, researchers have developed algorithms that enhance MD simulations, allowing for the study of events on longer timescales. These methods include techniques that increase the system's temperature, such as parallel tempering, and those that use predefined knowledge of transitions to focus the simulation, like umbrella sampling and metadynamics. Employing these advanced algorithms requires additional post-processing to accurately interpret the accelerated data.

Among these innovative approaches, well-tempered metadynamics is one technique I'm currently utilizing. It represents a sophisticated strategy to expedite MD simulations, facilitating the exploration of complex molecular phenomena by effectively sampling the energy landscape and accelerating the discovery of transitional states.

Our MD simulation results revealed high energy barriers between different states of calmodulin (CaM). To better understand the energy landscape of CaM, we employed well-tempered metadynamics. To accurately represent the switch between open and closed conformations, we defined two degrees of freedom as collective variables. 
- The distance between between linker regions of CaM,
- The dihedral angle, which necessitated the definition of four points: the Center of Mass of the N-lobe, the Center of Mass of the C-lobe, alongside the beginning and end points of the helical linker region in CaM.

We obtained 4 different structure of CaM from MD simulations. Each structure belongs to different systems: 
- To stimulate apo form of CaM, we removed calcium ions from the structure.(Now we have holo and apo forms of CaM)
- To stimulate different environmental conditions, we changed ionic strenght(IS) of the systems.(Now we have two different environmental conditions: lLow IS, Physiological)

In this repository, pmf files and metadynamics graphics are belong to Low IS Holo CaM.
