# j-pet-multiphoton-classification
Data transformation and classificiation methods for J-PET tomography.

## Repairing data
**Requirements**: python3.6 and the required packages  
**Input format**: CSV  
**Input columns**: Discribed in the function *dataFrameNames()* at */RepairingData/repairingData.py* script  
**Output format**: CSV  
**Output columns**: same as above  
**Purpose**: Repairing wrong class labels and shuffle the order of particles.  
**Usage**: ./RepairingData/repairingData.py 'path_to_output_data' 'data_part'  
**PS**: Input data folder and filename set as '/mnt/opt/groups/jpet/NEMA_Image_Quality/3000s/' and 'NEMA_IQ_384str_N0_1000_COINCIDENCES_'.
You can change it inside the script.  

## Transforming data
**Input format**: CSV  
**Input columns**: Discribed in the function *dataFrameNames()* at */TransformingData/transformingData.py* script  
**Output format**: binary file  
**Output columns**: same as above + result of the function *featureEngineering()* at */TransformingData/transformingData.py* script    
**Purpose**: Feature engineering and saving as binary file  
**Usage**: ./TransformingData/transformingData.py 'path_to_data' 'data_part'  
**PS**: Filename set as 'NEMA_IQ_384str_N0_1000_COINCIDENCES_' with the infixion 'REPAIRED_' while loading the data (see the scirpt */TransformingData/transformingData.py*).
You can change it inside the script.  

