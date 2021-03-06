

# Approaches for Effect Size Estimation and Synthesis of Single-Case Designs {#intro}

This chapter provides the background and purpose for this methods guide. It also gives an overview of the three major approaches for estimation and synthesis of single-case studies: 

a) design-comparable effect sizes, 
b) case-specific effect sizes, and 
c) multilevel modeling of the raw individual participant interrupted time-series data. 

We describe the motivation and rationale for each of these approaches and provide a series of decision rules to guide researchers in selecting among them. The remaining chapters provide details and illustrations of the methods. 

## Background

Educational decisions at the state, district, school, and student level are now expected to be informed by empirical evidence [@2014Council; @whatworksclearinghouse2020What]. 
These expectations create a major need for synthesis, or the integration of research findings from multiple, existing sources of evidence—including findings from single-case designs (SCDs). [@cooper2010Research; @pustejovsky2017Research]y developments in education related to the documentation of evidence-based practices. 
The first is the expanded use of SCD research methods across varying disciplines over the last 50 years, in both general and special education contexts [@kratochwill2013SingleCase]. 
Although the history of SCD methodology is beyond our present scope, innovations in design have expanded the use of SCDs across a range of professional fields, moving beyond SCD’s quasi-experimental and behavior analysis origins [see @kratochwill2013SingleCase for more detailed information on the history of SCD].
Over the past 20 years, researchers' commitment to using rigorous procedures to identify evidence-based educational practices affirms not only the importance of randomized control trials (RCTs), but the effectiveness and efficiency of SCD. 

The second development is the emergence of effect size (ES) measures and synthesis methods for use with SCD and other interrupted time series data [@shadish2015Role; @Swaminathan2014effect]. 
Interest in synthesis of SCDs is long-standing [e.g., @Center1985methodology; @Gingerich1984meta; @White1987some], emerging around the same time as methods for meta-analysis of group designs were becoming more statistically rigorous and sophisticated [@hedges1985statistical; @shadish2015metaanalytic]. 
However, the past twenty years have seen increased intensity of methodological research focused on SCDs and a substantial expansion in the diversity, flexibility, and accessibility of available analytic methods upon which researchers can draw. 
We view the current state of methodology as falling into three strands: 

a) approaches that summarize the effect of each case and then synthesize these case-specific effect sizes [e.g., @pustejovsky2018Using], 
b) methods that use multi-level models for analyzing the raw (or standardized) data from one or multiple SCD studies [@VandenNoortgate2008multilevel], and 
c) techniques that use design-comparable effect size metrics [@Hedges2012ABk; @Hedges2012MB; @Pustejovsky2014design; @Shadish2013d; @Swaminathan2014effect]. 

The present guide is organized around these three broad methodological strands. 

The third development is the increased use of systematic review and meta-analysis procedures to identify and affirm evidence-based practices in education [@Beretvas2008review; @Shadish2007methods]. 
Maggin and colleagues [-@maggin2011Quantitative] examined the production of systematic reviews and meta-analyses of SCDs from 1985 to 2009, finding a marked increase in the appearance of such reviews between 2000 and 2009. 
In another survey, Jamshidi and colleagues [-@jamshidi2018Methodological] found increasing production through 2015, as well as improvements in the quality of published reviews. 
However, they also noted that, even in more recent literature, reviews often frequently failed to use appropriate methods for combining findings across studies [@jamshidi2018Methodological]. 
Thus, there remains a need for guidance about how to select and apply methods for synthesizing findings from SCD research.

Effect size (ES) measures are a critical companion to visual analysis for the interpretation of single-case research results, and are a key input in two of the available approaches for meta-analytic synthesis of SCDs.
Although a variety of technically sound ES metrics exist for researchers to use when interpreting SCD findings, relatively few published meta-analyses use these more advanced techniques [cf. @barton2017TechnologyAided; @Maggin2017meta-analysis; @jamshidi2018Methodological]. 
One reason for the lack of widespread use by researchers may be the conceptual and procedural complexity associated with advances in ES measures and meta-analysis techniques. 
A more rapid uptake of ES estimation methods may be hindered by the complexity of data extraction and calculation of ES for SCD. 
In addition, researchers may lack software tools for ES estimation for single-case studies when using some common statistical packages such as SPSS and SAS [@odom2018Betweencase; @Pustejovsky2014design; @shadish2015Role]. 

## Purpose of the Methods Guide

