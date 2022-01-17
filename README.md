# COMSOL_GNN
## Cantilever, Simply supported beam, L-shaped beam topoplogy optimization prediction with GNN
### Flow
![flow](https://user-images.githubusercontent.com/56711947/149702568-05db5730-2646-476e-a2ac-5a0e9fc7a430.jpg)

### Input node features
Displacement, stress, strain energy density, mesh coordinates, volume fraction
![inputs](https://user-images.githubusercontent.com/56711947/149703492-c969eace-fdde-4517-bb2f-0df6636d3ff8.jpg)  

### Graph structure
Triangular mesh to graph structure  
![graph](https://user-images.githubusercontent.com/56711947/149703999-0ded7908-4fb6-4449-85f8-ea057ea1f3e2.jpg)

### Model architecture
33 Graph convolution layers with batch normalization, dropout, L2 regularization  
Used residual connection in hidden node features  
![model](https://user-images.githubusercontent.com/56711947/149703686-7803865c-212e-4ed5-ac1c-74407af170be.jpg)

### Results
Top picture -> Topology optimization  
Bottom picture -> GNN prediction  
![res_pic](https://user-images.githubusercontent.com/56711947/149704099-81d2a28e-263e-44ad-bc4f-d1951d55b493.jpg)  
  
Compliance scatter plot & Coefficient of determination
![scatter](https://user-images.githubusercontent.com/56711947/149704275-df5a24e0-9410-4f1e-8924-6b31a6b2532a.jpg)
