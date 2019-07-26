# Understanding rumination as a form of inner speech: probing the role of motor processes

An online (and a PDF) version of the thesis is available at https://www.barelysignificant.com/phd_thesis/.

## Abstract

Rumination is known to be a predominantly verbal process and has been proposed to be considered as such as a dysfunctional form of inner speech. On the other hand, research on the psychophysiology of inner speech revealed that the neural processes involved in overt speech and inner speech tend to be very similar. This is coherent with the idea that some forms of inner speech could be considered as a kind of simulation of overt speech, in the same way as imagined actions can be considered as the result of a simulation of the corresponding overt action (e.g., walking and imagined walking). In other words, the motor simulation hypothesis suggests that the speech motor system should be involved as well during inner speech production. The corollary hypothesis might be drawn, according to which the production of inner speech (and rumination) should be disrupted by a disruption of the speech motor system. We conducted a series of five studies aiming to probe the role of the speech motor system in rumination. Overall, our results highlight that although verbal rumination may be considered as a form of inner speech, it might not specifically involve the speech motor system. More precisely, we argue that rumination might be considered as a particularly strongly condensed form of inner speech that does not involve fully specified articulatory features. We discuss these findings in relation to the habit-goal framework of depressive rumination and we discuss the implications of these findings for theories of inner speech production.

<!--

Rumination is known to be a predominantly verbal process and has been proposed to be considered as such as a dysfunctional form of inner speech. On the other hand, research on the psychophysiology of inner speech revealed that the neural processes involved in overt speech and inner speech tend to be very similar. This is coherent with the idea that some forms of inner speech could be considered as a kind of simulation of overt speech, in the same way as imagined actions can be considered as the result of a simulation of the corresponding overt action (e.g., walking and imagined walking). In other words, the motor simulation hypothesis suggests that the speech motor system should be involved as well during inner speech production. The corollary hypothesis might be drawn, according to which the production of inner speech (and rumination) should be disrupted by a disruption of the speech motor system.

We conducted a series of five studies aiming to probe the role of the speech motor system in rumination. In Study 1, we used surface electromyography to examine the involvement of the speech motor system during induced rumination. We observed that induced rumination was associated with increased facial (lips and forehead) muscular activity as compared to rest. Moreover, an orofacial relaxation was more efficient in decreasing self-reported state rumination than a non-orofacial relaxation. These results taken together suggest that rumination might be considered as a form of inner speech recruiting the speech motor system. In Study 2, we induced rumination in either a verbal or a non-verbal modality to compare their electromyographic correlates. Our results shown that i) the induction of rumination in different modalities was not successful but that ii) comparing (a posteriori) groups of verbal versus non-verbal ruminators did not reveal differences in their electromyographic correlates. Moreover, a comparison of an orofacial relaxation to a non-orofacial relaxation (as in the first study) revealed an opposite pattern of results to those of Study 1. In Study 3, we compared the electromyographic correlates of both overt speech and inner speech production of two classes of nonwords. An automatic classification approach was undertaken to discriminate these signals according to the class of nonword to be uttered. Although this approach lead to reasonable accuracy rates during overt speech production, it failed to discriminate inner speech content based on surface electromyography signals. In Study 4, we used articulatory suppression to test the involvement of the speech motor system during rumination. Self-reported levels of state rumination showed a decrease after both motor activities (silent mouthing vs. finger-tapping), with only a slightly stronger decrease after the articulatory suppression than the control task. Importantly, the rumination level decrease was not moderated by the modality (verbal vs. non-verbal) of the ruminative thoughts. In Study 5, we induced either rumination or a more constructive form of repetitive thinking (problem-solving). We compared the effects of articulatory suppression to a control induction on self-reported state rumination and state affects following each thinking-style induction. Preliminary results suggest no stronger effect of articulatory suppression (chewing) in reducing self-reported state rumination as compared to finger-tapping.

Overall, these results highlight that although verbal rumination may be considered as a form of inner speech, it might not specifically involve the speech motor system. More precisely, we argue that rumination might be considered as a particularly strongly condensed form of inner speech that does not involve fully specified articulatory features. We discuss these findings in relation to the habit-goal framework of depressive rumination and we discuss the implications of these findings for theories of inner speech production.

-->

## Technical notes

My dissertation is a book based on R Markdown and **bookdown**
(<https://github.com/rstudio/bookdown>, <https://bookdown.org/>). This bookdown project was originally a fork of the demo book
(<https://github.com/rstudio/bookdown-demo>) and is largely inspired by Tristan Mahr's own dissertation: <https://github.com/tjmahr/dissertation/blob/master/README.md>.

Some things I have changed from previous versions of the template.

* I deactivated the default TOC from bookdown and defined a custom one in `00-toc.Rmd` to be able to define the order of the `00-*.Rmd` files (e.g., abstract, preface, etc.).

* I deactivated the default references manager (i.e., natbib or biblatex) to be able to provide a .csl file for the references (`citation_package` in `_output.yml` needs to be `none`). See the `pandoc_args` in the `_output.yml` file.
