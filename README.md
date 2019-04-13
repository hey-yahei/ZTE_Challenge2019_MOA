## Baseline for ZTE_Challenge2019(Model Optimization and Acceleration)
I will open source my previous solutions without tweak.     
Just some experimental code of ideas are shown here, while more general tools may be open source after the challenge.   
    
### Costs     
Test the origin model on RTX2080TI(ms) --          
![](https://github.com/hey-yahei/ZTE_Challenge2019_MOA/blob/master/assets/images/costs.jpg)      

### Ideas List    
1. `merge_bn.ipynb`: Merge batchnorm layers to convolution.      
2. `clear_idle_filters.ipynb`: Clear some idle filters whose weights are near to zero.     
3. `fc_svd.ipynb`: Seperate a fully connection into several ones via SVD.    
4. Seperate a kxk-convolution into \[kxk, 1x1\] or \[kx1, 1xk\].
5. Use some special algorithm for computations(im2, kn2, Winograd, FFT, direct and so on). 
6. Try different stategies to prune.
7. Sparse convolutions and fully connections.
8. Quantization...
    
**Good luck~**
