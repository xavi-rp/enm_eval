# enm_eval

Example of using ENMevaluate (library: ENMeval) with models to predict several bumblebee distributions in Europe, modifying prevalence (MaxEnt parameter).

Created on: 6th October, 2015

Contact: Xavier Rotllan-Puig (xavi@rotllanpuig.cat)

Description: The aim of this script is to build several SDMs (with Maxent) with different
combinations of those parameters that affect models' performance (i.e. regularization and 
features). The R library ENMeval allows evaluate which is the optimal combination of these
parameters in order to improve model performance while limiting overfitting.
The Akaike Information Criterion corrected for small samples sizes reflects both model
goodness-of-fit and complexity and it is independent of the partitioning method because 
it is computed with the full set of presences.
The model with the lowest AICc value (i.e. Delta_AICc = 0) is considered the best model out 
of the current suite of models.
Big AUC_diff, equal to overfitted models. 

Original data:  
   -presences_91_12_maxent_meters.csv <- presences of bumblebee species with more than 25 unique 
         records in Europe between 1991-2012 (Rasmont et al., 2015)
         
   -table of prevalences
   
   -explanatory variables to run Maxent
   

References: 

 (1) Muscarella, R., Galante, P. J., Soley-Guardia, M., Boria, R. A., Kass, J. M., Uriarte, 
     M., Anderson, R. P. (2014) ENMeval: An R package for conducting spatially independent 
     evaluations and estimating optimal model complexity for Maxent ecological niche models. 
     Methods in Ecology and Evolution, 5: 1198–1205. doi: 10.1111/2041-210X.12261
     
 (2) Rasmont P., Franzén M., Lecocq T., Harpke A., Roberts S.P.M., Biesmeijer J.C., Castro L.,
     Cederberg B., Dvorák L., Fitzpatrick Ú., Gonseth Y., Haubruge E., Mahé G., Manino A., 
     Michez D., Neumayer J., Ødegaard F., Paukkunen J., Pawlikowski T., Potts S.G., Reemer M., 
     J. Settele, J. Straka, Schweiger O. (2015) Climatic Risk and Distribution Atlas of European 
     Bumblebees. Biorisk 10 (Special Issue), 246 pp.
     
 (3) Radosavljevic, A., Anderson, R. P. (2014), Making better Maxent models of species 
     distributions: complexity, overfitting and evaluation. Journal of Biogeography, 41: 629–643.
     doi: 10.1111/jbi.12227 
     
   


