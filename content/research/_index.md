---
projects:
 - 
    title: "Verifiable, Executable Language Design for Cyber-Physical Systems"
    subtitle: Advised by Jean-Baptiste Jeannin
    image: img/ftscs22.jpg
    question: How do we design programs that are both formally verifiable and directly implementable on real systems?
    description: "Cyber-Physical Systems (CPS), such as robots and industrial controls, are often found in demanding applications, and formal verification can give designers the certainty they need to build safer systems. CPS aren’t typically implemented in languages that can be easily verifiable, because the intricacies of their behavior are difficult to characterize. While tools exist for formally verifying models of CPS, it can be challenging to ascertain that the model accurately reflects reality. We combine an augmented type system with the modeling and execution capabilities of synchronous programming to offer both verification and execution on real hardware, without translation. We have successfully demonstrated verifying and implementing an autonomous braking controller on real robots, and plan to continue verifying ever more complex systems. To our knowledge, we are the first project to use our department’s M-Bot platform, a wheeled robot normally used as a teaching tool, in published research.
<br><br>
I currently lead this project, and am involved in nearly all areas, from the development of the type system to the implementation of our language on real hardware. I had formulated much of our language’s type theory, combining the temporal properties of synchronous programs with the verification expressiveness of refinement types. I had also developed our first interfaces between a synchronous language and robot hardware, and continue to contribute to the development of robot firmware and communications architecture. Additionally, I am involved in designing our experiments, which are a highly-visible test of our system’s capabilities, showing physically that our verification can indeed be valid in the real world. The project has grown significantly in scope since its inception, with the goal of eventually becoming a dedicated robotics platform with formal verification built into every level. Such a large project requires significant engineering effort, and over the course of this project, I have mentored ten undergraduate research assistants, who were indispensable in their involvement."

 -
    title: Generalization of Quantitative Semantics
    subtitle: Advised by Jean-Baptiste Jeannin. In collaboration with Konstantinos Mamouras
    question: What functions can we use to communicate how strongly a formal specification is satisfied?
    description: "Typically, verifying a system is binary; its specifications are either satisfied or falsified. However, strongly satisfying a specification is indistinguishable from marginally satisfying it. What if a system that marginally satisfies a specification is perturbed by outside disturbances, such as noise? The strength with which a specification is satisfied can be quantified, and the various methods for deriving said quantity fall under the scope of quantitative semantics. Cyber-physical systems can have many adjustable parameters, and searching the entire space to find an unsafe set of parameters can be tedious. Quantitative semantics can guide this search, serving as an objective to be minimized in an optimization problem. We believe that many quantitative semantics share certain properties, and that there are other properties still which are desirable for certain search methods. From this, we propose a generalization to facilitate the development of new semantics and to determine the requirements for performing various searches in verification. 
<br><br>
My involvement on this project ranges from adapting existing quantitative semantics-based verifiers to our generalized framework, developing new quantitative semantics, and developing experimental benchmarks. Much of this project involves working with MATLAB and Simulink to verify models of real-world systems."

 -
    title: SAT Solver Characterization
    subtitle: Advised by Karem Sakallah. In collaboration with Armin Biere, Yonathan Fisseha, and Mathias Fleury
    image: img/satproject.jpeg
    question: What optimizations work best for solving particular problems?
    description: "Boolean satisfiability, or SAT, solvers, check whether there exists a set of Boolean assignments to variables that makes a set of formulas simultaneously satisfied. In real-world applications, such as digital circuit analysis, these sets of formulas can contain millions of variables and formulas, which makes for an extremely difficult constraint-solving task. Fortunately, there are optimizations that can significantly reduce solving time, but certain optimizations may only work for certain kinds of problems. We examine the properties of problems, solvers, and even computing hardware to draw connections between them, in order to determine which SAT solver optimizations might work best for particular situations. 
<br><br>
I have helped test hundreds of problems on a wide assortment of SAT solvers and their optimizations. I have also been involved with developing automated SAT solver experimentation tools that we have since run on hardware ranging from 90s-era PCs to modern high-performance computing clusters."

 -
    title: Animal Activity Logging and Validation
    subtitle: Advised by Geoffrey Brown, Adam Fudickar, and Bryce Himebaugh. In collaboration with Dustin Brewer, Dillon Gaughan, Timothy Greives, Alex Jahn, Zack Marvel, Devraj Singh, and Samuel Stratton
    image: img/tag.jpeg
    question: How can we efficiently record animal activity data, and how do we know our recordings are correct?
    description: "Animals are constantly on the move, and patterns in their movements provide a valuable trove of information, from migratory habits to man-made effects on their ecosystem. Accelerometer-based activity logging involves placing recording devices on animals to record these movements, which often places tight constraints on the size and mass of activity loggers. These constraints mean that some activity loggers do not have the energy or storage to record everything. They must be able to automatically detect and record only activity of interest to a particular study. Activity loggers must operate unsupervised for months on end, and the most important activities they collect might only happen a few times a year. Thus, researchers need a high level of confidence in the accuracy and reliability of the activity loggers their experiments depend on. 
