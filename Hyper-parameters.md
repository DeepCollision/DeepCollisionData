# Hyper-parameters for DQN in DeepCollision



| Hyper-parameter                 | Value | Description                                                  |
| :------------------------------ | :---- | ------------------------------------------------------------ |
| learning rate                   | 0.01  | Learning rate for <br />training DQN                         |
| minibatch size                  | 32    | Number of training cases over <br />which each stochastic gradient <br />descent (SGD) update is computed <br />Number of training |
| reply memory size               | 10000 | Number of training <br />samples in the reply memory         |
| discount factor                 | 0.9   | Discount factor gamma                                        |
| eplison                         | 0.1   | Value of eplison in eplison-greedy exploration               |
| target network update frequency | 100   | The frequency with which <br />the target network is updated |

