
<!-- README.md is generated from README.Rmd. Please edit that file -->

### Estimating reproductive rates and juvenile survival when offspring ages are uncertain: a novel multievent mark-recapture model applied to an endangered beluga whale population

#### Himes Boor, G.K., T.L. McGuire, A.J. Warlick, R.L. Taylor, S.J. Converse, J.R. McClung, A.D. Stephens

For questions regarding the code, contact [Gina Himes
Boor](mailto:gkhimesboor@montana.edu)

#### Citation:

Himes Boor, G.K., T.L. McGuire, A.J. Warlick, R.L. Taylor, S.J.
Converse, J.R. McClung, A.D. Stephens. Estimating reproductive rates and
juvenile survival when offspring ages are uncertain: a novel multievent
mark-recapture model applied to an endangered beluga whale population.

------------------------------------------------------------------------

#### Abstract

1.  Understanding the survival and reproductive rate of a population is
    critical to determining its long-term dynamics and viability. For
    some hard-to-study species, obtaining the mark-recapture data
    necessary to estimate vital rates can be difficult or impossible,
    particularly for reproductive rates. Existing models cannot
    currently accommodate data from populations in which offspring are
    not always detected, remain with parents for multiple years, and
    cannot be aged with certainty.
2.  To address this, we developed a novel multievent mark-recapture
    model that uses all available adult and adult-offspring sightings,
    including sightings with older offspring of uncertain age. To
    illustrate the model, we applied it using a Bayesian framework to
    thirteen years of photo-ID data from a critically endangered
    population of beluga whales (Delphinapterus leucas) to estimate
    reproductive rates, and survival rates for breeding females,
    non-breeders (male and female), and calves. We also evaluated model
    performance using simulated data under varying sample sizes, and
    adult and calf detection rates.
3.  Applying our model to the beluga data yielded reasonably precise
    estimates for all demographic rates of interest and provided new
    insight into proximate causes of the population???s decline. Our
    estimates indicated that non-breeder survival (0.962; 95% credible
    interval: 0.945 ??? 0.975) and reproductive rates for breeders that
    had not given birth the previous year (0.279; 0.226 ??? 0.34) are low
    relative to other belugas and likely contributing to negative
    growth. Breeding female survival (0.962; 0.945 ??? 0.975) was
    marginally low and could also be a factor in the population???s
    decline. Our simulation analysis indicated the model is
    asymptotically unbiased. Even at moderate sample sizes and detection
    rates it estimated ecological parameters of interest with good
    precision and low bias.
4.  This work yields an important new development in multievent
    mark-recapture modeling, allowing estimation of reproductive rates
    and juvenile survival for populations with extended adult-offspring
    associations and uncertain offspring ages, such as other marine
    mammals, elephants, and some great apes, bats, and birds.
    Additionally, our model provides new robust demographic rate
    estimates for an endangered population that were previously
    inestimable and that will enable new insights into the population???s
    decline and its causal mechanisms.

------------------------------------------------------------------------

#### CODE:

**Model:**  
[CIBW\_ME\_Model-ms\_code.R](scripts/CIBW_ME_Model-ms_code.R): R code
for the multievent mark-recapture model developed to estimate survival
and reproductive rates from the Cook Inlet beluga whale photo-ID data,
and that can be adapted for other data with similar characteristics
(i.e., mark-recapture study involving marked adults that are sometimes
observed with their unmarked offspring of unknown age).

**Simulations:**  
[CIBW\_ME\_sim.R](scripts/CIBW_ME_sim.R): R code for the accompanying
simulation analysis for the multievent mark-recapture model examining
model performance across varying detection rates and sample population
sizes.

#### DATA:

[ms\_SH\_data.csv](inputs/ms_SH_data.csv): formatted Cook Inlet beluga
whale photo-ID mark-recapture data for running the multievent model
described above. The data were collected by Dr.??Tamara McGuire and
colleagues at [The Cook Inlet Beluga Whale Photo-ID
Project](https://www.cookinletbelugas.com/) and should not be used
outside of this analysis without express permission from
[Dr.??McGuire](mailto:tamaracookinletbeluga@gmail.com).

#### Additional Required Files:

[start\_mat-ms\_SH\_data.csv](inputs/start_mat-ms_SH_data.csv):
formatted starting latent matrix required by JAGS to run the multievent
model (see [Inputs README file](inputs/README.md) for more information
about this file)

------------------------------------------------------------------------

#### Funding

Funding for development of this model came from the [North Pacific
Research Board](https://www.nprb.org/) (project \# 1718). Cook Inlet
beluga photo-ID data were collected using a wide range of funding
sources.
