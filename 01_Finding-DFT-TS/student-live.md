Lesson 01: Finding transition states using DFT
=======================

## Purpose
 In this project you will be investigating the reaction energies and transition state energies for S<sub>N</sub>1, S<sub>N</sub>2, E1, and E2 reactions using computational chemistry. 

## Learning Objectives
At the end of this lesson, students will be able to...
1. Draw moleculear geometries in ChimeraX and save them as *.xyz files.
2. Generate and save an ORCA input file using ChimeraX.
3. Run an ORCA input file to generate an output file.
4. Do basic analysis of an ORCA output file using either ChimeraX or a text editor.
5. Determine reaction energies in Hartree kcal/mol, and kJ/mol.

 ## Background
 Thermodynamic properties, such as reaction energies, are commonly calculated using quantum mechanical (QM) methods. While it is not possible to directly compare theoretical molecular energies with experiment, relative energies (reaction energies) can be compared. Additionally, by carefully selecting the reaction to be calculated errors in the calculations due to: not a large enough basis set, low level of theory, or the neglect of correlation can be largely canceled out. These types of reactions should have as few differences between the reactants and products as possible in terms of bonds and types of bonds and are called “isodesmic” reactions. 

 ## Outline
 For today we will be investigating the thermodynamic and kinetic control of the reaction of a secondary alkyl halide, 2-bromopropane, with the nucleophilic base methoxide. In this reaction there are four competing mechanisms (SN1, SN2, E1, and E2) which result in two different sets of products

 <img src="./RXN-01.svg" style="background-color: white; padding: 5px;"/>

 ### Task 01 - Calculate the thermodynamic reaction energies of the two overall reactions using B3LYP/6-311G*. 

 1) Open up ChimeraX and draw each product and reactant as separate molecules. You should have six total molecules as different models in the ChimeraX Model Panel when you are done (2-bromopropane, methoxide, 2-methoxypropane, propylene, methanol, and bromide).

    * You will need to have the SEQCROW tools installed to draw and make input files for quantum chemistry programs. Go to Tools &rarr; More Tools... Search for SEQCROW in the ChimeraX Toolshed window that appears, click on SEQCROW and install.

    * To draw simple molecules go to Tools &rarr; Structure Editing &rarr; 2D Builder. This will open a new window where you can draw Lewis structures. Make sure to indicate correct charges on atoms for methoxide, [CH<sub>3</sub>O]<sup>-</sup>, and bromide, Br<sup>-</sup>.

    * Before you click the "open molecule" button make sure to name your molecule. You can also rename molecules (models in ChimeraX language) by double clicking on the name of the model in the Model Panel, usually inset on the bottom right. If the Model Panel is not visibal you can access it by going to Tools &rarr; General &rarr; Model Panel. 
    
    * It is often useful to save your molecules as *.xyz files.

2) Generate an ORCA input file 