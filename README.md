# Data-Driven Fault Diagnosis in Unknown Model Discrete Event System

For a DES (modeling by complete Deterministic Finite State Automata), its model is unknown, but running logs are available. 

Using DeepLearning approach to do fault diagnosis based on the given running logs.

## Abstract

With the continuous development of technology, there will be more and more artificial systems, and more and more deeply into people's lives. The system faults are usually inevitable, and it is very difficult to diagnose and isolate this faults manually. Therefore, it is very important to establish formal methods to diagnose and isolate faults quickly. In recent years, via the discrete event systems (DES) model, the problem of fault diagnosis has been well investigated. Fault diagnosis methods can be roughly divided into white-box diagnosis and black-box diagnosis. The white-box diagnosis can give accurate results, but it needs sufficient knowledge of the target system. The black-box diagnosis does not depend on the system model, whereas it needs a mass of records of system running to ensure a satisfied accuracy of diagnosis.
In this paper, we present a diagnosis approach based on machine learning, which belongs the black-box method. First of all, in order to simulate the real DES, we construct the automata model randomly. In order to ensure that the generated automaton is diagnosable, we use the polynomial-time algorithm proposed by Sheng- Bing Jiang et al to verify the diagnosability of the automata. Then we use the constructed automata to generate the running-log data set. Secondly, we give the structure of the neural network models, and intuitively show that these models have excellent learning ability and generalization ability on the data set of the research problem. And then, we make an experiment to compare the accuracy of Cheng Jiang's critical tree approach with the models. The results show that, under certain conditions, the diagnosis accuracy of the method proposed in this paper is better than that of the critical tree approach. Finally, we also give a possible application scenario on a simple practical system to illustrate the practical applicability of the method in this paper.

**Key Words**: Fault Diagnosis; Discrete Event System; CNN; RNN; Sequence Classification
> 随着科技的不断发展，人造系统将越来越多，也越来越深入人们的生活。系统错误的发生通常很难避免，如果人工进行错误诊断，将会非常困难。因此，如何建立形式化方法来快速地诊断并隔离错误显得非常重要。近年来，人们通过离散事件系统(DES)对人造系统建模，广泛地研究了错误诊断问题。错误诊断方法大致可以分为白盒诊断和黑盒诊断。其中白盒诊断能够给出精确的结果，但需要对目标系统有充分的认知；而黑盒诊断不依赖系统模型，但需要大量的系统运行序列才能保证错误诊断的准确率。
> 本文使用了黑盒诊断方法，在仅系统前期的运行日志已知的情况下，探索能够构建诊断器的机器学习方法。首先，为了模拟现实中可诊断的离散事件系统，我们构造了随机自动机模型，并使用ShengBing Jiang等人提出的多项式时间算法来确保了随机生成的自动机的可诊断性，之后用已构建的可诊断自动机来生成运行日志数据集。接着我们给出了神经网络模型的结构，然后通过实验直观地展示了这些模型在该研究问题的数据集上具备优秀的学习能力和泛化能力。之后，我们设计一组实验比较了Cheng Jiang的关键树方法与本文模型的准确率。实验结果表明，一定条件下本文模型在准确率上可以比拟甚至超过关键树方法。最后，我们还给出简单实际系统上的一个可能应用场景，以说明本文方法的实际可应用性。

> **关键词**：错误诊断；离散事件系统；卷积神经网络；循环神经网络；序列分类 

## References

