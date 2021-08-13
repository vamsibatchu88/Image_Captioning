# Image_Captioning
Step 1 is to read the information from this file and store it in variable doc
Doc is a string variable

Step 2:
Now we have to separate Image ID and Image caption from doc variable. load_descriptions
Function is created. We will do it line by line means, we will split the data with \n. Next for each line we will splut the text on spaces. Token[0] will haveimage id and token[1:] will have caption

Step 3:
Clean the captions that 
a)	Lower case
b)	Remove punctuations
c)	Remove alphanumberic

Step 4: Get the vocabulary of words using set() function

Step 5: Save description 

Step 6: Add startseq & endseq to training captions

Step 7: Take Inception v3 model weights and encode the train images

Step 8: Train the model with 2 inputs
a)	Encoded Image vector
b)	Embedded matrix for training images vocabulary