The purpose of this methods guide is to improve educational researchers’ practice in the estimation of ES measures and synthesis of findings from SCDs. 
We recognize that no single method is ideal for all research goals. 
Furthermore, methods that have the most to offer can be complex and may appear difficult to carry out. 
Thus, through the use of this methods guide, we aim to: (a) provide guidance and decision rules to simplify the process of selecting effect size estimation and synthesis methods and (b) illustrate the step-by-step application of appropriate methods using readily available tools, such as web-based software to calculate case-specific ES or design-comparable ES for SCD studies [e.g., @pustejovsky2021scdhlm].

## Study Quality

Conducting a research synthesis (whether of group design studies, SCDs, or both) involves several stages, starting with formulating the research aims, specifying inclusion criteria, conducting a systematic search, and screening for eligible studies [@cooper2010Research; @pustejovsky2017Research]. 
Additionally, before carrying out effect size calculations or meta-analysis, it is critical to consider the methodological quality and potential biases of studies to be included in the synthesis. 
To assist researchers in doing so, several distinct sets of standards are available for SCD studies [e.g., @kratochwill2013SingleCase; @reichow2018Development; @tate2016SingleCase; @zimmerman2018Singlecase]. 
After assessing methodological quality, researchers can use one of two strategies to guide the estimation and synthesis of effect sizes. 
One strategy incorporates consideration of study quality as an inclusion criteria, so that low-quality studies are screened out and synthesis is based on the subset of studies with quality high enough so that changes in outcome(s) can reasonably be attributed to the intervention. 
For example, the What Works Clearinghouse Single-Case Pilot Standards [@Kratochwill2010single] indicated that effect sizes are only to be computed after studies have been shown to meet both minimum design criteria (e.g., a multiple-baseline study has at least three temporally spaced opportunities for the effect to be demonstrated, along with phases of at least three observations) and minimum evidence criteria (e.g., visual analysis of the data from the study show experimental control so that the changes in the outcome can be attributed to the intervention). 
Concerns with estimating effect sizes for SCD studies without the use visual analysis to rule out alternative explanations for observed changes in the outcomes continues to be echoed in the literature [@kratochwill2021Singlecase; @maggin2021Commentary]. 
An alternative strategy in considering study quality is to use broader inclusion criteria, code for aspects study quality, and examine study quality codes as potential moderators in a meta-analysis. 
With this approach, researchers can estimate ESs for studies of varying degrees of quality and empirically explore whether the magnitude of ESs varies depending on aspects of study quality. 

We assume that researchers who use this methods guide will have already selected a method to assess study quality and an approach for incorporating those assessments into their synthesis. 
As such, we do not focus on SCD study quality assessment methods, but rather provide guidelines that can be applied to a collection of studies that have met the researchers' inclusion criteria, which potentially include criteria related to study quality. 
Thus, in this guide we focus on the final stages of a research synthesis, on the questions of how to select a method for estimating effects, how to compute ES estimates (or otherwise prepare data for synthesis), and how to synthesize findings in the form of ES estimates or individual-level data. 

## Selecting an Approach for Effect Estimation and Synthesis

In order to select an approach for estimating and synthesizing effects from SCDs, we recommend that researchers first reflect on the research aims that motivate their synthesis. 
In some contexts, researchers’ primary aims may be focused on summarizing evidence to arrive at statements about average efficacy of a class of interventions. 
In other contexts, researchers might instead or additionally be interested in understanding variation in effects and the extent to which such variation is associated with characteristics of participants, specific features of interventions, or other contextual factors. 
When the focus is mostly on summarization, researchers may find it more useful to use design-comparable effect sizes that describe average effects. 
If individual-level variation is the focus, then approaches using case-specific effect sizes or multi-level modeling may be more advantageous. 

Another over-arching consideration for selecting a synthesis approach pertains to the features of the studies identified for inclusion in the synthesis. 
Quantitative synthesis requires choosing an effect size metric that permits comparisons of the magnitude of effects across individual participants and studies. 
Consequently, the extent to which eligible studies use different types of designs or different types of outcome measurements creates constraints on how effects from those studies can be described or compared. 
For instance, if all eligible studies used multiple baseline designs across participants (or another common type of SCD), then several different synthesis approaches are feasible. 
In contrast, if eligible studies include both SCDs and group design studies (such as small randomized experiments, each with a single pre-test and a single post-test), then researchers need a synthesis approach that permits comparisons across both types of designs. 
Similarly, if all eligible studies used SCDs with very similar methods for assessing the dependent variable, then synthesis based on multi-level modeling of raw data is possible. 
In contrast, if eligible studies used a variety of different assessments, then a synthesis approach based on case-specific effect sizes may be required. 

