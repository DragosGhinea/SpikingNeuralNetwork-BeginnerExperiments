# SpikingNeuralNetwork-BeginnerExperiments
Playing around with the spiking neural network architecture

For this project, [snnTorch](https://github.com/jeshraghian/snntorch) was used.

## Conda Environment

The environment for this project was created via
`conda create -n snn python=3.10`


## Introduction


Neuronii LIF (Leaky Integrate-and-Fire):

Aplicații practice în tehnologii neuromorfice: Sunt utilizați în cadrul sistemelor neuromorfice pentru a implementa funcționalitatea neuronilor în hardware specializat.

Simulări eficiente în timp real: Sunt potriviți pentru simulări eficiente în timp real în aplicații precum roboții autonomi sau interfețe creier-computer.



Neuronii artificiali (perceptroni, sigmoidi, etc.):

Învățare automată și rețele neurale artificiale: Sunt utilizați în cadrul rețelelor neurale artificiale pentru a învăța și a generaliza modele din date.

Aplicații de recunoaștere de tipare și clasificare: Sunt potriviți pentru aplicații precum recunoașterea vocală, recunoașterea obiectelor și clasificarea imaginilor.






Mergand pe abordarea SNN, am continuat cu Neuronii LIF ce au un consumul redus de resurse , dar o acuratete sacrificată intr-un mod tolerabil. Folosind LIF, suntem cumva la mijloc intre biologie si neuronii clasici prin inlocuirea unor procere de parsare a unor inputuri cu neuroni clasici cu  primirea datele ca niste spikeuri, care simuleaza astfel impulsurile electrice, facandu-i redundanta primirea tuturor inputurile deodata.

El poate sa le primeasca secvential, si dupa un timp, in functie de hiperparametrii membranei, o sa trimita si el un spike mai departe. Astfel, operatiunea aceasta iti permite sa faci procesari in paralel, pt ca nu tre sa sincronizezi nimic.
