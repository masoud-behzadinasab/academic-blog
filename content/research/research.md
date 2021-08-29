---
widget: blank
headless: true

weight: 10  # section position on page
design:
  columns: '1'

---

<style>
img {
  color: white;
  padding: 16px;
}
</style>

I consider the best of different numerical methods to build accurate, efficient, and robust predictive frameworks for tackling a variety of engineering challenges. My research involves usage and development of meshfree models (e.g. peridynamics), Galerkin methods (e.g. Isogeometric Analysis), and data-driven techniques (e.g. Neural Networks) for simulating the response of solid structures and fluid flows in extreme conditions (e.g. blast events).

<h2><span style="display:block; margin-top:30px; font-weight: bold;">Ductile Fracture Modeling in Additively Manufacture Metal with Peridynamics</span></h2>

<p>
<figure>
  <img align="right" Padding="210px" src="./figures/SFC.png" width="700">
</figure>
  
<p style='text-align: justify;'> 
  The peridynamic theory (PD) has shown promising capabilities in handling material failure without any complicated numerical treatments at material discontinuities (e.g. cracks and fracture). PD has been widely applied to a broad range of challenging problems, mostly involving brittle fracture. However, its applications to predicting ductile fracture remains largely untested. The third Sandia Fracture Challenge (SFC3) was seen as an opportunity to assess the state of the art of the theory in predicting the response of an additively manufactured 316L stainless steel bar with a complex geometry under the dynamic tensile experiments performed by Sandia National Laboratories (SNL). The performance of a recently developed finite deformation PD model coupled with a ductile fracture theory was explored over this problem. An iterative inverse technique was applied to calibrate the model parameters using the longitudinal and notched tensile tests data provided by SNL. A blind prediction of the deformation and failure behavior of the SFC3 geometry was performed by embedding the calibrated formulation in a PD simulation. Uncertainty was introduced into the model parameters to quantify material variability. We observed that while the modeling approach led to qualitatively good results and a correctly predicted crack path, it underpredicted the load-carrying capacity of the structure and simulated an early fracture. Our post-experiment analysis identified material instability issues associated with the model as the primary sources of error. As a remedy, we proposed a bond-associated, semi-Lagrangian PD formulation that is stable under large inhomogeneous deformation. The new method was tested by revisiting the challenge problem in a blind-prediction approach. We obtained significantly improved predictions of ductile fracture phenomenon in this challenge using the new technique.

  <span style="display:block; margin-top:20px; margin-bottom:-12px;">**Selected Publications**</span>

  -  <a href="https://link.springer.com/article/10.1007/s10704-020-00455-1">Revisiting the Third Sandia Fracture Challenge: A Bond-Associated, Semi-Lagrangian Peridynamic Approach to Modeling Large Deformation and Ductile Fracture</a>, <i>International Journal of Fracture</i>, 2020. 
  -  <a href="https://www.sciencedirect.com/science/article/pii/S0022509619309512">A Semi-Lagrangian Constitutive Correspondence Framework for Peridynamics</a>, <i>Journal of the Mechanics and Physics of Solids</i>, 2020. 
  -  <a href="https://www.sciencedirect.com/science/article/pii/S0020768319303506">On the Stability of the Generalized, Finite Deformation Correspondence Model of Peridynamics</a>, <i>International Journal of Solids and Structures</i>, 2020. 
  -  <a href="https://link.springer.com/article/10.1007/s10704-019-00361-1">The Third Sandia Fracture Challenge: Predictions of Ductile Fracture in Additively Manufactured Metal</a>, <i>International Journal of Fracture</i>, 2019. 
  -  <a href="https://link.springer.com/article/10.1007/s10704-019-00363-z">The Third Sandia Fracture Challenge: Peridynamic Blind Prediction of Ductile Fracture Characterization in Additively Manufactured Metal</a>, <i>International Journal of Fracture</i>, 2019. 
</p>
</p>



<h2><span style="display:block; margin-top:30px; font-weight: bold;">Mesoscale Simulation of Granular Materials under Shock Loading using Peridynamics</span></h2>

<p>
<figure>
  <img align="right" Padding="210px" src="./figures/granular.png" width="700">
</figure>
  
<p style='text-align: justify;'> 
  The behavior of granular materials under penetration is fundamental to many industries including civil, energy, and defense. Although there is considerable literature on experimental and numerical research on the dynamics of granular matter under impact loading, the behavior is still not well understood. One way to gain more insights into the continuum-scale physics is to study the underlying scales. Mesoscale modeling can be adopted to explicitly resolve the deformation of individual grains, their interactions with each other or the surrounding fluid (e.g., air or water). We have developed a meshfree computational framework for Lagrangian peridynamic-based mesoscale simulation of granular particles under shock loading. We explicitly consider intra-granular fracture and inter-particle contact and friction in our modeling approach. In this study, we simulated the shock wave perturbation decay experiment, which is a technique that involves monitoring the evolution of a perturbation in a shock wave front as it propagates through a material field and has been explored to probe the high-rate shear response of granular materials. We conducted a systematic investigation of the effects of grain fracture and frictional contact forces between grains on the continuum behavior of granular materials. A sensitivity assessment of dominant factors indicates that grain fracture, a phenomenon ignored in most computational investigations of granular materials, plays a large role in the bulk dynamic response. Our results show that the wave propagates faster with an increase in the toughness of the material and the inter-particle friction. Also, the shock amplitude is shown to decay faster in tougher materials. It is further confirmed that under strong compression self-contact among fractured grain sub-particles cannot be neglected. 


  <span style="display:block; margin-top:20px; margin-bottom:-12px;">**Selected Publications**</span>

  -  <a href="https://link.springer.com/article/10.1007/s40870-018-0174-2">Peridynamics Modeling of a Shock Wave Perturbation Decay Experiment in Granular Materials with Intra-Granular Fracture</a>, <i>Journal of Dynamic Behavior of Materials</i>, 2018. 
  -  <a href="https://aip.scitation.org/doi/abs/10.1063/1.5044814">Modeling Perturbed Shock Wave Decay in Granular Materials with Intra-Granular Fracture</a>, <i>AIP Conference Proceedings</i>, 2018. 
  -  <a href="https://www.osti.gov/servlets/purl/1348102">Perturbation Decay Experiments on Granular Materials</a>, <i>Sandia National Lab. (SNL-CA)</i>, 2016. 
</p>
</p>


