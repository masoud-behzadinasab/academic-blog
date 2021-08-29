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

I consider the best of different numerical methods to build accurate, efficient, and robust predictive frameworks for tackling a variety of engineering challenges. My research involves the usage and development of meshfree models (e.g. peridynamics), Galerkin methods (e.g. Isogeometric Analysis), and data-driven techniques (e.g. Neural Networks) for simulating the mechanical response of different materials, solid structures, and fluid flows in extreme conditions (e.g. large deformation, fracture, and fragmentation events).



<h2><span style="display:block; margin-top:30px; font-weight: bold;">A Peridynamic Model for Large Deformation and Failure Analysis of Thin-Walled Shell Structures</span></h2>

<p>
<figure>
  <img align="right" Padding="210px" src="./figures/PDshell.png" width="700">
</figure>
  
<p style='text-align: justify;'> 

Low-weight components are widely used in the design of engineering structures, where it is preferable to keep the structural weight low by using high-strength material (e.g., aircraft). These structures - having through-thickness dimension much smaller than the other two - are referred to as <i>shell structures</i>. Despite great progress made over the years to develop both structural shell theories and their discretization, challenges remain to efficiently and accurately predict the shell structural response under extreme loading conditions exhibiting large deformation and material failure using existing computational methods and tools. We have recently developed a comprehensive rotation-free Kirchhoff--Love (KL) shell formulation based on peridynamics (PD) that is capable of modeling large elasto-plastic deformations and fracture in shell structures. PD has been in development since 2000 and has shown great potential in simulating autonomous crack growth in solid materials without complicated numerical treatments. In our model, the KL equations of motion are formulated in terms of the midsurface displacement degree-of-freedoms (DOFs) without the need to introduce rotational DOFs and is thus more computationally efficient. To remove the need for a predefined global parametric domain, we employ Principal Component Analysis in a meshfree setting to develop a local parameterization of the shell midsurface. The KL shell kinematics is utilized to develop a correspondence-based PD formulation. A bond-stabilization technique is employed to naturally achieve stability of the discrete solution. By calculating the velocity gradient tensor using a higher-order meshfree gradient operator, 3D rate-form material models are employed to enable simulating a wide range of material behavior. A bond-associative damage correspondence modeling approach is adopted to use classical failure criteria at the bond level, which readily enables the simulation of brittle and ductile fracture. Discretizing the model with asymptotically compatible meshfree approximation provides a scheme which converges to the classical KL shell model while providing an accurate and flexible framework for treating fracture. Via a wide range of numerical benchmarks, ranging from elastostatics to problems involving plasticity, fracture, and fragmentation, we have validated the accuracy, convergence, and robustness of the developed PD thin-shell formulation. It is also worth noting that the present method naturally enables the discretization of a shell theory requiring higher-order smoothness on a completely unstructured surface mesh.

  <span style="display:block; margin-top:20px; margin-bottom:-12px;">**Selected Publications**</span>

  -  <a href="https://arxiv.org/abs/2107.13062">A General-Purpose, Inelastic, Rotation-Free Kirchhoff-Love Shell Formulation for Peridynamics</a>, <i>Preprint</i>, 2021. 

</p>
</p>



<h2><span style="display:block; margin-top:30px; font-weight: bold;">Air-Blast Fluid-Structure Interaction Modeling Using an Immersed IGA-Peridynamics Approach</span></h2>

<p>
<figure>
  <img align="right" Padding="210px" src="./figures/ABSI.png" width="700">
</figure>
  
<p style='text-align: justify;'> 
It is vital to mitigate the effects of blasts or hypervelocity impact on civil infrastructures. To assess the vulnerability of a given structure under blast loading, numerical simulations of such events can play an effective role in predicting the structural response.
We have recently formulated a novel formulation based on an immersed coupling of Isogeometric Analysis (IGA) and Peridynamics (PD) for the simulation of fluid–structure interaction (FSI) phenomena for air blast. Our aim is to develop a practical computational framework that is capable of capturing the mechanics of air blast coupled to solids and structures that undergo large, inelastic deformations with extreme damage and fragmentation. An immersed technique is used, which involves an <i>a priori</i> monolithic FSI formulation with the implicit detection of the fluid-structure interface and without limitations on the solid domain motion. The coupled weak forms of the fluid and structural mechanics equations are solved on the background mesh. Correspondence-based PD is used to model the meshfree solid in the foreground domain. We employ the Non-Uniform Rational B-Splines (NURBS) IGA functions in the background and the Reproducing Kernel Particle Method (RKPM) functions for the PD solid in the foreground. We feel that the combination of these numerical tools is particularly attractive for the problem class of interest due to the higher-order accuracy and smoothness of IGA and RKPM, the benefits of using immersed methodology in handling the fluid-structure coupling, and the capabilities of PD in simulating fracture and fragmentation scenarios. A great deal of numerical complexity is eliminated as there is no need to explicitly track crack interface (advantage of using PD) or fluid-structure interfaces (advantage of using immersed techniques). The developed computational methodology is applied to the simulation of fracture in brittle and ductile solids in an air-blast environment.

  <span style="display:block; margin-top:20px; margin-bottom:-12px;">**Selected Publications**</span>

  -  <a href="https://arxiv.org/abs/2108.11265">Coupling of IGA and Peridynamics for Air-Blast Fluid-Structure Interaction Using an Immersed Approach</a>, <i>Preprint</i>, 2021. 

