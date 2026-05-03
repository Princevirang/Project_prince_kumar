Introduction
This project explores the application of Deep Learning to identify phase transitions in statistical mechanics. Specifically, a Convolutional Neural Network (CNN) was developed to classify configurations of the 2D Ising Model as either "Ordered" (ferromagnetic) or "Disordered" (paramagnetic).
Motivation for the project
I was working on Ising model in my physics courses and I got this Idea to train a model to identify its phase, since I can train it on ordered and disordered phase, so I can get broader idea of where the critical temperature \(T_c\) lies as the model trained on perfect ordered and disordered images without background noise, as it was genereated with mathematical equation( not e.g a natural image of dog with BG noise) therefore the accuracy is around \(98-100\%\) but near critical temperature \(T_c\) the accuracy droped to 55\% that's because model was trained purely on the clear-cut ordered and disordered phases, feeding it a critical-phase image forces it to guess. It looks at the fractal domains, sees features of both classes, and throws its prediction in air. A 55\% accuracy means the model is practically guessing at random, which is exactly how a binary classifier should behave when handed edge-case data that sits right on the boundary line.
I have also attached evaluation.py in the folder that I used to generate data to test my model.

Instruction on predict.py
I have generated 10 ordered and 10 disordered phase samples, which are test samples (not used for training) and saved those images in the folder data and labelled the images with the phase, for example, the disordered images are saved as disordered\_0, disordered\_1 and so on; similarly for the ordered on and then my model will predict it.



Please read Readme.pdf in the zip folder to understand the project in detail.
