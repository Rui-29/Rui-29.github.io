---
layout: page
title: MACHINE LEARNING
subtitle: 
---
This page is for collecting tech-resources related to **ML and its applications**.  
**Papers/Seminars** that I think worth a reading/listening are also listed.

### Tech-resources
***GitHub*** | [All you need to know](https://youtu.be/rE2zRhZdjFU?si=aso4tbKCW44fIzjo), as well as [resolve merge conflicts](https://youtu.be/xNVM5UxlFSA?si=HNujkfm3R7DHeGoJ).  
***Notes***:  
* Configuring Git with '*git config*', initializing a Git Repository with *git init*, checking Repository Status with 'git status'.  
* Cloning a Repository with 'git clone', Creating and Staging Files with 'git add .', create and switch branch at the same time 'git branch' git checkout -b NAME.  
* Switching Between Branches with 'git switch', Pushing Changes to a Remote Repository with 'git push' (repo name)(branch name). Updating Local Repository with 'git pull'.
* better ask coworkers before pull request and merge your branch to the main, Viewing Change History with 'git show', Deleting Branches Locally and Remotely: git branch –d branch name to delete locally, git push -delete origin branch.  
* Merge the conflict is important, Git merge branch name (-- abort), three options: Accept current/incoming/both change.  

***GNN & PyG*** | [GNN using Pytorch Geometric | coding from Stanford](https://youtu.be/-UjytpbqX4A?si=UMotffD0bpDXo4fy) together with official tutorial of [Pytorch](https://pytorch.org/tutorials/beginner/basics/buildmodel_tutorial.html) & [PyG](https://pytorch-geometric.readthedocs.io/en/latest/get_started/introduction.html). Also, animation for GNN intro [[short]](https://youtu.be/epVW0_iVBX8?si=OXILHRrtdLSxkGsu) [[well detailed]](https://youtu.be/GXhBEj1ZtE8?si=HO35GR0cgprNJqy9) and [Microsoft](https://www.youtube.com/watch?v=zCEYiCxrL_0&t=2s). Basically it is dealing with multi-dimensional info, applied to material science, drug development, social networks, but also beyond...     
***Notes***:  
* The overall Pytorch workflow is to class a network, define parameters and forward functions. Remember to add ***self.*** Before parameter, otherwise it won't be added to parameter lists.  
* Training metric (loss) need to be differentiable, but evaluation metric no need, sklearn have a lot evaluation metrics already, no need to hand write.  
* The precision is the ratio ***tp / (tp + fp)***, recall ***tp / (tp + fn)***, F1 score: ***2 * precision * recall/(precision+recall)***, all of these are 1 best 0 worst.  
* [TensorboardX](https://github.com/lanpa/tensorboardX) for tracking torch training process, [sklearn manifold](https://scikit-learn.org/stable/modules/manifold.html) for dimensional reduction, with its [t-SNE](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html) for high dimension data visualization.  
* [nn.ModuleList](https://pytorch.org/docs/stable/generated/torch.nn.ModuleList.html) has more freedom than [nn.Sequential](https://pytorch.org/docs/stable/generated/torch.nn.Sequential.html), and can implement append.
* [Spatiotemporal GNN](https://www.sciencedirect.com/topics/computer-science/spatiotemporal-graph). And also a [video](https://youtu.be/RRMU8kJH60Q?si=Wrd2r0FIsHroQvgM). In summary, it deals with static structure with time-varying features. A Spatiotemporal Graph is defined as a graph that captures the temporal patterns and spatial information of things' usage events, where nodes represent locations, timestamps, and things, and edges represent relationships between locations, timestamps, and things based on similarities and periodic patterns. So basically, the features changing along the time, but all these nodes and edges are still there connected, which is a static structure.  

***MPC*** | [Model predictive control implementation](https://youtu.be/8BHMsKXlRq0?si=Ww5S014JPm5Qz0vC), together with a [short intro](https://youtu.be/YwodGM2eoy4?si=8ocz0FNhjLSE8f6s) by [Steven L. Brunton](https://scholar.google.com/citations?user=TjzWdigAAAAJ&hl=en).  
***Notes***:  
* Basic concept: strategy ***u*** at time ***k*** is the optimal short-time control starting at ***k***, applying to the system, and system will send updated states to MPC for the timestep ***k+1***.  
* Strength: can compose constraints, work with nonlinear systems (can be linearize if needed). Cons: online, computational expensive as need to reschedule future horizons every step receiving feedbacks.
* A compromising way is to do linear parameter varying, but with computational speed boosting, directly handle nonlinear system is becoming feasible.

**Model-based RL** |  let's goooo
**Model-based RL** |  let's goooo


### Papers/Seminars
**Jul 2021** | [GNN env based RL?](https://dl.acm.org/doi/abs/10.1145/3632775.3661957).  
    **Notes**: python is great in enhancing the ability from data processing to time-series forecasting, till the sophisticated control.
**Jul 2021** | [Spatiotemporal](https://www.sciencedirect.com/topics/computer-science/spatiotemporal-graph). And also a [video](https://youtu.be/RRMU8kJH60Q?si=Wrd2r0FIsHroQvgM)
