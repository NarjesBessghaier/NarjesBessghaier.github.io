---
title: "On the prevalence, co-occurrence, and impact of infrastructure-as-code smells"
collection: publications
date: 2024/3/12
venue: '2024 IEEE International Conference on Software Analysis, Evolution and Reengineering (SANER)'
paperurl: 'https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10589858'
citation: 'Bessghaier, N., Begoug, M., Mebarki, C., Ouni, A., Sayagh, M., & Mkaouer, M. W. (2024, March). On the prevalence, co-occurrence, and impact of infrastructure-as-code smells. In 2024 IEEE International Conference on Software Analysis, Evolution and Reengineering (SANER) (pp. 23-34). IEEE.'
---
In modern software systems, Infrastructure-as-Code
(IaC) tools play a pivotal role in automating the management
of various infrastructure resources such as networks, databases,
and services. This automation is done through code-based specification files, commonly known as IaC files. Similarly to other
code files, IaC files can suffer from violations of established
implementation and design standards, i.e., IaC smells. Although
prior research has studied various aspects of traditional smells
in non-IaC artifacts, there is little knowledge of how IaC
smells are prevalent, co-occurring, and impacting the change
and defect proneness of IaC code. To fill this gap, we conduct
an empirical study encompassing 82 Puppet-based open-source
projects. Our investigation focused on 12 types of IaC smells
in both implementation and design levels. Our findings reveal
that IaC smells do not manifest uniformly, as IaC smells that
are particularly associated with modularity issues, exhibit high
prevalence rates across projects. Additionally, we found that 74%
of IaC files are smelly and over 52% of the smelly IaC files have
at least two co-occurring IaC smells. Furthermore, our findings
highlight that, on average, smelly IaC files are modified nearly
3.8 times, in terms of number of commits, more frequently than
non-smelly IaC files. Furthermore, smelly IaC files are found to
be 3.1 times more prone to larger code changes, in terms of code
churn, than non-smelly IaC files. Additionally, we found that
smelly IaC files are 3.3 times more prone to the introduction of
defects that are likely to persist in 1.65 more commits before
being fixed than non-smelly IaC files. These findings advocate
developers to be more aware of IaC smells in their projects and
consider their correction