<br><br>
I helped develop a novel approach to <a href=\"https://github.com/jchen-cs/QValiData\">validating the event detection software running on our activity loggers</a>, which is responsible for recording activities researchers are interested in observing. The method, which simulates models of event detectors using pre-recorded data, enables researchers to instantaneously test event detection without needing to endlessly iterate with real hardware and experiments. The method has helped fine-tune event detectors that have collected hundreds of thousands of hours of experiment data in total. I was also involved with software development and assembly of our smallest loggers, which weigh less than 1g, and are capable of operating for months without recharging. 
<br><br>
In a similar vein, I have also helped develop a “wind tunnel” for characterizing the in-flight behavior of migratory moths. My involvement with this project included designing custom controller PCBs and 3D-printed parts.
<br><br>
Throughout my years on the project, I have worked closely with many of the researchers using our loggers, sometimes providing on-site support during experiments. My time spent alongside these researchers helped familiarize myself with their methods and requirements, which was instrumental in developing future loggers."

 - 
    title: Exploring the Aerodynamic Properties of Small Drone Propellers
    subtitle: Advised by Bryce Himebaugh
    image: img/proptest.jpeg
    question: What factors might influence the thrust output of drones hovering close to the ground?

    description: "Despite being many times smaller than their full-size counterparts, the propellers used by multicopters are subject to similar aerodynamic effects which must be accounted for in flight and in testing. In these experiments, we examined how the height of a drone propeller above the ground influences its thrust output, and the effects of varying ground surface types, such as grass. We also presented a method for visualizing and photographing the aerodynamic effects that occur around small propellers, such as tip vortices. 
<br>
I led this project and designed both the thrust measurement and high-speed photography hardware used in the experiments."


presentations:
 -
    title: "Synchronous Programming and Refinement Types in Robotics: From Verification to Implementation"
    authors:
      - name: Chen J
        me: true
      - name: Vargas de Mendonça JL
      - name: Jalili S
      - name: Ayele B
      - name: Bekele B
      - name: Qu Z
      - name: Sharma P
      - name: Shiferaw T
      - name: Zhang Y
      - name: Jeannin J-B
    year: 2022
    venue: Formal Techniques for Safety-Critical Systems
    type: Oral Presentation
    location: Auckland, New Zealand
    
 -
    title: "A Robotics Programming Language with Compile-Time Formal Verification"
    authors:
      - name: Chen J
        me: true
      - name: Jalili S
      - name: Vargas de Mendonça J L
      - name: Jeannin J-B
    year: 2021
    venue: University of Michigan Engineering Research Symposium
    type: Oral Presentation
    location: Ann Arbor, Michigan
    awards: Research Proposal Honorable Mention

 -
    title: "Validation and Simulation of Accelerometer-Based Activity Loggers"
    authors:
      - name: Chen J
        me: true
      - name: Brown G
      - name: Fudickar AM
    year: 2019
    venue: Indiana University Undergraduate Research Conference
    type: Oral Presentation
    location: Bloomington, Indiana

 - 
    title: "Testing the Developmental Effects of Photoperiodic Cues on Migratory Behavior of the Global Agricultural Pest, Black Cutworm (Agrotis ipsilon)"
    authors:
      - name: Stratton SM
      - name: Chen J
        me: true
      - name: Fudickar AM
    year: 2018
    venue: Animal Behavior Conference, Center for the Integrative Study of Animal Behavior (CISAB)
    type: Poster
    location: Bloomington, Indiana
    
 - 
    title: "Data Collection and Validation of a New Ultra-Lightweight Logger for Studying Animal Behavior."
    authors:
      - name: Gaughan D
      - name: Chen J
        me: true
      - name: Marvel Z 
      - name: Himebaugh B
      - name: Ketterson E
      - name: Brown G
      - name: Fudickar AM
    year: 2018
    venue: Animal Behavior Conference, Center for the Integrative Study of Animal Behavior (CISAB)
    type: Poster
    location: Bloomington, Indiana

 - 
    title: "Up in the Air: Ground Effect of Propellers and Altitude"
    authors:
      - name: Chen J
        me: true
      - name: Himebaugh B
    year: 2016
    venue: Indiana University Undergraduate Research Conference
    type: Poster
    location: Indianapolis, Indiana
---
# Research
**How can we build better tools for verification, and how can we tailor them to various applications?** Verification can be tricky, because rigorous guarantees require rigorous proofs. Verification problems can be either too difficult or too abstract to be applicable to real-life systems. Much of my past and ongoing work involves lowering the barrier to verification and giving users certainty that their verification is valid. The following is a collection of the various projects in which I have been involved, ranging from verifying (and empirically demonstrating) that robots do not crash to characterizing animal movement. 


