# SuperlifeStyle

## A Health Incentive Program for Superlife Life Insurance

Authors: H. Dharmadasa, E. Gao, K. Kirubakaran, V. Narayan & N. Verghese

<p float="left">
  <img src="./Logos and Figures/soa.png" width="300" />
  <img src="./Logos and Figures/unsw_horizontal.png" width="300" />
</p>

Welcome to SuperLifeStyle - Your Path to a Healthier Future!

SuperLifeStyle is a cutting-edge Health Incentive Program designed to  revolutionize the way you approach life insurance. We at Apex Analytics designed this program, tailored to not only protect your future but also enhance your present well-being.

Our primary objective with SuperLifeStyle is to incentivize healthy behaviors through engaging health incentives. By participating in the program, you not only secure your financial future with long-term insurance products but also embark on a journey towards a healthier lifestyle.

What sets SuperLifeStyle apart is our unique approach to promoting health and well-being. The implementation of our key 4 incentives offer a diverse range of incentives to encourage and support you in making positive lifestyle changes. By engaging with these initiatives, you not only decrease expected mortality but also unlock exclusive discounts on your insurance premiums.

Here's how SuperLifeStyle works:

1. **Engaging Health Incentives**: Our program offers a 
   range of engaging health incentives, including safety campaigns and 
   community fitness challenges, aimed at promoting healthy behaviors and 
   lifestyle choices. By participating in these initiatives, you not only 
   improve your overall well-being but also qualify for exclusive discounts
   on your insurance premiums.

2. **Personalized Approach**: We understand that each 
   individual's health journey is unique. That's why SuperLifeStyle allows 
   you to tailor your participation based on your preferences and health 
   goals. Whether you prefer safety education or community fitness 
   activities, our program offers flexibility to suit your needs.

3. **Ethical Considerations**: SuperLifeStyle is built on a
   foundation of ethical principles, ensuring transparency, respect for 
   autonomy, and genuine concern for your well-being. We adhere to ethical 
   frameworks such as utilitarianism, deontology, and virtue ethics to 
   guide our decision-making and program execution, prioritizing your 
   health and satisfaction above all else.

4. **Measurable Success**: Our program's success is not 
   just a promise - it's a measurable outcome. Through data-driven metrics 
   and comparisons, we track the impact of SuperLifeStyle on decreasing 
   expected mortality, increasing life insurance sales, and improving 
   market competitiveness. You can rest assured that your participation in 
   SuperLifeStyle is making a tangible difference in your life and the 
   lives of others.

Join us on this transformative journey towards a healthier, more 
secure future. Experience the power of SuperLifeStyle and unlock a world
 of benefits that will enhance your life in ways you never imagined.

> SuperLifeStyle - Where Health, Insurance, and Ethical Excellence Converge for Your Brighter Tomorrow!

## Table of Contents:

