# Petofi_Hungarian_text_generator_based_on_Transformer_Neural_Network

This text generator repository has 2 function now:

1. it is capable to merge multiple text files (utf-8 txt-s) to one file (this will be later our train,test,valid dataset)
2. and it is able to "preprate" this huge textfile. While the preparation the program
  solves the abbreviations
  deletes all spaces before \n-s or delete all douple \n-s
  searchs and repleaces puctuations
  brake sentences into newlines
  separates words as tokens
  builds the train, test, valid database
  
  
  
 The usage of program:
 1. you need to collect all mergeble files into folder: input_generator(text_merger)/books.
 the folder structure under it doesnt matter.
2. you need to run the textmerger.ipynb notebook file
it will merge all files what are in book folder. and the output file will be : "combinedalldata" which will be produced in input_generator(text_merger) folder

3. you need to copy the output file into inputs/combinedtext folder
4. you need to have your "abbreviations" and "punctuations" dictionaries text files in folder inputs/dictionaries
this dictionaries are txt files, in each txt files there are lines. in each line left there is a word which will be changed to the other word on the right next to =  !!cantunios space does matter!!
5. after that you need to run textcleaner.ipynb file
itt will create files into output folder.
the end output will be:prepareddata and the 3 databasetrain,databasetest,databasevalid files.
