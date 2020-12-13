## Complex valued GmdhPy

## Motivation

Even thought the GMDH method has been around for over 40 years, research with it using a fully complex dataset is fairly scarce.

When working with a complex valued system, a variety of techniques show ways to convert those complex numbers to a real system, in order to be modeled by a real valued algorithm. Most of the time, this means separating in independent systems for predicting the real/imaginary parts in separate (or abs/phase, or any other coordinate system chosen). Two problems emerge here: if we separate the parts of the complex value, we'll end up with around double the number of kernels to be predicted/stored, and also might loose any correlation happening between both parts (this was an issue with my field of research, RFPA modeling)

## The algorithm

A python package for Gmdh that works with complex values was not found. This is a modification of Konstantin Kolokolov "GmdhPy" python package, available at:

'''
https://github.com/kvoyager/GmdhPy
'''

All credit go to him, since this is only a mod of his work. Also, the operation of the functions are very detailed in his README. 
