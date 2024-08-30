# Description

This repository contains the working OpenSim model files (https://simtk.org/projects/opensim) for a kinematic model of a human torso, neck, and head that is suitable for tracking optical tracking passenger data that involves torso movements of around 10-30 cm. The pelvis is attached to the ground through a free joint, the lumbar spine comes from Christophy et al. (with a small change), and the neck model comes from Mortensen et al. The marker set has been custom designed to suit an experiment in a mechanical car simulator. To explore the models it is best to load them in OpenSim Creator (https://www.opensimcreator.com/)

# Model Description

 - *passengerModel.osim*\
        Work in progress of the passenger model. 

 - *reference/Christophy2012_axialRotationUpd_skeletonOnly.osim*\
        This is the model of Christophy 2012 et al. but only with the skeleton, joints, and coupling constraints. The coefficients of the axial coupling constraints have been updated from the original publication so that an axial_rotation of 45 degrees results in an axial rotation of the torso with respect to the pelvis of 45 degrees. This is described in detail on the SimTK forum for this model. Go to https://simtk.org and search for 'Musculoskeletal Model of the Lumbar Spine', go the forum of this model, then look at the post titled 'Axial rotation coordinate coupling coefficients update'. Or just use this link [Axial rotation coordinate ...](https://simtk.org/plugins/phpBB/viewtopicPhpbb.php?f=567&t=18771&p=0&start=0&view=&sid=ee1fa9fe49baefde716abe720cefe1a4) 

 - *reference/Mortensen2014_rigidTorso.osim*\
        This is the model of Mortensen et al. with the addition of a rigid torso-pelvis, a seat-pelvis joint, and a custom marker set.


# References

 - Christophy M, Faruk Senan NA, Lotz JC, O’Reilly OM. A musculoskeletal model for the lumbar spine. Biomechanics and modeling in mechanobiology. 2012 Jan;11:19-34.

 - Mortensen JD, Vasavada AN, Merryweather AS. The inclusion of hyoid muscles improve moment generating capacity and dynamic simulations in musculoskeletal models of the head and neck. PloS one. 2018 Jun 28;13(6):e0199912.


