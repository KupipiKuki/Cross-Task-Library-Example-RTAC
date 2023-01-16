# Cross-Task-Library-Example-RTAC
IEC-61131 SEL-RTAC Cross Task Library Example Project  

This project demonstrates the usage of the Cross Task library, its purpose is to give examples on how the library can be used in accordance with my understanding.  

This example utilizes two mutex objects to provide an synchronized access:  
- id 1 from the automation task to the main task 
- id 2 from the main task to the automation task 
  
- Automation Task Programs  
  - prg_autoTask  
    - Performs some calculation or function  
  - prg_CrossTask_AutoMain_Write  
    - Writes data from the Automation Task into the mutex 1 data structure  
  - prg_CrossTask_MainAuto_Read  
    - Reads data from the Main Task out of the mutex 2 data structure  

- Main Task Programs  
  - prg_mainTask  
    - Performs some calculation or function  
  - prg_CrossTask_MainAuto_Write  
    - Writes data from the Main Task into the mutex 2 data structure  
  - prg_CrossTask_AutoMain_Read  
    - Reads data from the Automation Task out of the mutex 1 data structure  

The CrossTaskView visualization provides a way to set data and see the results for this example  

Example provided by jcheers 2022  
Share as needed  
