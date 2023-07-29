# Demo for the ESWA'23 Paper

This is a demo repository for XAI application in code smell prioritization.    
This repository contains model generation, dataset generation, and data analyzing function.    
**Two video demos containing the execution result of the program is available in the ./vids/ directory. **

Since we do not have the original dataset and the toolset of MSR'23, we are replicating the approach using similar techniques and datasets.     
We are using the Blob smell in the MLCQ dataset annotated by third-party developers for dataset generation.      
Afterward, CK Metric are exploited to generate code metrics. The process metrics are replicated by ourselves using the PyDriller tool.     

Usage: 
1. Install the required dependencies.      
```
pip install -r requirement.txt
```
2. Execute Flask App.      
```
flask --app main run
```
3. Access http://localhost:5000/     
4. Type in the URL of the Git repo for analysis (see ./vids/Dataset Generation.mp4 for a video example).      
5. Access http://localhost:5000/project/{name_of_your_repo} to analyze data (see ./vids/Result Analyze.mp4 for a video example).      