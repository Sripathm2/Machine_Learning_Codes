# Kaggle
Kaggle datasets with Sid Dhar.

My notes:

1) df.isnull().sum() is used to find nulls in dataset.
2) For linear regression number of layers required around sqrt(number of features).
3) For CNN you can use this formula [(W-K+2P)/S]+1
   W is the input volume - in your case 128
   • K is the Kernel size - in your case 5
   P is the padding - in your case O i believe
   S is the stride - which you have not provided.
4) For CNN input and output channels are 1 or 3, 1 is greyscale and 3 is rgb color. 