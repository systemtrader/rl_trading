Building Trading Models Using Reinforcement Learning
==================


I propose the use of a learning algorithm and tile coding to develop an interest rate trading strategy directly from historical high-frequency order book data. No assumption about market dynamics is made, but it requires creating a simulator wherewith the learning agent can interact to gain experience. **This repository contains the framework built** to my dissertation of the quantitative finance mastership program, from [FGV](http://portal.fgv.br/en/news/fgv-among-worlds-10-best-think-tanks) University. You can check my master thesis <a href="" target="_blank">here </a> and the presentation <a href="" target="_blank">here </a> (both are still in progress). The folder structure is heavily inspired by OpenAi's [Gym](https://github.com/openai/gym) and the code in Udacity's [smartcab](https://github.com/udacity/machine-learning/tree/master/projects/smartcab) project.


### Install
This project requires **Python 2.7** and the following Python libraries installed:

- [Bintrees](https://pypi.python.org/pypi/bintrees/2.0.2)
- [Matplotlib](http://matplotlib.org/)
- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [Seaborn](https://web.stanford.edu/~mwaskom/software/seaborn/)
- [BeautifulSoup](https://pypi.python.org/pypi/beautifulsoup4)


### Run
In a terminal or command window, navigate to the top-level project directory `rl_trading/` (that contains this README) and run the following command:

```shell
$ python -m market_sim.agent [-h] [-t] [-d] [-s] [-m] <OPTION>
```

Where *OPTION* is the kind of agent to be run. The flag *[-t]* is the number of trials to perform using the same file, *[-d]* is the date of the file to use in the simulation, *[-m]* is the month of the date and *[-s]* is the number of sessions on each trial. Use the flag *[-h]* to get information about what kind of agent is currently available, as well as other flags to use. The simulation will generate log files to be analyzed later on. Be aware that any of those simulations options might take several minutes to complete.




### Data
An example of the datasets used in this project can be found [here](https://www.dropbox.com/s/xo5ul1h3hmtfw1k/201702.zip?dl=0). Unzip it and include in the folder `data/preprocessed`.


### Reference
1. BUSONIU, L. et al. *Reinforcement learning and dynamic programming using function approximators*. CRC press, 2010.
2. CHAN, N. T.; SHELTON, C. *An electronic market-maker*. 2001.
3. GOULD, M. D. et al. *Limit order books*. Quantitative Finance, 2013.
3. SUTTON, R. S.; BARTO, A. G. *Reinforcement Learning: An Introduction*, draft, in progress. 2st. MIT Press, 2017.
4. SPOONER, T. L. *Reinforcement Learning for High-Frequency Market Making in Limit Order Book Markets*. Master Thesis — the University of Liverpool, 2016.

<details><summary>More references</summary>

6. BELLMAN, R. *The theory of dynamic programming*. 1954.
7. CUMMING, J.; ALRAJEH, D.; DICKENS, L. *An Investigation into the Use of Reinforcement Learning Techniques within the Algorithmic Trading Domain.* Master Thesis, 2015.
5. DU, X.; ZHAI, J.; LV, K. *Algorithm trading using q-learning and recurrent reinforcement learning*. Citeseer, v. 1, p. 1, n.d.
6. FERRUCCI, D. et al. *Building watson: An overview of the deepqa project*. AI magazine, v. 31, n. 3, p. 59–79, 2010.
7. FLETCHER, T. *Machine learning for financial market prediction*. Thesis — UCL (University College London), 2012.
9. HALL, T.; KUMAR, N. *Why Machine Learning Models Often Fail to Learn: QuickTake Q&A*. 2017. [Online].
10. KAELBLING, L. P.; LITTMAN, M. L.; MOORE, A. W. *Reinforcement learning: a survey*. Journal of Artificial Intelligence Research, v. 4, p. 237–285, 1996.
11. KEARNS, M.; NEVMYVAKA, Y. *Machine learning for market microstructure and high frequency trading*. 2013.
12. KIM, A. J.; SHELTON, C. R.; POGGIO, T. *Modeling stock order flows and learning market-making from data*. 2002.
13. KPMG International. *Transformative change: How innovation and technology are shaping an industry*. 2016.
14. LEE, J. W. et al. *A multiagent approach to q-learning for daily stock trading*. IEEE Transactions on Systems, Man, and Cybernetics-Part A: Systems and Humans, IEEE, v. 37, n. 6, p. 864–877, 2007.
15. LI, X. et al. *An intelligent market making strategy in algorithmic trading*. Frontiers of Computer Science, Springer, v. 8, n. 4, p. 596–608, 2014.
16. LUESKA, L. C. *Modelo HJM multifatorial com processo de difusãso com jumps aplicado ao mercado brasileiro*. Master Thesis, 2016.
17. MELO, F. S.; MEYN, S. P.; RIBEIRO, M. I. *An analysis of reinforcement learning with function approximation*. In: ACM. Proceedings of the 25th international conference on Machine learning. 2008. p. 664–671.
18. MITCHELL, T. *Machine Learning*. McGraw-Hill, 1997. (McGraw-Hill International Editions). ISBN 9780071154673.
19. MOHRI, M.; ROSTAMIZADEH, A.; TALWALKAR, A. *Foundations of Machine Learning*. The MIT Press, 2012. ISBN 026201825X, 9780262018258.
20. NEVMYVAKA, Y.; FENG, Y.; KEARNS, M. *Reinforcement learning for optimized trade execution*. In: ACM. Proceedings of the 23rd international conference on Machine learning. 2006. p. 673–680.
21. O’HARA, M. *High frequency market microstructure*. Journal of Financial Economics, Elsevier, v. 116, n. 2, p. 257–270, 2015.
22. RONCALLI, T. *Big Data in Asset Management*. 2014. Apresentação.
23. SEIJEN, H. van; FATEMI, M.; ROMOFF, J. *Improving scalability of reinforcement learning by separation of concerns*. arXiv preprint arXiv:1612.05159, 2016.
24. SHERSTOV, A. A.; STONE, P. *Function approximation via tile coding: Automating parameter choice*. In: SPRINGER. International Symposium on Abstraction, Reformulation, and Approximation. 2005. p. 194–205.
25. SHREVE, S. *Stochastic calculus for finance I: the binomial asset pricing model*. Springer Science & Business Media, 2012.
26. SILVER, D. et al. *Mastering the game of go with deep neural networks and tree search*. Nature, Nature Publishing Group, v. 529, n. 7587, p. 484–489, 2016.
29. WASKOW, S. J. *Aprendizado por reforço utilizando tile coding em cenários multiagente*. 2010.
30. WATKINS, C. J.; DAYAN, P. *Q-learning*. Machine learning, Springer, v. 8, n. 3-4, p. 279–292, 1992.
31. WATKINS, C. J. C. H. *Learning from delayed rewards*. Thesis — University of Cambridge England, 1989.
32. XAVIER, A. *The Distribution/Intermediation Industry in Brazil: Challenges and Trends*. 2015. [Online].
</details>


### License
The contents of this repository are covered under the [Apache 2.0 License](LICENSE.md).
