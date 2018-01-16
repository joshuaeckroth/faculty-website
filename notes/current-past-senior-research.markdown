---
title: Senior research ideas
layout: note
---

# Current and past senior research

This page lists senior research students for which I was the advisor. To browse all Math/CS Department senior research over the years, visit the [Math/CS Department website](https://www2.stetson.edu/mathcs/).

## Current senior research

**Kim Chen: "ALPACA: Building Dynamic Cyber Ranges with Procedurally-Generated Vulnerability Lattices"**

**Proposal**: Cybersecurity is quickly becoming an area of paramount importance. Thus, effective education and training, through a balance of foundational and practical knowledge, are important for future security professionals. Cybersecurity proficiency depends on there being no path into the system, and insecure system have multiple paths. This graph thinking mentality is important for students to understand, as it will allow them to view cybersecurity attack scenarios is multiple different ways. However, an instructor cannot develop scenarios that can teach this in a reasonable amount of time, and most frameworks, while able to easily generate dynamic cyber ranges, do not support vulnerability lattices or otherwise multi-step solutions for arbitrary initial and goal state constraints. We propose a system that will meet this need by procedurally generating vulnerability lattices and build the required cyber range needed in order to allow individuals to practice the scenario.

**Malak Patel: "Automatic Data Visualization"**

**Proposal**: As access to data and interest in data analysis grows, so does the need to extract insights from data, particularly with data visualization. An ideal visualization is one that immediately exposes the central relationships among features embedded in the data. We propose an AI system that attempts to automatically produce such visualizations. We plan to model the problem as abductive inference, in which a visualization explains user-selected columns in the dataset. The project will have two phases. During the first semester, we plan to build a system that is capable of automatically producing two different kinds of visualization. During the second semester, we plan to add more visualizations, update the system to automatically select the best visualization according to heuristics, and evaluate the performance of the system with user studies.

**Kathryn Sarullo: "Exploring Classification by Discriminative Interpolation"**

**Proposal**: While there are many machine learning techniques for processing feature vectors, few techniques exist for processing functional data such as time series and curves. Classification by Discriminative Interpolation (CDI) is a recently developed state-of-the-art supervised learning algorithm that performs classification for functional data. CDI fits a model using wavelet basis functions to each curve while attempting to maximize the separation of curves from different classes. Next, a k-Nearest Neighbor (kNN) algorithm is used to predict the class of new, unlabeled curves. We propose to improve CDI’s accuracy and efficiency on a wide range of datasets. We plan to: investigate alternative basis functions such as `tents’ and parabolic functions; improve the kNN algorithm execution time by implementing k-d trees; and consider implementing alternatives to kNN such as Support Vector Machines (SVMs). We plan to evaluate our changes using datasets from the UCR Time Series Classification Archive.

**Acacia Zack: "Artificial Identity: An Interactive Exhibit Exploring the Boundaries of Artificial Intelligence and Vision-Based Identification"**

**Proposal**: Popular interest in vision-based identification is soaring, driven by advancements in video surveillance, self-driving cars, and object recognition. The developments of vision- based identification, particularly face recognition, can be considered both ingenious and unnerving. However, we believe that these reactions are due to negative media coverage of artificial intelligence and a lack of awareness of artificial intelligence’s capabilities and limitations. We propose to build Artificial Identity, an interactive exhibit that allows participants to explore and educate themselves about object identification. Artificial Identity consists of a custom designed system that includes a visualization of convolutional neural networks and the deconvolutions of each convolutional layer.

## Past senior research

### 2016-2017

**Michael Clay: "Git-Advise: An Automated Git Workflow Adviser"**

We built Git-Advise, a software tool that produces a sequence of Git commands that are able to transform a Git repository’s current state into a goal state described by the user. Prolog, a logic programming language, is the foundation of Git-Advise. The project is composed of a command line tool that allows for querying the state of the repository and setting a goal state, and an integration into a graphic user interface created by Dave Musicant and a group of students at Carleton College. The inspiration for this project comes from the EAAI Model AI Assignment “Git Planner.” We expanded on their ideas to build a larger and more capable Git adviser tool.

**Christian Decker: "Scene by Scene Script Generation for Live Action Hollywood Movies"**

Today there is no ”Google for video” that actually searches the con- tent of the video. Content-based video search can be achieved by indexing video scene transcriptions much like a film script. We have developed a tool that automatically processes video and produces a transcript representing its contents. Processing involves scene segmentation, face recognition, speech recognition, scene recognition and behavior recognition. In the first semester we accomplished scene segmentation by implementing existing research. During the second semester we applied modern techniques for face recognition, speech recognition, scene recognition, and behavior recognition.

**Jacob Hell: "Advaisor: A Rule Based Expert System for Academic Advising"**

Academic advising is an essential process for improving student retention and academic performance. When an advisor and student come together in an academic advising session, the student should leave with their questions answered and insight gained toward their academic future. However, there are some questions that a student might have that an advisor might not be prepared to answer. Such questions might relate to majors and minors in other disciplines with which the advisor is not familiar, or complex constraint satisfaction questions regarding graduation requirements and timelines. We believe that the advisor may be freed of much of the burden of delving into the Stetson Catalog and Degree Audit tools, and that advising time may be better spent interacting with the student than solving such queries. We propose a system that will meet this need by engaging in hypothetical reasoning to produce alternative pathways that meet students’ needs and interests. The system will internally represent facts and constraints from the Stetson Catalog and provide advisors and students with a user interface that supports complex queries about coursework, degree requirements, and elective courses based on student interests.

**Richard Roe: "Denial of Service via Internet of Things Devices: Attack Methodologies and Mitigation Techniques"**

The purpose of this research is to compare the effectiveness of traditional Denial of Service (DoS) attack vectors to a new attack method that is specifically designed for use in devices that have limited resources, such as Internet of Things (IoT) devices. New mitigation techniques will also be explored to help prevent, or reduce the effectiveness of, these attacks. While classical DoS attacks generally require both a large source of computing power and a specially crafted payload to be able to efficiently render the target machine or service inoperable, this research will focus on utilizing an attack that uses a generalized payload that targets a wide variety of internet services, and uses as little resources as possible. We will port the attack to common DoS utilities, as well as to a powerful IoT worm, so that the original tools’ attack methods can be compared to the new attack’s effectiveness and resource consumption. Once done, they will again be compared, but when attacking new mitigation techniques specifically designed to thwart both these and other attacks of their class. The results of this research can be applied to helping defend internet-facing web services from attack in both the public and private sector, because a free and open local proxy is cheaper and easier to setup than an online, paid, cloud solution.

### 2015-2016

**Melissa Abramson: "Signer-Independent Recognition of Static ASL Signs"**

As the Deaf community continues to grow, so does the market for tools that aid communication between the Deaf and hearing communities. One such tool is software for automatically recognizing ASL signs that could assist in learning and communicating in ASL. We have investigated the development of such a system that recognizes 28 static ASL signs. We have also developed several tools for data collection, modification, and classification. We found several common machine learning techniques that are not ideal to use for ASL recognition. We also explored the use of Caffe, a deep learning framework using convolutional neural networks. Due to hardware limitations and time constraints, we were not able to complete the training using Caffe and thus are unable to confirm if this is the ideal approach.

**Marisa Gomez: "A Mobile Fitness Application for Asthma Sufferers"**

Asthma sufferers can experience shortness of breath, wheezing and coughing during moderate or high intensity workouts. We developed a mobile fitness application that enables asthma sufferers to safely achieve their fitness goals without having to consult a personal trainer. This mobile application will present exercises for the user to complete, and provide a self rating form for after completion of the exercise. This form will indicate whether the user experienced symptoms of an asthma attack, difficulty in breathing, ease of completing the exercise, and preference for repeating the exercise at a later date. Once the user has completed twenty­five exercises, the application will offer to suggest an exercise based on the learned user preferences and health status. The application will calculate the probability of the user experiencing symptoms for each available exercise, and present the exercise that is the most safe.

**Joshua Letcher: "A Genetic Approach to the University Timetabling Problem"**

I propose two approaches to solving the University Timetabling problem. In the first approach, an optimal solution will be shown using Mixed Integer Programming (MIP). The second approach uses a genetic algorithm to ease the computational cost associated with the MIP approach. While the solutions given by the genetic approach may not be optimal, they are near optimal and much faster to find.

**Alex Ordonez: "Analysis of the Expected Payout of Bitcoin Mining on Common Consumer Hardware"**

Bitcoin does not yet have a solid definition. Some call it a cryptocurrency, some a commodity, some an investment target. Bitcoins can be acquired through distributed computing. Bitcoin mining, however, has an interesting catch. Only one block is added to the Blockchain every ten minutes. Every ten minutes, a Proof of Work is submitted and accepted by the Network. This Proof of Work problem can be distributed among many machines, such as dedicated servers. In this research, we will analyze the implementation of passive, fault-tolerant, client-side distributed Bitcoin mining. Key points of interest include speed, energy efficiency, network latency, client reliability, and population size to optimize Bitcoins acquired per minute. One of the most anticipated outcomes of this research is the possibility to reduce the dependency on advertising revenue on websites and mobile applications. However, the optimizations for solving the Proof of Work involved in mining Bitcoins can be applied to other problems, such as protein folding.

**Katie Porterfield: "Brain Drain: Using Brainwaves and Machine Learning to Detect Errors in Human Problem Solving"**

The Muse Headband is a simple to use EEG machine that provides real­time measurements of brain waves. Using this headband, we built a model using big data and machine learning techniques to interpret brain wave patterns to create a real time feedback system that helps the user understand their cognitive thinking while solving a problem. Once further developed, this model could then be applied in an educational setting to help a student understand how they are progressing through a problem without the interactions of a teacher to support them.