</p>
</p>



<h2><span style="display:block; margin-top:30px; font-weight: bold;">A Unified, Stable and Accurate Meshfree Framework for Peridynamic Correspondence Modeling</span></h2>

<p>
<figure>
  <img align="right" Padding="210px" src="./figures/unifiedPD.png" width="700">
</figure>
  
<p style='text-align: justify;'> 
The overarching goal of this project was to develop an accurate, robust, and stable methodology for finite deformation modeling using strong-form peridynamics (PD) and the correspondence modeling framework. We adopted recently developed methods that make use of higher-order corrections to improve the computation of integrals in the correspondence formulation. A unified approach was presented that incorporates the reproducing kernel (RK) and generalized moving least square (GMLS) approximations in PD to obtain non-local gradients of higher-order accuracy. We showed, however, that the improved quadrature rule does not suffice to handle instability issues that have proven problematic for the correspondence-model based PD. To address the shortcomings, a bond-associative, higher-order core formulation was developed that naturally provides stability without introducing artificial stabilization parameters. With a series of numerical benchmarks, we studied the convergence of RK-PD, GMLS-PD, and their bond-associated (BA) versions to a local counterpart, as the degree of non-locality (i.e., the PD horizon) approaches zero. Problems from linear elastostatics were utilized to verify the accuracy and stability of our approach. Our results show that the BA approach improves the robustness of RK-PD and GMLS-PD formulations, which is essential for practical applications. The higher-order, bond-associated model can obtain second-order convergence for smooth problems and first-order convergence for problems involving field discontinuities, such as curvilinear free surfaces. We used our unified PD framework to study wave propagation phenomena, which have proven problematic for the state-based correspondence PD framework. We showed that the improved stability and accuracy of the developed formulation results in significantly less wave dispersion. Furthermore, we proposed a new methodology to enforce natural boundary conditions in correspondence PD formulations. Our results indicate that the bond-associative stabilization method accompanied by higher-order gradient corrections provide the key ingredients to obtain the necessary accuracy, stability, and robustness characteristics needed for engineering-scale simulations.

  <span style="display:block; margin-top:20px; margin-bottom:-12px;">**Selected Publications**</span>

  -  <a href="https://link.springer.com/article/10.1007/s42102-020-00040-z">A Unified, Stable and Accurate Meshfree Framework for Peridynamic Correspondence Modeling—Part I: Core Methods</a>, <i>Journal of Peridynamics and Nonlocal Modeling</i>, 2021. 
  -  <a href="https://link.springer.com/article/10.1007/s42102-020-00039-6">A Unified, Stable and Accurate Meshfree Framework for Peridynamic Correspondence Modeling—Part II: Wave Propagation and Enforcement of Stress Boundary Conditions</a>, <i>Journal of Peridynamics and Nonlocal Modeling</i>, 2021. 

</p>
</p>



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
  The behavior of granular materials under penetration is fundamental to many industries including civil, energy, and defense. Although there is considerable literature on experimental and numerical research on the dynamics of granular matter under impact loading, the behavior is still not well understood. One way to gain more insights into the continuum-scale physics is to study the underlying scales. Mesoscale modeling can be adopted to explicitly resolve the deformation of individual grains, their interactions with each other or the surrounding fluid (e.g., air or water). We developed a meshfree computational framework for Lagrangian peridynamic-based mesoscale simulation of granular particles under shock loading. We explicitly consider intra-granular fracture and inter-particle contact and friction in our modeling approach. In this study, we simulated the shock wave perturbation decay experiment, which is a technique that involves monitoring the evolution of a perturbation in a shock wave front as it propagates through a material field and has been explored to probe the high-rate shear response of granular materials. We conducted a systematic investigation of the effects of grain fracture and frictional contact forces between grains on the continuum behavior of granular materials. A sensitivity assessment of dominant factors indicated that grain fracture, a phenomenon ignored in most computational investigations of granular materials, plays a large role in the bulk dynamic response. Our results show that the wave propagates faster with an increase in the toughness of the material and the inter-particle friction. Also, the shock amplitude was shown to decay faster in tougher materials. It was further confirmed that under strong compression self-contact among fractured grain sub-particles cannot be neglected. 


  <span style="display:block; margin-top:20px; margin-bottom:-12px;">**Selected Publications**</span>

  -  <a href="https://link.springer.com/article/10.1007/s40870-018-0174-2">Peridynamics Modeling of a Shock Wave Perturbation Decay Experiment in Granular Materials with Intra-Granular Fracture</a>, <i>Journal of Dynamic Behavior of Materials</i>, 2018. 
  -  <a href="https://aip.scitation.org/doi/abs/10.1063/1.5044814">Modeling Perturbed Shock Wave Decay in Granular Materials with Intra-Granular Fracture</a>, <i>AIP Conference Proceedings</i>, 2018. 
  -  <a href="https://www.osti.gov/servlets/purl/1348102">Perturbation Decay Experiments on Granular Materials</a>, <i>Sandia National Lab. (SNL-CA)</i>, 2016. 
</p>
</p>