1. [File Tree](#file-tree)
2. [Target Objectives for Superlife](#target)
3. [Project Development Pipeline](#pdp)
4. [Program Design](#design)
   1. [Safety Campaigns](#safety)
   2. [Community Fitness Challenges](#fitness)
   3. [Preventative Screening](#screen)
   4. [Smoking Cessation](#cess)
5. [Risk and Risk Mitigation Considerations](#risk)
6. [Data and Limitations](#data)
7. [Sensitivity Analysis](#sens)

## File Tree: <a name="file-tree"></a>

```
.
├── Case Study Documents
│   ├── 2024-srcsc-questions-answers.pdf
│   ├── srcsc-2024-case-study.pdf
│   ├── srcsc-2024-lumaria-encyclopedia-entry.pdf
│   ├── srcsc-2024-official-rules.pdf
│   └── srcsc-2024-superlife-inforce-dataset-key.pdf
├── Data
│   ├── Case Study Data
│   │   ├── 2024-srcsc-superlife-inforce-dataset.csv
│   │   ├── srcsc-2024-interventions.xlsx
│   │   ├── srcsc-2024-lumaria-economic-data.xlsx
│   │   └── srcsc-2024-lumaria-mortality-table.xlsx
│   ├── External Data
│   │   └── superlife_inforce_causes_of_death.csv
│   └── Processed Data
│       ├── Benefit_Modelling.csv
│       ├── Benefits_by_Age_Group.csv
│       ├── CLEANED_2024-srcsc-superlife-inforce-dataset.csv
│       ├── Neoplasm_Mortality_Loading.csv
│       ├── Sensitivity_Analysis.csv
│       ├── Superlife-inforce-mortality-table.csv
│       └── average_mortality_table.xlsx
├── Logos and Figures
│   ├── Benefit_Modelling_page-0001.jpg
│   ├── Benefit_Modelling_page-0002.jpg
│   ├── Benefit_Modelling_page-0003.jpg
│   ├── Benefits by Age Group_page-0001.jpg
│   ├── Cost reduction.png
│   ├── Lives saved.png
│   ├── Objectives.png
│   ├── Pipeline.png
│   ├── Post Interventions Life Table_page-0001.jpg
│   ├── Risk Map.jpeg
│   ├── Risk Rate.jpeg
│   ├── soa.png
│   ├── SPWL Sens Analysis.png
│   ├── T20 Sens Analysis.png
│   ├── unsw_horizontal.png
│   └── unsw_vertical.png
├── R Code
│   ├── ACTL5100 Lumaria Mortality Modelling.R
│   ├── Inforce Benefit Modelling.Rmd
│   ├── Inforce Data Cleaning.Rmd
│   ├── Inforce Data Visualisation.Rmd
│   ├── Inforce Mortality Modelling.Rmd
│   └── Sensitivity Analysis.Rmd
├── .gitignore
├── Apex Analytics Report.pdf
└── README.md
```

### Target Objectives for SuperLife: <a name="target"></a>

<img title="" src="./Logos and Figures/Objectives.png" alt="" width="450">

* <u>Incentivize Healthy Behaviors Through Participation in the Program  </u>
  
  Participation in SuperLifeStyle involves engaging in healthy behaviors, and policyholders will be encouraged to participate through discounts to their premiums. Advertising the health benefits of participation will also encourage participation.  

* <u>Decrease Expected Mortality </u>
  
  SuperLife has provided us with data indicating the health incentives which we have incorporated into SuperLifeStyle will decrease expected mortality for those who engage with them, and we have done our own external research to validate these numbers. Thus, the implementation of this program will lead to the decrease in expected mortality for participating policyholders.  

* <u>Increase Life Insurance Sales</u> 
  
  The discounts offered by SuperLifeStyle will aim to increase sales by attracting customers to SuperLife’s long-term insurance products; Lumarians who may not have considered purchasing these products before due to the price will now be able to access them at a price they would accept in exchange for participation.  

* <u>Improve Product Marketability and Competitiveness  </u>
  
  Similarly to the previous objective, the discounts offered by SuperLifeStyle will lower the effective price of long-term insurance for those willing to participate in the program, which will improve the marketability and competitiveness. 

* <u>Add Economic Value to Superlife</u>
  
    The reduction in mortality for participating policyholders will reduce their expected mortality and thus reduce the expected claims costs of these insurance products. The discounts offered by the scheme can be in the form of reduced premiums properly repriced in the hopes of increasing sales volume, or Superlife can choose not to reprice premiums and hold on to additional cost savings themselves. SuperLifeStyle will provide economic value through the increase in insurance sales and competitiveness of SuperLife’s products, as well as providing unique value in the form of health interventions that will separate Superlife from its competitors.

### Project Development Pipeline: <a name="pdp"></a>

<img title="" src="./Logos and Figures/Pipeline.png" alt="" width="450" data-align="inline">

We have determined that the reduction in claims costs from SuperLifeStyle’s mortality benefits will offset the implementation costs for term insurance between the ages of 23 and 84, and whole-life insurance for all ages above 23. This reduction in expenses will fund the premium discounts. The reduced costs and higher expected insurance sales from the discounts will create larger profits for SuperLife. 

### Pricing and Costs:

<img src="file:///Users/visweshnarayan/Library/Application%20Support/marktext/images/2024-04-08-09-13-27-image.png" title="" alt="" width="450">

The graph below indicates the lives that would have been saved if the program was implemented 20 years ago; the claims cost savings would have been Č11,491,341,272.57 for term insurance policies and Č58,051,148,810.82 for whole-life policies. The savings would increase to Č14,409,136,415.29 and Č131,818,490,081.97 after another 20 years. 

<img src="Logos%20and%20Figures/Cost%20reduction.png" title="" alt="Claims Cost Reduction" width="452">

<img title="" src="Logos and Figures/Lives saved.png" alt="Comparison of Lives Saved Now versus 20 Years prior" width="452">

Our analysis was limited by the data and assumptions we used as inputs. We primarily relied on data provided by SuperLife, such as the life table and mortality reduction figures; we have validated this data through reasonability checks and external research. To address the risk of inappropriately selected assumptions, we performed sensitivity testing which provided confidence that reasonable deviations in our assumptions would not significantly impact our findings. 

Alongside the sensitivity analysis, we have also considered several qualitative risks such as policyholders attempting to exploit the program without properly engaging. Mitigation strategies were listed in order to ensure the implementation of SuperLifeStyle comes with minimal risk.  

### Program Design <a name="design"></a>

<img src="./Logos%20and%20Figures/SuperLifeStyle%20Wellness%20Incentives.png" title="" alt="" width="450">

* **<u>Safety Campaigns</u>**<a name="safety"></a>
  
  Safety campaigns play a pivotal role in SuperLifeStyle, offering educational opportunities to policyholders on a variety of safety topics. These campaigns are designed to empower individuals with awareness, encouraging them to make more informed decisions. From fire safety and home security to road safety and health awareness, safety campaigns cover a broad spectrum of topics aimed at minimizing risks and protecting lives. SuperLife allocates approximately ˇC10 - ˇC35 per participant towards content development, including educational materials, infographics, videos, online modules, and in-person demonstrations. These resources are disseminated through various channels such as emails, social media, and websites, incentivizing participation with discounts to premiums.

* **<u>Community Fitness Challenges</u>**<a name="fitness"></a>
  
  SuperLife’s SuperLifeStyle scheme can provide incentives such as premium discounts, gift cards, or other rewards to stimulate engagement in fitness challenges. Beyond mere motivation for individual health priorities, SuperLife can integrate community fitness challenges with its term and life assurance offerings. This strategic bundling not only aims to reduce mortality rates but also to enhance sales, revenue, foster brand loyalty and engagement, and help SuperLife balance expenses and mortality reduction.

* **<u>Preventive Screening</u>**<a name="screen"></a>
  
  SuperLife can offer rewards to policyholders that undergo preventive screening programs, specifically those focused on cancers. Rewards include covering an annual screening session (ˇC32.5), and a reduction in yearly premiums for those that engage with the intervention (ˇC32.5). As most cancer related deaths occur beyond the age of 50, SuperLife can offer this intervention to policyholders above this age. Research supported mortality reduction figures roughly in-line with SuperLife’s own findings.

* **<u>Smoking Cessations</u>**<a name="cess"></a>
  
  This incentive encourages the quitting of smoking. Participants will be directed to facilities and services known to help with the cessation of smoking, such as individual and group counselling sessions, and nicotine replacement therapy. Successfully abstaining from smoking is required for the policyholder to be considered as engaging with this incentive.
  
  While short-term participation in these initiatives is enough to begin accessing the discounts, the impact to mortality from engagement will only become apparent over a much longer period, thus consistent long-term participation is a key requirement of the program. Participants who cease to engage will no longer receive discounts and may be required to pay back a portion of the premiums previously discounted.
  
  ### Incentive Finalization
  
  The selection process of these four incentives was as follows: we set up a model to rank the extensive list of incentives provided to us by SuperLife’s product development team based off the impact to mortality balanced by the cost of implementation and identified Safety Campaigns and Community Fitness Challenges as the two most effective. We then selected two more incentives that also ranked highly that addressed specific health concerns that we noticed had a large impact on SuperLife’s policyholder demographic; cancer is a leading cause of death for policyholders and thus Preventative Screening was selected, and a large portion of policyholders are smokers, so Smoking Cessation Programs was selected.
  
  These incentives were selected through external research, we were able to find details on how these health initiatives worked which aided in the construction of SuperLifeStyle’s logistics. We were also able to broadly validate the mortality impact and cost figures provided by SuperLife; this will be discussed further in the Data and Data Limitations section of the report. All sources are listed in the bibliography.

### Risk and Risk Mitigation Considerations <a name="risk"></a>

<style>
</style>

|                          |            |          |
| ------------------------ | ---------- | -------- |
| Risk                     | Likelihood | Severity |
| Inflation<br> (INF)      | 5          | 3        |
| Climate Change<br> (CC)  | 3          | 2        |
| Engagement<br> Rate (ER) | 5          | 1        |
| Pandemic<br> (PAND)      | 2          | 4        |
| War                      | 1          | 5        |

<img src="Logos%20and%20Figures/Picture 1.png" title="" alt="Claims Cost Reduction" width="452">



The implementation of SuperLifeStyle is accompanied by several key risks which this section will outline and discuss mitigation strategies for. 

* *<u>Climate</u>* – High Severity, Moderate Likelihood – Can lead to higher mortality rate due to heat related illnesses. 

* *<u>Inflation</u>* – Moderate Severity, High Likelihood – Persistently high inflation can curb spending as cost-of-living pressures will force potential customers to spend elsewhere which will affect SuperLifeStyle program performance and profits. 

* *<u>Pandemic</u>* – High Severity, Low Likelihood – Can exponentially increase mortality rate and cause a downturn in the economy leading to an adverse impact on the program and profits 

* *<u>Engagement Rate</u>* – Low Severity, High Likelihood – Low impact on results when inflation rates are fixed 

* *<u>War</u>* – High Severity, low Likelihood – Creates market volatility and potential increase in mortality rate amongst annuitants. Impacts economy adversely and leads to poor investment returns and profits 

#### Data and Limitations <a name="data"></a>

In order to check the reasonability of Superlife's in-house data, we have cross-validated it against two other data sources:

1. SuperLife In-Force Data

2. Australian Life Table

<style>
</style>

| Data Requirement     | Data Sources                                                     | Data Limitations                                                                                                                           |
| -------------------- | ---------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| Mortality rate       | Lumaria life table (Lumaria govt)                                | Life table provides mortality by age only<br> and does not provide mortality rates by sex or smoking status.                               |
| Mortality rate       | Policyholder mortality rates (in-force<br> policyholder dataset) | Mortality rates implied at the ends of the<br> age spectrum are weak estimates due to low sample size or low occurrences of<br> mortality. |
| Mortality Rate       | Australian Life Table                                            | Chosen due to similar characteristics to<br> Lumaria but may not be exact                                                                  |
| Economic Assumptions | Central Bank of Lumaria                                          | Not verified if inflation targeting practices were implemented                                                                             |

#### Sensitivity Analysis <a name="sens"></a>

<p float="left">
  <img src="./Logos and Figures/T20 Sens Analysis.png" width="300" />
  <img src="./Logos and Figures/SPWL Sens Analysis.png" width="300" />
</p>

A key quantitative risk is the incorrectness of assumptions used. To address this risk, sensitivity testing reveals reasonable results for moderate changes to the economic landscape in the form of interest rate and inflationr ate fluctuations.

### Final Recommendations

The proposed program adopts a holistic approach to health and wellbeing and offers SuperLife’s policyholders health-promoting activities to engage with. In addition to being informed by medical research, the quantitative modelling also reaffirms the projected success of the program from a mortality reduction and savings perspective. SuperLifeStyle will bring value to SuperLife in terms of competitiveness, marketability, and economic value and should gradually be scaled by SuperLife depending on the initial performance.

### Bibliography

Greenhalgh, EM, Scollo, MM and Winstanley, MH [editors]. *Tobacco in Australia: Facts and issues*. Melbourne: Cancer Council Victoria. Available from: tobaccoinaustralia.org.au/chapter-7-cessation/7-17-financial-incentives 

Engagement Rate: 

1. Swirr Re. (2022). “Health and Wellness Engagement Impact”. Retrieved from 2022-10-sr-swissre-health-engagement-impact-paper.pdf 

Preventative Screening: 

1. H.-O. Adami a, N.E. Day b, D. Trichopoulos c d, W.C. Willett e. (2001). Primary and secondary prevention in the reduction of cancer morbidity and mortality. *European Journal of Cancer.* Available from: Primary and secondary prevention in the reduction of cancer morbidity and mortality - ScienceDirect 
2. James A. Hanley, Measuring Mortality Reductions in Cancer Screening Trials, Epidemiologic Reviews, Volume 33, Issue 1, July 2011, Pages 36–45. Available from https://doi.org/10.1093/epirev/mxq021 

Ethical Considerations and Framework: 

1. Page K. The four principles: can they be measured and do they predict ethical decision making? BMC Med Ethics. 2012 May 20;13:10. doi: 10.1186/1472-6939-13-10. PMID: 22606995; PMCID: PMC3528420. Available from https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3528420/ 
2. Van Wolfren. J., Inbar K., Zeelenberg M. (2013). Moral hazard in the insurance industry. *Vetspar.* Available from researchgate.net/publication/235988864_Moral_hazard_in_the_insurance_industry 

Safety Campaigns: 

1. Aburumman, Mohammed & Newnam, Sharon & Fildes, Brian. (2019). Evaluating the effectiveness of workplace interventions in improving safety culture: A systematic review. Safety Science. 115. 376-392. 10.1016/j.ssci.2019.02.027. 
2. Newnam, Sharon & Muir, Carlyn. (2015). Effectiveness of Prevention-Focused, Workplace Health and Safety Campaigns. Institute for Safety, Compensation and Recovery Research 
3. Choi, Sung & Choi, Seo & Kwon, Soon & Pok, Jin. (2023). A Study on the Impact of Unsafe Behavior on Safety and Health Culture According to Workplace Safety and Health Education Experience. Forum of Public Safety and Culture. 25. 235-247. 10.52902/kjsc.2023.25.235. 

Australian Life Table: 

1. The Australian Government Actuary. (2019). Australian Life Tables 2015‑17. Available from https://aga.gov.au/publications/life-tables/australian-life-tables-2015-17