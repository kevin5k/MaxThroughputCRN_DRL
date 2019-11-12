# What is this repository about?
This is the repository for VTC paper that was presented in September 2019.

## Paper Abstract
Radio Frequency powered Cognitive Radio Networks (RF-CRN) are likely to be the eyes and ears of upcoming modern networks such as Internet of Things (IoT), requiring increased decentralization and autonomous operation. To be considered autonomous, the RF-powered network entities need to make decisions locally to maximize the network throughput under the uncertainty of any network environment. However, in complex and large-scale networks, the state and action spaces are usually large, and existing Tabular Reinforcement Learning technique is unable to find the optimal state- action policy quickly. In this paper, deep reinforcement learning is proposed to overcome the mentioned shortcomings and allow a wireless gateway to derive an optimal policy to maximize network throughput. When benchmarked against advanced DQN techniques, our proposed DQN configuration offers performance speedup of up to 1.8x with good overall performance.

Presentation pdf is included for convenience. For additional details, readers are advised to lookup IEEE Xplore Database.
DOI: 10.1109/VTCFall.2019.8891294

## DRL Libraries Used
`keras-rl` implements some state-of-the art deep reinforcement learning algorithms in Python and seamlessly integrates with the deep learning library [Keras](http://keras.io). Documentation is available [online](http://keras-rl.readthedocs.org).

Furthermore, `keras-rl` works with [OpenAI Gym](https://gym.openai.com/) out of the box. This means that evaluating and playing around with different algorithms is easy.

## Environment and Agents
Custom environment is used in this work. For understanding, 2ST represents 2 Secondary Transmitters; 3ST represents 3 Secondary Transmitters.

Customized DRL agent can be found in the folder subfolder of "rl".

## Algorithms Implemented
As of today, the following algorithms have been implemented:

- [x] Deep Q Learning (DQN) [[1]](http://arxiv.org/abs/1312.5602), [[2]](https://www.nature.com/articles/nature14236)
- [x] Double DQN [[3]](http://arxiv.org/abs/1509.06461)
- [x] Dueling network DQN (Dueling DQN) [[9]](https://arxiv.org/abs/1511.06581)
- [x] Double Duel Network DQN (DD-DQN)


## Results
All results for 2ST and 3ST are saved in tensorboard format. When launching tensorboard, set the logdir to be "backscatter/logs"

## Citation
If you find this work interesting and use it in your research, you can contact me for co-authorship opportunities. Otherwise, you can cite this work as follows:

```bibtex
@INPROCEEDINGS{8891294,
author={K. S. H. {Ong} and Y. {Zhang} and D. {Niyato}},
booktitle={2019 IEEE 90th Vehicular Technology Conference (VTC2019-Fall)},
title={Cognitive Radio Network Throughput Maximization with Deep Reinforcement Learning},
year={2019},
volume={},
number={},
pages={1-5},
keywords={Backscatter;Radio frequency;RF signals;Radio transmitters;Mathematical model;Artificial neural networks;Throughput},
doi={10.1109/VTCFall.2019.8891294},
ISSN={},
month={Sep.},}
```


