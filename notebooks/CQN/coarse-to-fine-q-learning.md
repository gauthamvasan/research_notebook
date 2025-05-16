
# Continuous Control with Coarse-to-fine Reinforcement Learning 


*Seo, Y., Uruç, J., & James, S. Continuous Control with Coarse-to-fine Reinforcement Learning. In 8th Annual Conference on Robot Learning.*


|    Code     | Paper       | Website     |
|-------------|-------------|-------------|
|[Project Website](https://younggyo.me/cqn/) | [Code](https://github.com/younggyoseo/CQN/tree/master) | [Paper](https://arxiv.org/pdf/2407.07787) |


:::{figure} ../assets/CQN/take_plate_off_colored_dish_rack.mp4
:align: center

Coarse-to-fine action discretization
:::

:::{figure} ../assets/CQN/architecture_overview.png
:align: center

Inference and Q-value extraction 
:::



Design choices
- C51
- Dueling networks
- Weighted sum of behavior cloning loss + Q-learning loss
- Q-learning update uses max operator, but action sampling isn't off-policy. It's weird. It's still the same max operator again. Wouldn't this cancel out the effects?