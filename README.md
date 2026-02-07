# DifferLand_training
Code for how to use DifferLand, and develop your own "DifferLand"

## Step by step
### Preparation
```bash
# Nevigate to your own path
cd /to/your/own/path/
# Create a new folder
mkdir DifferLand_training
cd DifferLand/
mkdir code
cd code/
# Copy code of simplified DifferLand_site_version, only ACM model
cp -r /data1/fyliu/e_soil_carbon_model/code/DifferLand_v_simple/ ./
# Copy code of DifferLand_site_version
cp -r /data1/fyliu/e_soil_carbon_model/code/DifferLand_site/ ./
# Copy code of DifferLand_global_version
cp -r /data1/fyliu/j_DifferLand_ET_SOC/code/DifferLand_global_v3/ ./
# Activate your python environment
conda activate DifferLand
# or
conda activate diffland
# Download an additional python package for site version
pip install geopy
```

### Use DifferLand site version
```bash
cd DifferLand_site/experiments/
python calibration.py
```

### Use DifferLand global version
cd ../../DifferLand_global_v3/experiments/
python calibration.py

### Develop your own "DifferLand"
1. Recommend to develop based on the original DifferLand code, no matter site or global version, especailly the global version.
2. A case study see in DifferLand_v_simple at site scale.
