# Causl intelligence Team Deepmind

## Fairness

- unfairness underlying data
  - 1
    - causal bayesian networks for describing different possible unfairness
    - scenarios 
    - underlying the data
  - 2
    - cbns
    - for measuring 
    - unfairness underlying data
- fair prediction models
  - CBNs for developing fair prediction models
  - Causal influence 

## Causal decision making



## Causal structure learning



## Causal inference estimation problem



## College admission example measuring unfairness

![image-20220711101818513](https://asdsadsadsad.oss-cn-beijing.aliyuncs.com/image-20220711101818513.png)
$$
A=\bar{a}
$$

$$
A=a
$$

$$
PSE_{a\bar{a}}=\mathbb{E}_{p PO(Y_{\bar{a}}(Q_a, D_a))}[Y_\bar{a}(Q_a,D_\bar{a})]-\mathbb{E}_{p PO(Y_a)}[Y_a]
$$

$$
\hat{p}PO(Y_{\hat{a}}(Q_a,D_\hat{a}))|
$$

$$
A \sim Bern (\pi)
$$

$$
Q \sim p_{\theta}^{q}(\cdot |A)
$$

$$
H_d \sim p_\theta^q (\cdot)
$$

$$
D \sim p_\theta^d ( \cdot |A,H_d)
$$

$$
Y \
$$

$$
\
$$

## Causal decision making Can Make Actual Interventions

- Select set of nodes and values in a causal graph that optimize causal effect of interest
- Constrained causal bayesian optimition
  - Continuous setting and ensures that causal effects on protected variables satisfy some constraints
- Causal bandits with unknown graphs
  - Discrete setting and causal graph is unknown

## Constrained causal bayesian 

- Goal
- Select intervention on Statin
- Aspirin 
- Calroies
- Intake
- inimize the prostate specific antigen 
- while keeping BMI lower than 25

## Sub sections

- Reduces the search space by exploiting the graph structure and avaialbel data
- models causal effects with Gaussian processes to capture uncertainity and correlations
- Uses a sequential strategy to select interventions via an acquisition function balances the probability of satisfying the constraints with expected improvement

## Causal bandits with unknown graphs

- Under common assumptions
  - the best intervention set
    - is given

## Causal inference estimation problem

- Select identification formulas
  - Choose between several causal effect identification formulas accounting for statistical and practical considerations

## Selection 

$$
\mathcal{G}
$$

$$
\tau = \mathbb{E}[Y|do (A)]
$$

$$
Z_1
$$

$$
Z_2
$$

$$
\tau \rightarrow O(\sqrt{n})
$$

$$
k^* = arg \mathop{min} \limits_{k} c_k \sigma_k^2
$$

$$
f_3(d) = \mathop{max}\limits_{x_3}(2x_3 + f_4(d-x_3))
$$

## Causal structure learning

- Model that yields the shortest description of the data is most plausible 
- Select graph that leads 

## Causal graph

![image-20220711110320258](https://asdsadsadsad.oss-cn-beijing.aliyuncs.com/image-20220711110320258.png)

毋庸置疑，[临床试验](https://blog.trialspark.com/what-are-clinical-trials/)是推进医学各个方面的关键。大多数健康试验或研究的核心都是着眼于预防、检测或治疗疾病的方法。虽然有多种研究设计可供选择，但许多都属于两大类：干预性或观察性。

***介入试验\***

介入试验[专门](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4083571/)用于评估治疗或预防措施对疾病的直接影响。在作为介入试验的一个例子的随机对照试验中，患有相同疾病的参与者将被随机分成两个或更多组之一：干预组或对照组。有些人会接受干预，可能是药物、设备或其他一些医疗干预（即饮食改变）。有些人不会接受干预，或者会接受当前的标准干预。两组对于试验的目标都是必不可少的，即衡量正在测试的任何药物、设备或其他医疗干预措施的安全性和有效性。

***观察性研究\***

在观察性研究期间，研究者不实施干预。正如美国[国家癌症研究所](https://www.cancer.gov/publications/dictionaries/cancer-terms/def/observational-study)解释的那样，参与者被观察或测量某些结果，但没有试图影响结果。也就是说，没有给予任何治疗。这种方法的一个好处是，如果需要，可以在很长一段时间内研究大量人群。一项观察性研究甚至可以是一项调查，其中调查人员对特定人群进行抽样并随着时间的推移向他们提问。 

***主要区别\***

这两种研究方法之间的一些主要区别在于它们的目标和组织。介入性试验的目的是获得有关特定干预的更多信息。参与者被组织成不同的治疗组，因此研究人员可以比较结果。 

另一方面，观察性研究旨在获得更多关于人群、疾病、信仰或行为的信息，而无需任何干预。研究人员观察参加研究的参与者，但不会直接影响他们的治疗或行为。他们比较了从数据中得出的疾病结果、人群或人群之间的差异。在观察性研究中，调查人员不会创建组进行比较，他们观察和描述已经存在的组。



It goes without saying that [clinical trials](https://blog.trialspark.com/what-are-clinical-trials/) are key to advancing all aspects of medicine. At their core, most health trials or studies look at ways to prevent, detect, or treat disease. While there are various study designs to choose from, many fall within two broad categories: interventional or observational.

***Interventional trials\***

An interventional trial is [specifically designed](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4083571/) to evaluate the direct impacts of treatment or preventative measures on disease. During a randomized controlled trial, which is one example of an interventional trial, participants with the same disease will be randomly separated into one of two or more groups: intervention groups or control groups. Some will be given the intervention, which could be a drug, device, or some other medical intervention (i.e., diet change). Some will not receive the intervention, or will receive the current standard intervention. Both groups are essential to the objectives of a trial, which is to measure the safety and efficacy of whatever drug, device, or other medical intervention is being tested.

***Observational studies\***

During an observational study, no intervention is implemented by the investigator. As the[ National Cancer Institute](https://www.cancer.gov/publications/dictionaries/cancer-terms/def/observational-study) explains it, participants are observed or certain outcomes are measured, but no attempt is made to affect the outcome. Which is to say, no treatment is given. One benefit to this approach is the fact that a large population can be studied, over a long period of time, if needed. An observational study could even be a survey in which the investigator is sampling a particular group of people and asking them questions over time. 

***Key differences\***

Some key differences between these two research approaches are their aim and organization. The aim of an interventional trial is to get more information about a particular intervention. Participants are organized into different treatment groups so investigators can compare results. 

On the other hand, observational studies aim to get more information about populations, diseases, beliefs or behaviors , without any intervention. The investigators observe the participants taking part in the study, but don’t directly influence their treatments or behaviors. They compare differences among disease outcomes, people or populations that emerge from the data. In observational studies investigators do not create groups to compare, they observe and describe groups that already exist.