These two broad considerations—the aims of the synthesis and the features of eligible studies—can guide the selection of an approach for synthesis of SCDs. 
We now describe in more detail how three broad approaches to synthesis fit within these considerations. 

### Design-Comparable Effect Sizes

In some situations, the aim of the research team is to synthesize the evidence for intervention effectiveness from both single-case and group design studies. 
For example, a meta-analysis by Wood and colleagues [-@wood2018Does] analyzed 22 single-case and between-group studies to examine the effects of text-to-speech and other read-aloud tools on reading comprehension outcomes for students with reading disabilities. 
The authors used the standardized mean difference to estimate read-aloud intervention effects in the group design studies and a comparable standardized mean difference from the included single-case research, resulting in an overall average weighted effect size of $d$ = 0.35, 95% CI (0.14, 0.56). 
Because the purpose of the @wood2018Does study involved the comparison and averaging of effects across single-case and group designs, it was critical to use an ES metric that is theoretically comparable across the designs. 
In similar situations, researchers should select from the design-comparable effect size options [@Hedges2012ABk; @Hedges2012MB; @Pustejovsky2014design; @Shadish2013d; @Swaminathan2014effect; @VandenNoortgate2008multilevel]. 
However, if researchers aim to synthesize findings from only single-case studies (i.e., not to integrate findings across single-case and group design studies), other options may be preferable.

### Case-Specific Effect Sizes 

In addition to summarizing average effects across studies, researchers may also be interested in exploring variation in treatment effects across individual participants. 
When dependent variables are measured differently across studies, it is important for researchers to use an effect size metric and synthesis approach that accounts for such. 
For example, Bowman-Perrott and colleagues [-@bowman-perrott2016Promoting] examined five potential moderators of the effectiveness of the Good Behavior Game in promoting positive behavior in the classroom. 
Results of their meta-analysis suggested that the intervention was most effective in reducing problem behaviors among students with or at risk for emotional and behavioral disorders. 
Another meta-analysis by Mason and colleagues [-@mason2016Video] investigated the moderating effects of participant characteristics, targeted outcomes, and implementation components on the efficacy of video self-modeling, in which a learner with disabilities watches a video of a model engaged in targeted skills or tasks. 
They found that intervention effects were stronger for younger participants with autism-spectrum disorders. 

Because these syntheses focused on investigating variation across individuals in the effect of treatment, it was important that the effect size estimation and synthesis approach produced effect estimates for each individual participant, rather than a study-level summary effect estimates. 
In addition, because the outcome measure differed among studies, the researchers needed an individual-level effect size metric that is not scale-dependent (e.g., they could not be based on simple raw score mean differences). 
In contexts like these, researchers should consider selecting among the case-specific effect size estimation and synthesis options. 
The case-specific effect size options are not viable for synthesis across single-case and group design studies because the case-specific effects are not comparable to the group design effects. 
However, the design-comparable effects are not viable for studying within-participant variation between individuals in treatment effectiveness because they produce effect estimates at the study level (i.e., the effect averaged across the cases), not the individual level. 

### Multilevel Modeling of Individual Participant Interrupted Time-Series Data

Finally, researchers might have identified a set of SCDs that all use the same or very similar outcome measures, with the aim of studying the variation in effects over time within and between individuals. 
For example, Datchuk and colleagues [@datchuk2020Level] meta-analyzed 15 single-case studies with 79 students to examine the effects of an intervention on the level and trend in correct writing sequences per minute for students with disabilities. 
They found the effect increased with time in intervention (i.e., there was a positive effect on the trend) and that this temporal change in effect was more pronounced with younger students. 
When focusing on both variation in effect over time and variation in effect across cases, it is important that the researchers select a meta-analytic approach that does not rely only on a single effect estimate for a study (e.g., design-comparable effect sizes) or even a single effect estimate for a case (e.g., case-specific effect sizes). 
In contexts like this, we suggest researchers consider options for multilevel modeling of individual participant data series. 

### Summary of Options for Effect Estimation and Synthesis 

The flow chart in Figure \@ref(fig:synthesis-flow-chart) illustrates a set of heuristic decision rules for selecting among the three general approaches to estimating and synthesizing single-case research. 
If the primary purpose of one’s research is to integrate findings from both single-case and group-design studies, the researcher should consider design-comparable effect sizes. 
Alternately, if the primary purpose of the research is to integrate findings from SCDs only, additional questions should be addressed related to the measurement of the dependent variable. 
If the outcome of interest is measured in different ways for different cases and the researcher aims to examine how effects vary across the cases, then the researcher should consider the options for estimating and synthesizing case-specific effect sizes. 
If the outcome is measured the same way across cases, and there is interest in how the effect changes over the course of an intervention, the researcher should consider multilevel modeling of the raw data series. 


