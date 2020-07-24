# Skeletonization
Tracking c. elegans can become quite a challenge, when these worms roll up in coiled shapes, aggregate with other worms, or with dirt in the petri dish. In this work, a simple solution is proposed using artificial vision techniques to help tracking these nematodes. This method uses the distance transform function to obtain an improved skeleton. Using this new skeleton some possible predictions of the next pose are obtained. An optimization function evaluates all and determines the best next pose prediction.

# Requirements:
This demo was tested in Windows 10 with Matlab R2018b.
- Windows 10
- Matlab R2018b

# Clone Skeletonization repository:
```
git clone https://github.com/playanaC/Skeletonization.git
```

# Run the skeletonization demo in Matlab:
- Before you start, change the path of the images in *path variable* in Main.m file.
- Run Main.m macro. This macro will first find the region of interest (inside the petri dish), then it will get all the worm trajectories, these will be evaluated to classify the areas in worm tracks(red), noise (blue), areas with little movement (green). Second, you will evaluate each tracks to obtain all the worm skeletons within it. Third, the results will be saved in xml files. 


# Image adquisition system:
- Images were captured by an [open hardware system](https://github.com/JCPuchalt/c-elegans_smartLight).


# References:
- Puchalt, J. C., Sánchez-Salmerón, A.-J., Martorell Guerola, P. & Genovés Martínez, S. "Active backlight for automating visual monitoring: An analysis of a lighting control technique for *Caenorhabditis elegans* cultured on standard Petri plates". PLOS ONE 14.4 (2019) [doi paper](https://doi.org/10.1371/journal.pone.0215548)

- Puchalt, J.C., Sánchez-Salmerón, A., Ivorra, E. et al. "Improving lifespan automation for *Caenorhabditis elegans* by using image processing and a post-processing adaptive data filter". Scientific Reports (2020) [doi paper](https://doi.org/10.1038/s41598-020-65619-4).
