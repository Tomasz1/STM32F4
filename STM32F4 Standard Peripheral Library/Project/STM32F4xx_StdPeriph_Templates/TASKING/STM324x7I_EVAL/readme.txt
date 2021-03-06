/**
  @page tasking TASKING Project Template for STM32F4xx devices
 
  @verbatim
  ******************** (C) COPYRIGHT 2013 STMicroelectronics *******************
  * @file    readme.txt
  * @author  MCD Application Team
  * @version V1.1.0
  * @date    18-January-2013
  * @brief   This sub-directory contains all the user-modifiable files needed to
  *          create a new project linked with the STM32F4xx Standard Peripherals
  *          Library and working with TASKING VX-toolset for ARM Cortex-M.
  ******************************************************************************
  *
  * Licensed under MCD-ST Liberty SW License Agreement V2, (the "License");
  * You may not use this file except in compliance with the License.
  * You may obtain a copy of the License at:
  *
  *        http://www.st.com/software_license_agreement_liberty_v2
  *
  * Unless required by applicable law or agreed to in writing, software 
  * distributed under the License is distributed on an "AS IS" BASIS, 
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  ******************************************************************************
  @endverbatim
 
 @par Directory contents
 
 - .cproject/.project: A pre-configured project file with the provided library
                       structure that produces an executable image with TASKING.

- TASKING                     : This folder contains
 
     - stm32f4xx.lsl          : This file is TASKING linker script that contains the 
                                STM32F4xx vector table and used to place program code (readonly) 
                                in internal FLASH and data (readwrite, Stack and Heap)in
                                internal SRAM. 
                                You can customize this file to your need.

                           
 @par How to use it ?

 - Open TASKING toolchain.
 - Click on File->Import, select General->'Existing Projects into Workspace' 
   and then click "Next". 
 - Browse to  TASKING workspace directory and select the project: 
   - STM324x7I_EVAL: to configure the project for STM32F4xx devices.
 - Under Windows->Preferences->General->Workspace->Linked Resources, add 
   a variable path named "Cur_Path" which points to the folder containing
   "Libraries", "Project" and "Utilities" folders.
 - Rebuild all project files: Select the project in the "Project explorer" 
   window then click on Project->build project menu.
 - Run program: Select the project in the "Project explorer" window then click 
   Run->Debug (F11)

 @note The needed define symbols for this config are already declared in the
       preprocessor section: USE_STM324x7I_EVAL, STM32F427X, USE_STDPERIPH_DRIVER 
       
 @note The full support of STM32F4 (2MB flash) using �TASKING_CortexMandR-VX_v4.3r1p1.zip� 
       will be available at Tasking web site at the following link: www.tasking.com/support/arm
       After installing the patch, please ensure that you are referring to STM32F437II part 
       number in your Tasking project.


 * <h3><center>&copy; COPYRIGHT STMicroelectronics</center></h3>
 */