<div class="figure">
<img src="images/Synthesis-flow-chart.png" alt="Flow chart showing the approach for synthesizing effect evidence based on the types of studies being examined and whether the outcome variable is common across cases."  />
<p class="caption">(\#fig:synthesis-flow-chart)Flow chart showing the approach for synthesizing effect evidence based on the types of studies being examined and whether the outcome variable is common across cases.</p>
</div>

### Limitations in Selecting an Approach for Effect Estimation and Synthesis

We emphasize that Figure \@ref(fig:synthesis-flow-chart) presents a heuristic, simplified procedure for the selection among the three general approaches to ES estimation and synthesis, which does cover every possible research context. 
There will surely be situations where researchers’ aims and contexts differ from those we describe, and thus do not align perfectly with one of our primary approaches to estimating and synthesizing single-case effect sizes. 
For example, researchers who are synthesizing findings from a set of SCDs may wish to compare their results to a previously published meta-analysis of group design studies, but not to investigate individual-level variation in treatment effects. 
They may therefore elect to use design-comparable effect sizes even though they are not formally integrating results from group design studies within their review. 

A further possibility is that researchers might elect to use multiple approaches to synthesis in order to address different aims or questions. 
For example, consider a project in which researchers have identified both single-case and group design studies. 
They might want to integrate findings across design types while also exploring the variation in effects among individuals. 
In this scenario, researchers could estimate design-comparable effect sizes for their first aim and case-specific effect sizes from the subset of single-case studies for their second aim. 

We also note that there may be situations that falls in between those we described for case-specific effect sizes and those for multilevel modeling of the raw data series. 
For example, researchers may want to examine how effects vary over time and across cases, using studies with different outcomes. 
For this purpose, the researchers can use extensions of the primary approaches we present. 
The researchers could either standardize the raw data before estimating a multilevel model, or they could synthesize case specific effect sizes where they use multiple standardized effects for each case (e.g., an effect that indexes the immediate shift in level, and another effect that indexes a change in slope). 
Our simplified selection method cannot exhaustively cover all currently available options. 

Finally, we anticipate that the heuristic guidance we provide here will need to be refined over time, as further methodological innovations become available. 
We anticipate that research presently underway will provide even more meta-analytic options in the future, with implications for how to select an approach for synthesis. 
At some point it may be possible to compute case-specific effect sizes that are also design-comparable, or it may be possible to standardize the data for multilevel models in a way that leads to parameter estimates from the model that correspond to design-comparable effect estimates. 
If such methods become available, some of the distinctions made here will become artificial. 
In the time, remainder of this methods guide follows the proposed heuristics for selecting among the three major approaches to effect size estimation and synthesis. 
Even as methodology continues to advance, researchers need guidance that acknowledges the complexity of research purposes and contexts and is dynamic in its accommodation of such variation, while also being concrete and straightforward enough to be put into practice. 

## Structure of the Methods Guide

We divide the remainder of this guide into three major sections: 

a) design-comparable effect size estimation and synthesis, 
b) case-specific effect size estimation and synthesis, and 
c) multilevel modeling to estimate and synthesize effects. 

These sections do not build upon each other or need to be read in order. Rather, we expect those using this guide to follow the decision rules in Figure \@ref(fig:synthesis-flow-chart) to determine which section of the guide is most appropriate for them, and then to jump immediately to that section. 

Each major section is divided into chapters. 
The initial chapter of each section introduces the specific approach and its assumptions, discusses when to use it, and what options exist within the approach. 
Furthermore, we provide additional decision rules for selecting among the specific techniques and options available with a given broad approach. 
We encourage researchers to use the decision rules within the initial chapter of the major section to get to an appropriate option. 
Then, researchers can directly refer to the chapter that has the illustration for that specific option. 
For each illustration, we: 

1) describe the purposes for estimating and synthesizing effects, and the available data, 
2) demonstrate how to use the decision rules in Figure \@ref(fig:synthesis-flow-chart), along with the additional decision rules within the initial chapter of the major section, to arrive at the option being illustrated, 
3) present the data for the illustration showing how it needs to be structured for the analysis, and 
4) provide a step-by-step illustration of how to estimate and synthesize effects using readily available analysis tools. 
