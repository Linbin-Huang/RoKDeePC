# RoKDeePC
code of paper "Robust and kernelized data-enabled predictive control for nonlinear systems"

--- Simulink Model for RoKDeePC (Version 1.0) ----
--------------------------------------------------

Copyright 2023 ETH Zurich, Linbin Huang (linhuang@ethz.ch, huanglb@zju.edu.cn)

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-- MATLAB R2020b (or higher versions) is required to run the simulink models. 
   "OSQP" (https://osqp.org/) may need to be installed to run the models with DeePC.

-- To get the results, open the Simulink model "RoKDeePC_running.slx".
!! Then, simply run the script "Run_whole.m".
!! The results can be found in the colored scope of the Simulink model "RoKDeePC_running.slx".
   The other functions/scripts in the folders will be automatically executed during the simulations.

-- The example nonlinear unknown test system in the Simulink model corresponds to the one in Example 1 of the paper.
   The converter model in Example 2 contains some blocks whose copy rights are owned by MathWorks and is therefore not released at this point.
   We may release the converter model in future versions of this software, once we replace those blocks with our own code.
   Interested readers can try with their own models in the RoKDeePC simulation framework, while as mentioned in the paper,
   the kernel parameters may need to be re-chosen (in the file "InitFile.m").
   
-- The main parameters of RoKDeePC can be changed in the script "Load_parameters.m".

!! If you are using this software in your research or teaching, please include explicit mention of this software and of our paper:

@article{huang2023,
  title   =  {Robust and kernelized data-enabled predictive control for nonlinear systems},
  author  =  {Huang, Linbin and Lygeros, John and D{\"o}rfler, Florian},
  journal =  {IEEE Transactions on Control Systems Technology},
  year    =  {2023}
}

!! The code also contains the "DeePC" implementation, If you are using it in your research or teaching, 
   please include explicit mention of this software and of our paper:

@article{markovsky2022data,
title={Data-driven control based on the behavioral approach: From theory to applications in power systems},
  author={Markovsky, Ivan and Huang, Linbin and D{\"o}rfler, Florian},
  journal={IEEE Control Systems},
  year={2023}
}
