
by Gregory Urman

www.linkedin.com/in/gregoryurman 


## Multi-Armed Bandit ##

In this project, we will examine the classic reinforcement learning problem known as the Multi-Armed Bandit. It is also known as the K-armed bandit problem or the N-armed bandit problem [1, see footnotes in the end]. Here, we are looking to maximize our potential gains from a set of potential resources by choosing between each resource so as to maximize our expected gains. (The term I've heard the most here is "maximize our rewards" and that entails knowing how much rewards, if any, might be derived from a set of actions). This kind of problem has been researched since the 1950's and may take many forms including: A) how to distribute a given budget among these research departments to maximize results? B) gaining the most out of clinical trials while minimizing potential losses, C) financial applications, etc [1]. In this case, we will start with the simplest example: slot machines.


![one_arm_bandit](https://user-images.githubusercontent.com/22970879/41629289-ec662a58-73e5-11e8-9f41-40c6d7ba5a36.jpg)
[2]


Please be aware that we will be choosing between different resources through the use of an AGENT. Meaning, an algorithm or a program that we have trained to make decisions that will then work on its own. The specific algorithm we will be using is called "Epsilon-Greedy" and it uses the exploitation vs. exploration tradeoff model for reinforcement learning [4]. Specifically:

"It considers different paths to “explore” and “exploit” in order to maximize rewards. ... One uses coins to put into one of three (3) slot machines and tries to win as much money as they can by picking the best machine to risk the coins on [in reality this would be an ever-evolving process because depending on when you start and end, the average of which machine seems to yield the best results will change, so don’t get any ideas of finding the perfect gambling technique!] ... To use a concrete example: Suppose, after your first 12 pulls, you played machine #1 four times and won $1 two times and $0 two times. The average for machine #1 is $2/4 = $0.50. And suppose you’ve played machine #2 five times and won $1 three times and $0 two times. The average payout for machine #2 is $3/5 = $0.60. And suppose you’ve played machine #3 three times and won $1 one time and $0 two times. The average payout for machine #3 is $1/3 = $0.33. ... Now you have to select a machine to play on try number 13. You generate a random number p, between 0.0 and 1.0. Suppose you have set epsilon = 0.10. If p > 0.10 (which it will be 90% of the time), you select machine #2 because it has the current highest average payout. But if p < 0.10 (which it will be only 10% of the time), you select a random machine, so each machine has a 1/3 chance of being selected. So, Machine #2 seems to yield the best results in this case." [3] 








??? do I need this: optimal policy for maximizing the expected discounted reward ???



1 = https://en.wikipedia.org/wiki/Multi-armed_bandit 

2 = http://blog.yhat.com/posts/the-beer-bandit.html 

3 = https://jamesmccaffrey.wordpress.com/2017/11/30/the-epsilon-greedy-algorithm/

4 = https://en.wikipedia.org/wiki/Reinforcement_learning



