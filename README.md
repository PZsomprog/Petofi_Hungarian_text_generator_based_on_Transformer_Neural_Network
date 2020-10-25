# Petofi_Hungarian_text_generator_based_on_Transformer_Neural_Network

The repository contains 2 functions:

1. The first merges multiple text files (utf-8 txt files) to a single file. This file will be the training, test and validation dataset.
2. The second preprocesses a text file. It expands contractions, removes spaces before new lines, removes excess new line characters. Furthermore it replaces punctuations, breaks sentences into new lines, separates words and build the training, test and validation database.

The usage of the program:

1. Collect al txt file you want to merge into a folder: input_generator(text_merger)/books. (The folder structure under it doesn’t matter)
2.  Run the textmerger.ipynb notebook file. The code merges all files in the book folder. The output file called “combinedalldata” is created with input_generator(text_merger)
3. Copy the output file into the inputs/combinedtext folder
4. The folder inputs/dictionaries contains two text files called "abbreviations" and "punctuations”. These will be read into a python dictionary which will replace the elements of the left column with the elements in the right column if found in the text. (Caution the  = caracter is the separator in the text files, spaces will be also taken into account.)
5. Run textcleaner.ipynb. It creates files to the output folder. These files are the following: prepareddata (the entire tokenized text) and databasetrain,databasetest,databasevalid (the training, test and validation data respectively)
