# Title Generator From Text
This project aims to use an LSTM (Long Short-Term Memory) language model to learn from two databases containing titles and texts, and generate a headline based on the given text. The project utilizes two databases: one consists of text files located in a specific folder on Google Drive, and the other is a database obtained from a CSV file named 'fakenewdata.csv' containing title and text data.

The project starts by mounting Google Drive and importing the necessary libraries for data processing. Then, the folder path where the text files are located is defined, and the content of the files is read. The content is split into titles and texts, and these data points are added to a DataFrame.

Next, the 'fakenewdata.csv' file is read, creating a DataFrame called fake_data that contains the title and text data. This DataFrame is concatenated with the other data to create the data DataFrame using pd.concat.

A function called prepare_text is defined to preprocess the text data. The preprocessing steps involve removing punctuation, numbers, converting uppercase letters to lowercase, removing non-Latin characters, and eliminating non-English characters. This function is applied to the 'title' and 'text' columns of the data DataFrame, processing the data before further use.

Finally, an LSTM language model is trained on the data DataFrame. The LSTM model takes in the title and text data and creates a language model based on this information. This language model can be used to generate text-based headlines.

The project involves training a language model based on the title and text data from the database, preprocessing the text data, and then using the language model to generate a text headline.

## Datasets

https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification

https://www.kaggle.com/datasets/pariza/bbc-news-summary?resource=download