1. Lin F. Diagnosability of discrete event systems and its applications[J]. Discrete Event Dynamic Systems, 1994, 4(2): 197-212.
2. 吴旋. 基于离散事件动态系统的故障诊断理论的研究[D].浙江大学,2002.
3. Son H I, Lee S. Failure diagnosis and recovery based on DES framework[J]. Journal of Intelligent Manufacturing, 2007, 18(2): 249-260.
4. Sampath M, Sengupta R, Lafortune S, et al. Diagnosability of discrete-event systems[J]. IEEE Transactions on automatic control, 1995, 40(9): 1555-1575.
5. Jiang S, Huang Z, Chandra V, et al. A polynomial algorithm for testing diagnosability of discrete-event systems[J]. IEEE Transactions on Automatic Control, 2001, 46(8): 1318-1321.
6. Yoo T S, Lafortune S. Polynomial-time verification of diagnosability of partially observed discrete-event systems[J]. IEEE Transactions on automatic control, 2002, 47(9): 1491-1495.
7. Pecheur C, Cimatti A, Cimatti R. Formal verification of diagnosability via symbolic model checking[C]. In Workshop on Model Checking and Artificial Intelligence (MoChArt-2002), Lyon, France. 2002.
8. Fessant F, Clérot F. An efficient som-based pre-processing to improve the discovery of frequent patterns in alarm logs[C]. In Conference on Data Mining| DMIN. 2006, 6: 277.
9. Jiang C, Deng W, Qiu D. Fault Diagnosis in Unknown Discrete Event Systems via Critical Tree[C]. In 2019 Chinese Control And Decision Conference (CCDC). IEEE, 2019: 1846-1851.
10. Briones L B, Lazovik A, Dague P. Optimal observability for diagnosability[C]. In Nineteenth International Workshop on Principles of Diagnosis (DX-08). 2008: 31-38.
11. de Kleer J. Using crude probability estimates to guide diagnosis[J]. Artificial intelligence, 1990, 45(3): 381-391.
12. Cassez F, Tripakis S. Fault diagnosis with static and dynamic observers[J]. Fundamenta Informaticae, 2008, 88(4): 497-540.
13. Christopher C J, Cordier M O, Grastien A. Critical observations in a diagnostic problem[C]. In 53rd IEEE Conference on Decision and Control. IEEE, 2014: 382-387.
14. Christopher C J, Grastien A. Formulating event-based critical observations in diagnostic problems[C]. In 2015 54th IEEE Conference on Decision and Control (CDC). IEEE, 2015: 4462-4467.
15. Cordier M O, Travé-Massuyes L, Pucel X. Comparing diagnosability in continuous and discrete-event systems[C]. In Proceedings of the 17th International Workshop on Principles of Diagnosis (DX-06). 2006: 55-60.
16. Jéron T, Marchand H, Pinchinat S, et al. Supervision patterns in discrete event systems diagnosis[C]. In 2006 8th International Workshop on Discrete Event Systems. IEEE, 2006: 262-268.
17. Christopher C J, Pencolé Y, Grastien A. Inference of fault signatures of discrete-event systems from event logs[C]. In DX. 2017: 219-233.
18. Kim Y. Convolutional neural networks for sentence classification[J]. arXiv preprint arXiv:1408.5882, 2014.
19. Zhang X, Zhao J, LeCun Y. Character-level convolutional networks for text classification[C]. In Advances in neural information processing systems. 2015: 649-657.
20. Marinho W, Martí L, Sanchez-Pi N. A compact encoding for efficient character-level deep text classification[C]. In 2018 International Joint Conference on Neural Networks (IJCNN). IEEE, 2018: 1-8.
21. Bai S, Kolter J Z, Koltun V. An empirical evaluation of generic convolutional and recurrent networks for sequence modeling[J]. arXiv preprint arXiv:1803.01271, 2018.
22. Cassandras C G, Lafortune S. Introduction to discrete event systems[M]. Springer Science & Business Media, 2009.
23. Escobet T, Bregon A, Pulido B, et al. Fault Diagnosis of Dynamic Systems[M]. Springer International Publishing, 2019.
24. Buda M, Maki A, Mazurowski M A. A systematic study of the class imbalance problem in convolutional neural networks[J]. Neural Networks, 2018, 106: 249-259.
25. Yosinski J, Clune J, Bengio Y, et al. How transferable are features in deep neural networks?[C]. In Advances in neural information processing systems. 2014: 3320-3328.
26. Bengio Y. Practical recommendations for gradient-based training of deep architectures[M]. Neural networks: Tricks of the trade. Springer, Berlin, Heidelberg, 2012: 437-478.
27. Masters D, Luschi C. Revisiting small batch training for deep neural networks[J]. arXiv preprint arXiv:1804.07612, 2018.
28. Kingma D P, Ba J. Adam: A method for stochastic optimization[J]. arXiv preprint arXiv:1412.6980, 2014.
29. Ruder S. An overview of gradient descent optimization algorithms[J]. arXiv preprint arXiv:1609.04747, 2016.
